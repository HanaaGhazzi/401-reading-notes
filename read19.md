# Message Queues

## message
is a package of information, categorized by queue and event queue - Which general bucket does this message belong i.e. “Database Events”, “Filesystem Events”, “Network Events”, etc event - What event has happened i.e. “delete, add, update, connection lost, an error”, etc. payload - data associated with the event i.e. “record id, record information, error text”, etc.

Any connected client can **“publish”** a message into the server. Any connected client can “subscribe” to receive messages by type. The Queue server has the ability to see which clients are connected, to which Queues they are attached and further, to which events they are subscribed.

The Queue server is tasked with receiving any published message and then distributing it out to all connected and subscribed clients. It must further ensure that subscribed clients can “catch up” and pull down any messages that they might have missed during a period of disconnection with the server

##  Queue

“Queue” will keep track of the delivery status of every event/message.

Any broadcast that is not received by a subscriber will remain “in the queue” until it can be delivered.

In this type of systems, rather than a broadcasting of messages, clients will likely “poll” the server to retrieve any messages “in the queue” for them, on their own timeline/schedule.


## Real Time Messaging 

messages are simply brokered by the server. They come in, are processed and are immediately broadcast out to subscribers. Should a subscriber at any point lose connection with the server, any messages broadcast by the server will clearly be missed by the client. These are known as “Real Time” messaging systems.

### terms: 

**Web Socket** communication protocol that provides full-duplex comm over single TCP

**Socket.io** javascript library for building realtime web applications

**Client** a user computer that interacts with a server

**Server** computer that accepts requests from a client and returns data