# OSI Model and Socket.io

## OSI Model

the **O**pen **S**ystems **I**nterconnection model is a representation to how networks function, it consist of 7 layers:

1. Physical Layer
2. Data Link Layer
3. Network Layer
4. Transport Layer
5. Session Layer
6. Presentation Layer
7. Application Layer

Every layer abstracts lower level functionality to hide the details from the end user, and each level use different naming convintions than the other; ex: layer 1 label data as *bits* while layer 2 labels it *frames*, also each layer has a different set of issues and problems to deal with and/or solve

---

## Socket.io

To understand *Socket.io* we first need to talk about **WebSocket**, WebSocket establishes a two-way connection between a client and a server, a *handshake* is sent to open a TCP/IP connection, and it stays open until one of the parties drops off. this is referred to as a full-duplex connection.

*Socket.io* is a library built on top of *WebSocket* to add more functionalities and solve some common issues like brodcasting an event to multiple subscribers.
