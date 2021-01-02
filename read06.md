# HTTP and REST

## HTTP "Hyper Text Transfer Protocol" :
- stateless (request-response) application layer protocol
- used to build distributed, collaborative, hypermedia information systems
- foundation for the world wide web

**HTTP is associated with serving:(.html ,images, videos, .json, .xml, binary executables,...)**

## HTTP Requests (HTTP/1.1):
request is formatted in text and transferred using TCP. The first line of the request contains the ``METHOD``,`` URL``, and ``HTTP VERSION``. The following lines are the request ``HEADERS``.

``Safe`` methods should only be used for information retrieval and should not change the server state.

``Idempotent`` methods means if two identical requests are made they should get an identical response

``Cacheable`` means the client should be able to cache the response.


## HTTP Response :
A HTTP/1.1 response is also formatted in text and transferred using TCP. The first line of the response contains the ``HTTP VERSION``, ``STATUS CODE``, and ``STATUS MESSAGE``.

## REST :

**REST is acronym for REpresentational State Transfer. In layman’s terms, is a means by which we can reference, manipulate, and transfer state.**
REST (REpresentational State Transfer):
to reference, manipulate, and transfer state.

uses a common set of methods ``verbs`` to operate on the state of a resource ``noun``, using ``HTTP`` as the transfer protocol.

![rest](https://images.tutorialedge.net/uploads/rest-api.png)