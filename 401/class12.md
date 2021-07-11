## Socket.io

### REVIEW, RESEARCH & DISCUSSION

- The benefit of transforming data into packets is to be able to transfer them individually to reach their destination.  Upon reaching their destination, the destination recompiles the data passed thru the packet to adhere to the protocols of whichever TCP/UDP level they are at in the process.

- UDP is often refered to as a connectionless protocol because as a connectionless protocol it does not require the two endpoints (sending and recieving) to have an established connection.  I think that this is what allows the emit of listeners without needing a server set up?

- Can socket server application have multiple socket connections? Yes!

- Can a socket connection application be connected to multiple socket servers? Maybe!

- Can an application be both a socket server and a socket connection? No, they would need to be in different files. Also can someone tell me if these answers are correct?

### Terms

- Observer pattern "is a behavioral design pattern that lets you define a subscription mechanism to notify multiple objects about any events that happen to the object they’re observing.This is what allows us to emit into a "hub" and have whichever applications that are connected to that "hub" be able to listen for what is emitted and then act accordingly. 

- Listener: waits for a predefined (or just created/emitted) event to occur before running code. 

- Event Handler: is the function that is run which is dependent upon the event listener having happened

- Event Driving Programming: is our CAPS lab and essentially what we are focusing on now.  In event driven programming there are no function calls, rather, functions are ran based on the presence of an event happening.  It is the event (listener) that invoked the handler (function).

- Event Loop: the event loop is the flow of an even driven programming app.  Where one event triggers a handler which could emit an additional event or prompt change to the payload of an already existing event. 

- Event Queue: "an event queue is a repo where events from an application are held prior to being procesed by a receiving program or system

- Call stack: "a mechanism for an interpreter (like JavaScript in a web browser) to keep track of its place in a script that calls multiple functions
- Emit/Raise/Trigger: these words are synonymous and refer to when an event is being created using the emit() method

- Subscribe: establishing a connection between a server and an application.  This allows the application to receive information from the server and vice versa and happens after the "three-way handshake". Syn/Ack also are involved here, I believe. 

- database: a structured way to store data locally so as to not make repetive requests/receive repetitive responses. 

### Preparation Materials

WebSocket : is a computer communications protocol, providing full-duplex communication channels over a single TCP connection. The WebSocket protocol was standardized by the IETF as RFC 6455 in 2011, and the WebSocket API in Web IDL is being standardized by the W3C.

WebSocket is distinct from HTTP. Both protocols are located at layer 7 in the OSI model and depend on TCP at layer 4. Although they are different, RFC 6455 states that WebSocket "is designed to work over HTTP ports 443 and 80 as well as to support HTTP proxies and intermediaries," thus making it compatible with HTTP. To achieve compatibility, the WebSocket handshake uses the HTTP Upgrade header[1] to change from the HTTP protocol to the WebSocket protocol.

Socket.IO enables real-time bidirectional event-based communication. It works on every platform, browser or device, focusing equally on reliability and speed. Socket.IO is built on top of the WebSockets API (Client side) and Node.js. It is one of the most depended upon library on npm (Node Package Manager).

Socket.IO is a library that enables real-time, bidirectional and event-based communication between the browser and the server. It consists of:

- a Node.js server: Source | API
- a Javascript client library for the browser (which can be also run from Node.js): Source | API

```
const socket = new WebSocket("ws://localhost:3000");

socket.onopen = () => {
  socket.send("Hello!");
};

socket.onmessage = (data) => {
  console.log(data);
};
```
