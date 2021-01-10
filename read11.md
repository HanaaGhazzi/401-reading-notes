# Authentication:

## User Modeling
**Modern web applications need to model sensitive information about their users.**

## Cryptography

_Cryptography is the science which studies methods for encoding messages so that they can be read only by a person who knows the secret information required for decoding, called the key which include the cryptanalysis_

![/](https://image1.slideserve.com/2390327/what-is-cryptography-l.jpg)

### cryptanalysis
_is the science of decoding a encoded method without having the proper key._

## Hashing Algorithms
Cryptographic Hash Algorithm takes a piece of data and produces a hash that is deliberately difficult to reverse.

![//](https://cdn.auth0.com/blog/hashing-one-way-road-to-security/hash-flow.png)

## cypher algorithms
- user token can be created by a random unique string (tokenseed) with a user account,
- encrypting the tokenseed with a unique key only the server knows, so we can send the encrypted key to the client,
- client send a request with the encrypted key, and the server decode the key back to the tokenssed, and send the data.


## Basic authorization,
is a method for an HTTP user agent (e.g. a web browser) to provide a user name and password when making a request.

#### they are joined by :
- "base 64encoded" and placed after the string,
- server can return the username and password, if the combination is valid,
- server responds with a validation response, which lets the user to re-authenticate with sending the user name and password every time,

## JSON Web Token?

JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object.

- use JSON Web Tokens:
- Authorization
- Information Exchange