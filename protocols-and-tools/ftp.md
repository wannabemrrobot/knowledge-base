---
description: A brief overview on File Transfer Protocol.
---

# File Transfer Protocol

File Transfer Protocol is a network protocol, used to send files from one computer to another computer via TCP/IP connections. 

Within the `TCP/IP suite`, this FTP protocol is considered as an `application layer protocol`.

This protocol runs on the basis of `Client-Server` architecture, where one computer serves as an server and other as a client. These two computers can share the file providing that they have internet connection. 

In the FTP transaction, the end user computer is often referred as `localhost` and the other computer involved is called as `remote host`. Both computers need to be properly configured and connected via network to transfer files via FTP.

Servers must be setup to run FTP services and a FTP software client is needed at the client end access those services.

## Current State of FTP:
Although many file transfers can be conducted via HTTP(Hyper Text Transfer Protocol), FTP is still commonly used to transfer files behind the scenes in many applications such as banking services. Sometimes it can also be used to download softwares in the browsers.

## Security:
FTP does not use encryption. For authentication, it relies on cleartext usernames and passwords, making data transmissions sent over FTP vulnerable to ordinary methods of eavesdropping, impersonation and other attacks.