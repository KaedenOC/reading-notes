# Socket.io

[Web Sockets](https://en.wikipedia.org/wiki/WebSocket)

- A **Web Socket** - communication protocol that provides full-duplex communication channels over a single, long-lived connection between a client and a server.

- The Web Socket **request/response handshake** involves an HTTP-based initial handshake, where the client sends a request to the server and the server responds with a special response accepting the Web Socket connection.

- Once the connection is established, both the client and the server can send messages to each other in real-time without the need for **polling** or continuous requests.

[Socket.io Tutorial](https://www.tutorialspoint.com/socket.io/)

- The event handler `io.on()` in Socket.io allows you to listen for specific events emitted by the server.

- Possible proof of life or proof that the code works as expected could be demonstrated by connecting a client to the server, emitting an event from the server, and verifying that the client receives and handles the event correctly.

- The `socket.emit()` method is used to send an event from the client to the server or to specific clients.

[Socket.io vs Web Sockets](https://www.educba.com/websocket-vs-socket-io/)

- **WebSocket** - protocol that provides a low-level, bidirectional communication channel between a client and a server.

- **Socket.IO** is a library that simplifies real-time communication, built on top of WebSocket and other protocols.

- **Socket.IO** provides additional features like automatic reconnection, event-based communication, and room-based messaging, which WebSocket alone does not offer.

- **Socket.IO** is often used in scenarios where real-time, bidirectional communication is required, such as chat applications, collaborative editing tools, or multiplayer games.

- **WebSocket** is more suitable for cases where a simple, low-level, bidirectional channel is needed, without the need for additional features provided by Socket.IO.

[OSI MODEL](https://www.youtube.com/watch?v=vv4y_uOneC0)

Takeaways:

- Defines how network protocols interact and operate at different layers to enable communication between devices on a network.

- **Seven Layers of the model**: Physical, Data Link, Network, Transport, Session, Presentation, and Application.

[TCP Handshakes Explained](https://www.youtube.com/watch?v=xMtP5ZB3wSk)

- **TCP** - Transmission Control Protocol - reliable and connection-oriented transport protocol. With TCP, data can be delivered successfully and accurately.

- The video explains the process of establishing a TCP connection between a client and a server.

- Like when two people meet for the first time and handshake. The client and server exchange packets to establish a reliable and synchronized connection before the data transmission begins.

## Additional Resources

[Socket.io Documentation](https://socket.io/docs/v4/)

[Socket.io Server API](https://socket.io/docs/v4/server-api)

[Socket.io Client API](https://socket.io/docs/v4/client-api)

[Socket Testing Tool](https://amritb.github.io/socketio-client-tool/)
