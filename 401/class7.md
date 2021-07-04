## Bearer Authorization

### Put in correct order:

- register your app to get a client_id and client_secret

- ask client if they want to sign in via a 3rd party

- redirect to 3rd party authentication endpoint

- make a request to a 3rd party API endpoint

- recieve authorization code

- make request to access token endpoint

- receive access token

### What can you do with an authorization code?

with an authorization code you can split and decode to compare if user entered text exists in database

### What can you do with an access token?

with an access token a user is granted access to defined routes.

### What's a benefit of using OAuth instead of your own basic authentication? 

sharing user data between applications without sharing the user's credentials. For ex: logging into spotify thru facebook or logging into codepen account using your github login credentials. "known as secure, third-party, user-agent, delegated authorization".
VOCAB Client ID username or some information unique to the user.

## Preview

Client secret is app level environment variable. Adds a second layer of verification to the token created.

Authentication endpoint the route in which authentication occurs.

API Endpoint "the means from which teh API can access the resources they need from a server to perform their task...the location where the API sends a request and where the response emenates is what is known as an edpoint...it is what the developer will implemente to make their requests" https://rapidapi.com/blog/api-glossary/endpoint/

Authorization code sent thru headers and is then decoded and compared (is this right??)

Access Token username + secret = authentication token

## Term

+ Client ID
Client Secret
Authentication Endpoint
Access Token Endpoint
API Endpoint
Authorization Code
Access Token

### JWT :

#### What is JSON Web Token?

JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed. JWTs can be signed using a secret (with the HMAC algorithm) or a public/private key pair using RSA or ECDSA.

#### What is the JSON Web Token structure?

In its compact form, JSON Web Tokens consist of three parts separated by dots (.), which are:

- Header : The header typically consists of two parts: the type of the token, which is JWT, and the signing algorithm being used, such as HMAC SHA256 or RSA.

```
{
  "alg": "HS256",
  "typ": "JWT"
}
```

- Payload : The second part of the token is the payload, which contains the claims. Claims are statements about an entity (typically, the user) and additional data

```
{
  "sub": "1234567890",
  "name": "John Doe",
  "admin": true
}
```

- Signature : To create the signature part you have to take the encoded header, the encoded payload, a secret, the algorithm specified in the header, and sign that.

```
HMACSHA256(
  base64UrlEncode(header) + "." +
  base64UrlEncode(payload),
  secret)
  ```
  


