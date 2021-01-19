# Socket.io

## WebSocket

is a computer communications protocol, providing full-duplex communication channels over a single TCP connection. The WebSocket protocol was standardized by the IETF as RFC 6455 in 2011, and the WebSocket API in Web IDL is being standardized by the W3C.

WebSocket is distinct from HTTP. Both protocols are located at layer 5 in the OSI model and depend on TCP at layer 4. Although they are different, RFC 6455 states that WebSocket "is designed to work over HTTP ports 443 and 80 as well as to support HTTP proxies and intermediaries," thus making it compatible with the HTTP protocol.


![web](https://www.xoriant.com/sites/default/files/uploads/2015/02/img4-webS.png)

## Socket.IO

enables real-time bidirectional event-based communication. It works on every platform, browser or device, focusing equally on reliability and speed. Socket.IO is built on top of the WebSockets API (Client side) and Node.js. It is one of the most depended upon library on npm (Node Package Manager).

Socket.IO is a JavaScript library for real-time web applications. It enables real-time, bi-directional communication between web clients and servers. It has two parts:**a client-side library that runs in the browser**, and **a server-side library for node.js**. Both components have an identical API.

## Why Socket.IO?

Socket.IO is quite popular, it is used by Microsoft Office, Yammer, Zendesk, Trello, and numerous other organizations to build robust real-time systems. It one of the most powerful JavaScript frameworks on GitHub, and most depended-upon NPM (Node Package Manager) module. Socket.IO also has a huge community, which means finding help is quite easy.

- It handle all the degradation of your technical alternatives to get full duplex communication in real time.

- It also handles the various support level and the inconsistencies from the browser.

- It also gives the additional feature room support for basic publish infrastructure and thinks like automatic reconnect.

- Currently, AFAIK is the most used one and easier to help with vanilla web sockets.

## Key Differences between WebSocket and socket.io

Both WebSocket vs Socket.io are popular choices in the market; let us discuss some of the major Difference Between WebSocket vs Socket.io:

- It provides the Connection over TCP while Socket.io is a library to abstract the WebSocket connections.

- WebSocket doesn’t have fallback options while Socket.io supports fallback.

- WebSocket is technology while Socket.io is a library for WebSockets.