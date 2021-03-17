# LOCAL STORAGE FOR WEB APPLICATIONS

* Cookies are included with every HTTP request, thereby slowing down your web application by needlessly transmitting the same data over and over
* Cookies are included with every HTTP request, thereby sending data unencrypted over the internet (unless your entire web application is served over SSL)
* Cookies are limited to about 4 KB of data — enough to slow down your application (see above), but not enough to be terribly useful

## INTRODUCING HTML5 STORAGE
What I will refer to as “HTML5 Storage” is a specification named Web Storage.
 **HTML5 Storage** : it’s a way for web pages to store named key/value pairs locally, within the client web browser,**Like cookies**Like cookies, this data persists even after you navigate away from the web site, close your browser tab, exit your browser, or what have you.

# TRACKING CHANGES TO THE HTML5 STORAGE AREA

 If you want to keep track programmatically of when the storage area changes, you can trap the storage event. The storage event is fired on the window object whenever ``setItem()``,`` removeItem()``, or ``clear()`` is called and actually changes something.

 # LIMITATIONS IN CURRENT BROWSERS

**5 megabyte** is how much storage space each origin gets by defaul

**QUOTA_EXCEEDED_ERR** is the exception that will get thrown if you exceed your storage quota of 5 megabytes.

* **SQL** is a standard language for storing, manipulating and retrieving data in databases

