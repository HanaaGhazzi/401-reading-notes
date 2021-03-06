# TCP Servers

## TCP (Transmission Control Protocol)

TCP is a standard that defines how to establish and maintain a network conversation through which application programs can exchange data. TCP works with the Internet Protocol (IP), which defines how computers send packets of data to each other. Together, TCP and IP are the basic rules defining the Internet. The Internet Engineering Task Force (IETF) defines TCP in the Request for Comment (RFC) standards document number 793.

## How Transmission Control Protocol works

TCP is a connection-oriented protocol, which means a connection is established and maintained until the application programs at each end have finished exchanging messages. It determines how to break application data into packets that networks can deliver, sends packets to and accepts packets from the network layer, manages flow control and -- because it is meant to provide error-free data transmission -- handles retransmission of dropped or garbled packets and acknowledges all packets that arrive. In the Open Systems Interconnection (OSI) communication model, TCP covers parts of Layer 4, the transport layer, and parts of Layer 5, the session layer.

## What TCP is used for

TCP is used for organizing data in a way that ensures the secure transmission between the server and client. It guarantees the integrity of data sent over the network, regardless of the amount. For this reason, it is used to transmit data from other higher-level protocols that require all transmitted data to arrive. Examples include:

Secure Shell (SSH), File Transfer Protocol (FTP), Telnet: For peer-to-peer file sharing, and, in Telnet's case, logging into another user's computer to access a file. Simple Mail Transfer Protocol (SMTP), Post Office Protocol (POP), Internet Message Access Protocol (IMAP): For sending and receiving email HTTP: For web access These examples all exist at the application layer of the TCP/IP stack and send data downwards to TCP on the transport layer.

## What is the OSI model?

The Open Systems Interconnection (OSI) model is a conceptual model created by the International Organization for Standardization which enables diverse communication systems to communicate using standard protocols. In plain English, the OSI provides a standard for different computer systems to be able to communicate with each other.

The OSI model can be seen as a universal language for computer networking. It’s based on the concept of splitting up a communication system into seven abstract layers, each one stacked upon the last.

OSI model is a layered server architecture system in which each layer is defined according to a specific function to perform. All these seven layers work collaboratively to transmit the data from one layer to another.

The Upper Layers: It deals with application issues and mostly implemented only in software. The highest is closest to the end system user. In this layer, communication from one end-user to another begins by using the interaction between the application layer. It will process all the way to end-user.

The Lower Layers: These layers handle activities related to data transport. The physical layer and datalink layers also implemented in software and hardware. Upper and Lower layers further divide network architecture into seven different layers as below

- Application

- Presentation

- Session

- Transport

- Network, Data-link

- Physical layers

![osi](https://www.blackmoreops.com/wp-content/uploads/2016/05/OSI-Layer-Please-Do-Not-Tell-Secret-Passwords-Anytime-blackMORE-Ops-1.png)


## Advantages of the OSI Model
Here, are major benefits/pros of using the OSI model :

- It helps you to standardize router, switch, motherboard, and other hardware

- Reduces complexity and standardizes interfaces

- Facilitates modular engineering

- Helps you to ensure interoperable technology

- Helps you to accelerate the evolution

- Protocols can be replaced by new protocols when technology changes.

- Provide support for connection-oriented services as well as connectionless 
service.
- It is a standard model in computer networking.

- Supports connectionless and connection-oriented services.

- Offers flexibility to adapt to various types of protocols