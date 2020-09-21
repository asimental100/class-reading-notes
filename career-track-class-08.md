HTTP Basics
  1. HTTP stands for Hypertext Transfer Protocol. It's a stateless, application-layer protocol for communicating between distributed systems, and is the foundation of the modern web. 
  2. HTTP allows for communication between a variety of hosts and clients, and supports a mixture of network configurations. To make this possible, it assumes very little about a particular system, and does not keep state between different message exchanges. This makes HTTP a stateless protocol. The communication usually takes place over TCP/IP, but any reliable transport can be used. The default port for TCP/IP is 80, but other ports can also be used.
  3. Communication between a host and a client occurs, via a request/response pair. The client initiates an HTTP request message, which is serviced through a HTTP response message in return.
  4. The current version of the protocol is HTTP/1.1, which adds a few extra features to the previous 1.0 version. The most important of these, in my opinion, includes persistent connections, chunked transfer-coding and fine-grained caching headers.
  5. URLs - At the heart of web communications is the request message, which are sent via Uniform Resource Locators (URLs). The protocol is typically http, but it can also be https for secure communications. The default port is 80, but one can be set explicitly.
  6. Verbs - URLs reveal the identity of the particular host with which we want to communicate, but the action that should be performed on the host is specified via HTTP verbs.
  7. Status Codes - With URLs and verbs, the client can initiate requests to the server. In return, the server responds with status codes and message payloads. The status code is important and tells the client how to interpret the server response.
    7.a. 100 codes are informational messages
    7.b. 200 codes are successful request codes
    7.c. 300 codes are redirection codes
    7.d. 400 codes are client error codes
    7.e. 500 codes are server error codes

How DNS Works
  1. DNS = Domain Name System where we remember names (words) rather than IP addresses to navigate the web.
