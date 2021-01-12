# Bearer Authorization


## bearer token
**is an opaque string, not intended to have any meaning to clients using it. Some servers will issue tokens that are a short string of hexadecimal characters, while others may use structured tokens such as JSON Web Tokens.**

- are sent to the user/client after the initial signin process has completed.
- Clients must make every subsequent request to the server with that token, in the header
- Authorization: Bearer encoded.jsonwebtoken.here
- The server opens the token, does the re-authentication, and then grants or denies access
- In express servers, this can be done in middleware, in conjunction with a user model


## How does a bearer token work?

The Bearer Token is created for you by the Authentication server. When a user authenticates your application (client) the authentication server then goes and generates for you a Token. Bearer Tokens are **the predominant type of access token used with OAuth 2.0.** ... You use the bearer token to get a new Access token.

## JWT

- Basically, JWT is a token format. and JWT is used as a token in the OAuth OAuth is an authorization protocol.
- OAuth uses server-side and client-side storage
- Although JWTs can be encrypted to also provide secrecy between parties, we will focus on signed tokens.
- Signed tokens can verify the integrity of the claims contained within it, while encrypted tokens hide those claims from other parties. When tokens are signed using public/private key pairs, the signature also certifies that only the party holding the private key is the one that signed it.

### Write the following steps in the correct order:

- Register your application to get a client_id and client_secret

- Ask the client if they want to sign in via a third party

- Receive authorization code

- Receive access token

- Make a request to the access token endpoint

- Redirect to a third party authentication endpoint

- Make a request to a third-party API endpoint

![/](https://pieterderycke.files.wordpress.com/2013/03/oauth-windows-phone-authorization-flow.png)

### Terms:

- **Client ID :** At registration the client application is assigned a client ID and a client secret (password) by the authorization server. The client ID and secret is unique to the client application on that authorization server.

-  **Authentication Endpoint :** is an authentication mechanism used to verify the identity of a network’s external or remote connecting device.

- **Access Token Endpoint :** an HTTP endpoint that micropub clients can use to obtain an access token given an authorization code.

- **API Endpoint :**a point at which an application program interface (API) – the code that allows two software programs to communicate with each other – connects with the software program.

- **Authorization Code :** used for any transaction or entry that has restrictions on which users are entitled to access.

- **Access Token :** an object encapsulating the security identity of a process or thread