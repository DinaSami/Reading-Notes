## Authentication

### Review, Research, and Discussion

Singleton in computer science terms refers to a single instance of something.
How singleton pattern can be used with node modules, specifically with classes a singleton pattern can (and should?) be used with node modules so that you only have one area or location in your software that is making the node. This is achieved using class syntax. If tasked with building a middleware system like express uses, what approach might you take to construct/operate it? Express is an app level middleware system that needs to be used throughout the entire app in order for the app to run as an express app.

TERMS Router Middleware: middleware that is applied at the route level meaning that it can be applied to particular routes and take place in the WRRC.
Singleton Pattern: instantiating a single type of object in a single place.
CRUD -> REST method matches: CREATE:POST, READ:GET, UPDATE:PUT, DELETE:DELETE
Mock Testing: creating a testing environment where a mock request can be made to avoid complications from testing on a live site.

### Term

- Router Middleware

- Dynamic Module Loading

-Singleton Pattern

-CRUD -> REST Method Matches

Mock Testing

### Securing Passwords with Bcrypt Hashing Function :

Passwords are the first line of defense against cyber criminals. It is the most vital secret of every activity we do over the internet and also a final check to get into any of your user account, whether it is your bank account, email account, shopping cart account or any other account you have.

Cryptographic hash algorithms MD5, SHA1, SHA256, SHA512, SHA-3 are general purpose hash functions, designed to calculate a digest of huge amounts of data in as short a time as possible. Hashing is the greatest way for protecting passwords and considered to be pretty safe for ensuring the integrity of data or password.

### Basic access authentication 

In the context of an HTTP transaction, basic access authentication is a method for an HTTP user agent (e.g. a web browser) to provide a user name and password when making a request. In basic HTTP authentication, a request contains a header field in the form of Authorization: Basic <credentials>, where credentials is the Base64 encoding of ID and password joined by a single colon :.

HTTP Basic authentication (BA) implementation is the simplest technique for enforcing access controls to web resources because it does not require cookies, session identifiers, or login pages; rather, HTTP Basic authentication uses standard fields in the HTTP header.

### bcrypt

bcrypt is a password-hashing function designed by Niels Provos and David Mazières, based on the Blowfish cipher and presented at USENIX in 1999.[1] Besides incorporating a salt to protect against rainbow table attacks, bcrypt is an adaptive function: over time, the iteration count can be increased to make it slower, so it remains resistant to brute-force search attacks even with increasing computation power.
