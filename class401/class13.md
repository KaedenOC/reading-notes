# Message Queues

[Socket.io Chat Example](https://socket.io/get-started/chat/)

Example: Allows users to send messages to eachother. Communication stays open even when users are offline.

- We run `node index.js` to get proof of life on the back end and we see that in our command line: `listening on *:3000`.

- We want to use the `broadcast` flag in order to send an event to everyone except for the socket that triggered the event.

[Rooms](https://socket.io/docs/v4/rooms)

A room is an arbitrary channel that sockets can join and leave. It can be used to broadcast events to a subset of clients.

- To join a room: `socket.join` method on the server side.

>Ex: `socket.join('room_name');`

- To leave a room: `socket.leave` method on server side.

>Ex: `socket.leave('room_name');`

[Namespaces](https://socket.io/docs/v4/namespaces/)

Allows you to create separate communication channels within a single Socket.IO server. It provides a way to partition the WebSocket connections into distinct groups or namespaces based on different functionalities or contexts.

- Separate communication, apply different settings, Manage resource allocation.

- Possible use case is a dashboard application that serves multiple clients or organizations. Each organization might have its own set of data and users. We would use namespaces here to create isolated real-time communication channels.

## Additional Resources

[Socket.io Emit Cheatsheet](https://socket.io/docs/v4/emit-cheatsheet/)

I would like to learn more about socket.io