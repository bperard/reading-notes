# 412

## Web Sockets

- What is a Web Socket?  
A WebSocket is a communication protocol that provides a bi-directional, full-duplex communication channel over a single TCP connection between a client and a server. It enables real-time communication between a client and a server, allowing the server to push new data to the client at any time.

- Describe the Web Socket request/response handshake and what happens once the connection is established.  
The WebSocket protocol starts with an HTTP handshake, in which the client sends an HTTP request to the server. This request includes a special header called "Upgrade," which indicates that the client wants to upgrade the connection to a WebSocket connection. The server responds with a 101 status code, indicating that it accepts the upgrade request and is switching to the WebSocket protocol.

Once the WebSocket connection is established, both the client and the server can send messages to each other. The messages can be of any data type.

- Web Sockets provide a standardized way for the server to send content to a client without first receiving a ____ from that client.  
HTTP request

## Socket.io Tutorial

- What does the event handler io.on() do?  
Event handler that listens for a specified event and executes a callback.

- Describe some possible proof of life or proof that the code works as expected  
Console log an event that is emitted

- What does socket.emit() do?  
Emits an event and a payload for listeners to receive.

## Socket.io vs Web Sockets  

- What is the difference between WebSocket and Socket.IO? (think Git and GitHub, or OAuth and Auth0).  
Socket.IO is a library built on top of the WebSocket protocol

- When would you use Socket.IO?  
Socket.IO provides a higher-level interface and additional features that make it easier to handle real-time communication between a client and a server.

- When would you use WebSockets?  
 If you need low-level control over the WebSocket protocol, or if you have specific performance requirements.

## OSI Model Explained

- What are a couple of key takeaways from this video?  
The OSI (Open Systems Interconnection) model is a conceptual model that describes how data communication takes place in a networked computing environment. It was developed by the International Organization for Standardization (ISO) in 1984 to provide a common framework for designing and implementing network protocols and communication systems.

The OSI model is divided into seven layers, each of which represents a different aspect of data communication:
Physical layer, data link layer, network layer, transport layer, session layer, presentation layer, and application layer.

## TCP Handshakes Explained

- Translate the gist of this video to a non-technical friend  
When two devices want to communicate over a network using TCP (Transmission Control Protocol), they need to establish a connection first. The devices agree on some basic rules for communication, such as how data will be exchanged and how errors will be handled.

The TCP handshake involves a three-way exchange of messages between the two devices. Here's how it works:

The first device synchronize message to the second device.

The second device sends back a synchronize-acknowledge message.

Finally, the first device sends an acknowledge message back to the second device, confirming that the connection has been established.

Once the TCP handshake is complete, the devices can start exchanging data over the network. If there are any errors or problems during the communication, the devices will use the ground rules they established during the handshake to handle them and keep the communication going smoothly.
