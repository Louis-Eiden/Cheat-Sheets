# Websocket Cheat Sheet

---
## **UNDER CONSTRUCTION**
---

A cheat sheet for Websocket commands.

#

[variable] = placeholder for a variable

#

## Table of Contents
- [Introduction](#introduction)
- [WebSocket Basics](#websocket-basics)
- [WebSocket Handshake](#websocket-handshake)
- [Sending and Receiving Messages](#sending-and-receiving-messages)
- [Closing a WebSocket Connection](#closing-a-websocket-connection)
- [WebSocket Libraries and Frameworks](#websocket-libraries-and-frameworks)
- [WebSocket Security](#websocket-security)
- [WebSocket Best Practices](#websocket-best-practices)

## Introduction
WebSocket is a communication protocol that provides full-duplex communication channels over a single TCP connection. It enables real-time, bidirectional communication between a client and a server.

## WebSocket Basics
- WebSocket is based on the HTTP protocol and uses the same ports (80 for HTTP and 443 for HTTPS).
- It provides a persistent connection between the client and the server, allowing both parties to send and receive data at any time.
- WebSocket supports various data formats, including text and binary data.

## WebSocket Handshake
- The WebSocket handshake is an HTTP-based protocol that establishes a WebSocket connection between the client and the server.
- It involves an initial HTTP request from the client and an HTTP response from the server to upgrade the connection to WebSocket.

## Sending and Receiving Messages
- WebSocket allows sending and receiving messages between the client and the server.
- Messages can be sent as text or binary data.
- Both the client and the server can initiate sending messages.

## Closing a WebSocket Connection
- WebSocket connections can be closed by either the client or the server.
- A close frame is sent to indicate the intention to close the connection.
- WebSocket supports graceful closure, allowing both parties to perform cleanup operations before closing the connection.

## WebSocket Libraries and Frameworks
- There are various WebSocket libraries and frameworks available for different programming languages and platforms.
- Some popular options include Socket.IO, SignalR, and WebSocket API in JavaScript.

## WebSocket Security
- WebSocket connections can be secured using SSL/TLS encryption.
- It is important to ensure proper authentication and authorization mechanisms to prevent unauthorized access.

## WebSocket Best Practices
- Use WebSocket only when it provides a clear advantage over other communication protocols.
- Implement appropriate error handling and fallback mechanisms.
- Optimize WebSocket performance by minimizing unnecessary data transfers.


## curl to a websocket server

> curl -i -N -H "Connection: Upgrade" -H "Upgrade: websocket" -H "Host: localhost:8080" -H "Origin: http://localhost:8080" http://localhost:8080
