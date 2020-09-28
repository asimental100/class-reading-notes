Why you should use BCrypt to hash passwords
  1. Using a Key Factor, BCrypt is able to adjust the cost of hashing. With Key Factor changes, the hash output can be influenced. In this way, BCrypt remains extremely resistant to hacks, especially a type of password cracking called rainbow table.

Hashing in Action: Understanding bcrypt
  1. npm install bcrypt
  2. A better way to store passwords is to add a salt to the hashing process: adding additional random data to the input of a hashing function that makes each password hash unique. The ideal authentication platform would integrate these two processes, hashing and salting, seamlessly.
  3. bcrypt was designed by Niels Provos and David Mazières based on the Blowfish cipher: b for Blowfish and crypt for the name of the hashing function used by the UNIX password system.
  4. bcrypt runs in two phases:
    4.1. A function called EksBlowfishSetup is setup using the desired cost, the salt, and the password to initialize the state of eksblowfish. Then, bcrypt spends a lot of time running an expensive key schedule which consists of performing a key derivation where we derive a set of subkeys from a primary key. Here, the password is used as the primary key. In case that the user selected a bad or short password, we stretch that password/key into a longer password/key. The aforementioned practice is also known as key stretching. What we are going through this first phase is to promote key strengthening to slow down calculations which in turn also slow down attackers.
    4.2. The magic value is the 192-bit value OrpheanBeholderScryDoubt. This value is encrypted 64 times using eksblowfish in ECB mode with the state from the previous phase. The output of this phase is the cost and the 128-bit salt value concatenated with the result of the encryption loop.
  5. bcrypt gives us access to a Node.js library that has utility methods to facilitate the hashing process. saltRounds represent the cost or work factor.

Token Storage
  1. Securing SPAs that make API calls come with their own set of concerns. You'll need to ensure that tokens and other sensitive data are not vulnerable to cross-site scripting (XSS) and can't be read by malicious JavaScript.
  2. To reduce security risks if your SPA is using implicit (we recommend using authorization code flow with PKCE instead) or hybrid flows, you can reduce the absolute token expiration time. This reduces the impact of a reflected XSS attack (but not of a persistent one).
  
