## Event Driven Applications


### REVIEW, RESEARCH & DISCUSSION
- Access control is important for site management, in that it gives certain users certain access to certain areas of the site.  

- The word press hosted website that my organzation uses is an example of a web application that benefits from access control.  Only one person is able to make an post edits to pages, as the admin, and other people are only able to view content or edit but not update. 

- A role is used to determine what a user has access and the ability to do within the site. 

- Role based access "makes it simple for owners to manage users in groups based on their role or position, rather than assigning permissions to each specific individual. RBAC largely eliminates discretion when providing access to objects" [source](https://umbrellatech.co/access-control/system-types/)

- Authorization: authorization typically requires a bearer token of the user.  Access to different resources within a site is based on the token that connected a particular user.

- Role Based Access Control: granted permission and access to resources or areas of a site based on attributes associated with a users defined role. 

- Capabilities: are what and how the user is able to access or contribute to a site.  Example of capabilities could be the ability to edit users, create users or delete users. 

### Document the following Vocabulary Terms

- Authorization
- Role Based Access Control
- Capabilities

### Event-Driven Programming in Node.js

Event-Driven Programming is a logical pattern that we can choose to confine our programming within to avoid issues of complexity and collision.For the most recognizable example of Event-Driven Programming for people at any level of programming skill, we’ll turn to our old friend The Web Browser.

Event-Driven Programming makes use of the following concepts:

- An Event Handler is a callback function that will be called when an event is triggered.
- A Main Loop listens for event triggers and calls the associated event handler for that event.

EventEmitter

Node.js natively provides us with a useful module called EventEmitter that allows us to get started incorporating Event-Driven Programming in our project right away. 

```
const EventEmitter = require('events').EventEmitter;
const myEventEmitter = new EventEmitter;
```

Removing Listeners

There will likely come a time when you want to remove an event listener from an event. This could be for performance reasons (the event is no longer needed) or to avoid memory leaks (if an event listener references an object that is no longer needed, it won’t be able to be garbage-collected. This can lead to a build up of unnecessary objects).

```
const EventEmitter = require('events').EventEmitter;
const chatRoomEvents = new EventEmitter;

function userJoined(username){
  chatRoomEvents.on('message', function(message){
    document.write(message);
  })
}

chatRoomEvents.on('userJoined', userJoined);
```

