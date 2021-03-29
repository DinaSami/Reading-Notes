## JavaScript
### Table of content

**The Past, Present, and Future of Local Storage for Web Applications**

 **Cookies** were invented early in the web’s history, and indeed they can be used for persistent local storage of small amounts of data. But they have three potentially dealbreaking downsides:

- Cookies are included with every HTTP request, thereby slowing down your web application by needlessly transmitting the same data over and over
- Cookies are included with every HTTP request, thereby sending data unencrypted over the internet (unless your entire web application is served over SSL)
- Cookies are limited to about 4 KB of data — enough to slow down your application (see above), but not enough to be terribly useful


In the beginning, there was only **Internet Explorer** . Or at least, that’s what Microsoft wanted the world to think. To that end, as part of the First Great Browser Wars,Internet Explorer.
One of these things was called DHTML Behaviors, and one of these behaviors was called **userData**.

In 2002, Adobe introduced a feature in Flash 6 that gained the unfortunate and misleading name of **“Flash cookies.”** Within the Flash environment, the feature is properly known as *Local Shared Objects**.
 
what is **HTML5 Storage** ? Simply put, it’s a way for web pages to store named key/value pairs locally, within the client web browser. 
 
HTML5 Storage is based on named key/value pairs. You store data based on a named key, then you can retrieve that data with the same key.

HTML5 storage:

- HTML5 Storage specification
- Introduction to DOM Storage on MSDN
- Web Storage: easier, more powerful client-side data storage on Opera Developer Community
- DOM Storage on Mozilla Developer Center. (Note: most of this page is devoted to Firefox’s prototype implementation of a globalStorage object, a non-standard precursor to localStorage. Mozilla added support for the standard localStorage interface in Firefox 3.5.)
- Unlock local storage for mobile Web applications with HTML5, a tutorial on IBM DeveloperWorks
