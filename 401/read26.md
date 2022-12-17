# Authentication & Production Server

## Reading:
#### What is JSON Web Token?
- JSON Web Token (JWT) is an open standard (RFC 7519) that outlines a condensed and independent method for securely transferring data between parties as a JSON object. The fact that this information is digitally signed allows for verification and confidence. JWTs can be signed using a public/private key pair using RSA or ECDSA or a secret (with the HMAC algorithm).

#### What is the JSON Web Token structure?
- In its compact form, JSON Web Tokens consist of three parts separated by dots (.), which are:

1. Header
- The header typically consists of two parts: the type of the token, which is JWT, and the signing algorithm being used, such as HMAC SHA256 or RSA.
2. Payload
- The second part of the token is the payload, which contains the claims. Claims are statements about an entity (typically, the user) and additional data. There are three types of claims: registered, public, and private claims.
3. Signature
- To create the signature part you have to take the encoded header, the encoded payload, a secret, the algorithm specified in the header, and sign that.

#### When should you use JSON Web Tokens?
1. Authorization: The most typical application of JWT is in this situation. Once logged in, the user can access routes, services, and resources that are authorized with that token by including the JWT in any subsequent requests. Nowadays, JWT is frequently used for single sign-on because of its low overhead and ease of use across several domains.

2. Information Exchange: Information can be securely transmitted between parties using JSON Web Tokens. You can be certain that the senders are who they claim to be because JWTs can be signed, for instance using public/private key pairs. You may also confirm that the content hasn't been altered because the signature is created using the header and the payload.

#### Installation
`pip install djangorestframework_simplejwt`

#### How JWT Works?
- The JWT is acquired by exchanging an username + password for an access token and an refresh token.
- The access token is usually short-lived (expires in 5 min or so, can be customized though).
- The refresh token lives a little bit longer (expires in 24 hours, also customizable). It is comparable to an authentication session. After it expires, you need a full login with username + password again.
