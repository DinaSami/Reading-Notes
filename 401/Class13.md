## Message Queues

## Review, Research, and Discussion

- **What does it mean that web sockets are bidirectional? Why is this userful?** This means that sockets can facilitate information flowing into and out of a socket connection between a socket server and client.

- **Does socket.io use HTTP? Why?** Socket.io uses HTTP when a websocket is unable to be established. [Source](https://socket.io/docs/v4/index.html)

- **What happens when a client emits an event?** when a client emits an event, it travels to thru the socket to the server.

- **What happens if a client "misses" an event?** The event is ignored and does not trigger any subsquent code. 

- **How can we mitigate this?** I would think with some added logic or error handling functions you would be able to track missed events and debug. 
- 

## Terms

- **Socket vs. Web Socket**: "WebSockets typically run from browsers connecting to Application Server over a protocol similar to HTTP that runs over TCP/IP. So they are primarily for Web Applications that require a permanent connection to its server. On the other hand, plain sockets are more powerful and generic. They run over TCP/IP but they are not restricted to browsers or HTTP protocol. They could be used to implement any kind of communication." [source](https://stackoverflow.com/questions/4973622/difference-between-socket-and-websocket#:~:text=WebSockets%20typically%20run%20from%20browsers,are%20more%20powerful%20and%20generic.)

- **Socket.io**: "is a library that enables real-time, bidirectional and event-based communication between the browser and the server" [source](https://socket.io/docs/v4/index.html#What-Socket-IO-is) 

- **Client**: can be thought of as the browser. It connects to an established server and makes requests. 

- **Server**: responds to requests from the client.

- **OSI Model (Operations Systems Interconnection Model)**: Application -> Presentation -> Session -> Transport -> Network -> Data Link -> Physical.  Explains how information is passed thru the internet from the browser all the way down to the fiberoptic wires. 

- **TCP Model(Transmission Control Protocol)**: uses less, but in effect more concise, levels as OSI to demonstrate how information is passed over the internet.  It requires that all information from the server be present in order to fulfull the clients request. 

- **UDP (User Datagram Protocol)**: is similar to TCP except for that it allows for not all of the data to be present in the servers response to the client.  An example of UDP is a streaming platform and when the client has to pause to buffer the streaming content.

- **Packets**: refer to the way that data is sent in the TCP model.

### Rooms

A room is an arbitrary channel that sockets can join and leave. It can be used to broadcast events to a subset of clients.

```
io.on('connection', socket => {
  socket.join('some room');
});
```
### Default room

Each Socket in Socket.IO is identified by a random, unguessable, unique identifier Socket#id. For your convenience, each socket automatically joins a room identified by its own id.

### Usage with asynchronous code

Please make sure to use io.to(...).emit(...) (or socket.to(...).emit(...)) in a synchronous manner.

### Disconnection

Upon disconnection, sockets leave all the channels they were part of automatically, and no special teardown is needed on your part.

### Implementation details

The “room” feature is implemented by what we call an Adapter. This Adapter is a server-side component which is responsible for:

- storing the relationships between the Socket instances and the rooms
- broadcasting events to all (or a subset of) clients

```
// main namespace
const rooms = io.of("/").adapter.rooms;
const sids = io.of("/").adapter.sids;

// custom namespace
const rooms = io.of("/my-namespace").adapter.rooms;
const sids = io.of("/my-namespace").adapter.sids;
```

