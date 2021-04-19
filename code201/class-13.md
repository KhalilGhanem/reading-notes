# Local Storage

## Cookies
Cookies were invented early in the web’s history, they can be used for persistent local storage of small amounts of data, But they have three downsides:

* Cookies are included with every HTTP request, thereby slowing down your web application by needlessly transmitting the same data over and over
* Cookies are included with every HTTP request, thereby sending data unencrypted over the internet (unless your entire web application is served over SSL)
* Cookies are limited to about 4 KB of data — enough to slow down your application (see above), but not enough to be terribly useful

## HTML5 Storage
it’s a way for web pages to store named key/value pairs locally, within the client web browser. Like cookies, this data persists even after you navigate away from the web site, and this data is never transmitted to the remote web server.

* HTML5 Storage is based on named key/value pairs.
* You store data based on a named key, then you can retrieve that data with the same key. The named key is a string. 
* The data can be any type supported by JavaScript.
* If you are storing and retrieving anything other than strings, you will need to use functions like parseInt().

## Storage Objects
HTML web storage provides two objects for storing data on the client:
* window.localStorage - stores data with no expiration date
* window.sessionStorage - stores data for one session (data is lost when the browser tab is closed)

Storage Objects methods:
* setItem() : we use it to storing data to Storage Object
* getItem() : we use it to retrieving data from Storage Object
* clear() : We use it to clear the data from the Storage Object