User Modeling
  1. User models that have sensitive data that should NEVER be sent to client applications. If your application requires that users be able to read each others personal information, create a second Profile model to hold that data and strictly limit access to the Profile model. Safely using a second model will ensure that no users will accidentally (or maliciously) get access to sensitive information.
  2. Cryptography is the science which studies methods for encoding messages so that they can be read only by a person who knows the secret information required for decoding, called the key; it includes cryptanalysis, the science of decoding encrypted messages without possessing the proper key.
  3. A Cryptographic Hash Algorithm takes a piece of data and produces a hash that is deliberately difficult to reverse. If identical data is passed into the algorithm the same hash will always be produced. Hash algorithms are often used for checking the integrity of data.
  4. A Cryptographic Cypher Algorithm takes a piece of data and a key and produces encrypted data. Later the encrypted data can be reversed into the original data by decrypting it using the same key.

Basic Access Authentication
  1. A method for an HTTP user agent (e.g. a web browser) to provide a user name and password when making a request. In basic HTTP authentication, a request contains a header field in the form of Authorization: Basic <credentials>, where credentials is the Base64 encoding of ID and password joined by a single colon :
  2. HTTP Basic authentication (BA) implementation is the simplest technique for enforcing access controls to web resources because it does not require cookies, session identifiers, or login pages; rather, HTTP Basic authentication uses standard fields in the HTTP header.
  
JSON Web Tokens
  1. JSON Web Token (JWT) is an open standard (https://tools.ietf.org/html/rfc7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed. JWTs can be signed using a secret (with the HMAC algorithm) or a public/private key pair using RSA or ECDSA.
  
bcrypt
  1. npm install bcrypt
  2. a password-hashing function designed by Niels Provos and David Mazières, based on the Blowfish cipher and presented at USENIX in 1999.[1] Besides incorporating a salt to protect against rainbow table attacks, bcrypt is an adaptive function: over time, the iteration count can be increased to make it slower, so it remains resistant to brute-force search attacks even with increasing computation power.
  3. A bcrypt hash string is of the form:  " $2b$[cost]$[22 character salt][31 character hash] "
