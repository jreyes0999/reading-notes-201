# Local Storage

- Cookies were invented early in the web’s history, and indeed they can be used for persistent local storage of small amounts of data. But they have three potentially deal breaking downsides:
  - Cookies are included with every HTTP request, thereby slowing down your web application by needlessly transmitting the same data over and over
  - Cookies are included with every HTTP request, thereby sending data unencrypted over the internet (unless your entire web application is served over SSL)
  - Cookies are limited to about 4 KB of data — enough to slow down your application (see above), but not enough to be terribly useful

## So what is HTML5 Storage?
- Simply put, it’s a way for web pages to store named key/value pairs locally, within the client web browser. Like cookies, this data persists even after you navigate away from the web site, close your browser tab, exit your browser, or what have you. Unlike cookies, this data is never transmitted to the remote web server.

## CHECKS FOR HTML 5 STORAGE
```
function supports_html5_storage() {
  try {
    return 'localStorage' in window && window['localStorage'] !== null;
  } catch (e) {
    return false;
  }
}
```

## DETECTS SUPPORT FOR HTML 5 STORAGE
```
if (Modernizr.localstorage) {
  // window.localStorage is available!
} else {
  // no native support for HTML5 storage :(
  // maybe try dojox.storage or a third-party solution
}
```
## HTML5 STORAGE
- HTML5 Storage is based on named key/value pairs. 
- You store data based on a named key, then you can retrieve that data with the same key. The named key is a string. 
- The data can be any type supported by JavaScript, including strings, Booleans, integers, or floats. However, the data is actually stored as a string. If you are storing and retrieving anything other than strings, you will need to use functions like parseInt() or parseFloat() to coerce your retrieved data into the expected JavaScript datatype.

- Calling setItem() with a named key that already exists will silently overwrite the previous value. Calling getItem() with a non-existent key will return null rather than throw an exception. Like other JavaScript objects, you can treat the localStorage object as an associative array. Instead of using the getItem() and setItem() methods, you can simply use square brackets.

- If you want to keep track programmatically of when the storage area changes, you can trap the storage event. The storage event is fired on the window object whenever setItem(), removeItem(), or clear() is called and actually changes something.

## STORAGE EVENT OBJECT
* PROPERTY - key, oldValue, newValue, url* 
* TYPE - string, any, any, string
* DESCRIPTION - the named key that was added, removed, or modified // the previous value (now overwritten), or null if a new item was added // the new value, or null if an item was removed // the page which called a method that triggered this change

- “5 megabytes” is how much storage space each origin gets by default. This is surprisingly consistent across browsers, although it is phrased as no more than a suggestion in the HTML5 Storage specification. One thing to keep in mind is that you’re storing strings, not data in its original format. If you’re storing a lot of integers or floats, the difference in representation can really add up. Each digit in that float is being stored as a character, not in the usual representation of a floating point number.
- “QUOTA_EXCEEDED_ERR” is the exception that will get thrown if you exceed your storage quota of 5 megabytes. “No” is the answer to the next obvious question, “Can I ask the user for more storage space?”  is purely a user-initiated action, not something that you as a web developer can build into your web application.
