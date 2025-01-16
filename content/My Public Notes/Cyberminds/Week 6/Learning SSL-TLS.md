
Source: [SSL/TLS and PKI History](https://www.feistyduck.com/ssl-tls-and-pki-history/)

>[!important] SSL/TLS is prevalent in every digital communication

**Root of Trust**: list of certificates that your browser *thinks* are valid or trustworthy
Certificates can grant "authentication" but always based on the Root of Trust (the root CA may be fake or the root CA may trust malicious Intermediate CA)

```mermaid
sequenceDiagram
Client->>Server: Client_hello
Server->>Client: Server_hello
```
**Client_hello**: includes supported cipher suites
**Server_hello**: includes chosen cipher suite
➡No crypto at this point : makes it possible the **Dumbing down attack** (choose less secure cipher suite in order to eavesdrop the communication)
*Cipher suite*: key exchange method and cipher spec

>[!info] New protocols encrypt and sign the client_hello to ensure authentication


```mermaid
sequenceDiagram
Server->>Client: certificate
Server->>Client: server_key_exchange
Client-->>Server: certificate_request
Server->>Client: server_hello_done
```

```mermaid
sequenceDiagram
Client-->>Server: certificate
Client->>Server: client_key_exchange
Client-->>Server: certificate_verify
```
```mermaid
sequenceDiagram
Client->>Server: change_cipher_spec
Client->>Server: finished
Server->>Client: change_cipher_spec
Server->>Client: finished
```
Keys are changed every few minutes

**The RoT is established by the browser** (Look in Certification Manager) - follows a Oligarchic model