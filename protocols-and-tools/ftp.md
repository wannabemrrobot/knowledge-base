---
description: A brief overview on File Transfer Protocol.
---

# File Transfer Protocol

## Overview
File Transfer Protocol is a network protocol, used to send files from one computer to another computer via TCP/IP connections. 
It runs on port 21.

Within the `TCP/IP suite`, this FTP protocol is considered as an `application layer protocol`.

This protocol runs on the basis of `Client-Server` architecture, where one computer serves as an server and other as a client. These two computers can share the file providing that they have internet connection. 

In the FTP transaction, the end user computer is often referred as `localhost` and the other computer involved is called as `remote host`. Both computers need to be properly configured and connected via network to transfer files via FTP.

Servers must be setup to run FTP services and a FTP software client is needed at the client end access those services.
For example, in Microsoft Windows, the user's own computer can be setup as a FTP server using the `Internet Information Services Manager.`

## File access via FTP
Now, there are a couple of ways for accessing the files via FTP.

- FTP client softwares such as *FileZilla*
- Browsers - access files with url *ftp.serverIP*

## Anonymous Login
Some of the FTP Server configurations allows for an anonymous login, meaning the user who wants to access FTP services can access them without a username or password in some cases, or with the username `anonymous` or `ftp` with anything as the password.

Most of the public online downloading sites, have a FTP user called `anonymous` to allow everyone access to the site's resources without identifying themselves.

## Security
FTP was **not built to be secure**. FTP does not use **encryption**. For authentication, it relies on **cleartext usernames and passwords**, making data transmissions sent over FTP **vulnerable** to ordinary methods of eavesdropping, impersonation and other attacks.

## SFTP
SFTP stands for **Secure File Transfer Protocol**. SFTP is same as FTP, except it does transfers in an encrypted format using the secure shell. Thus, it adds an extra layer of security, making everything like authentication and file transfers in an encrypted way.

Both the FTP and SFTP are connection-oriented protocols that use TCP for file transfers. Thus, file delivery is guaranteed.

## TFTP
TFTP stands for **Trivial File Transfer Protocol**. Unlike FTP and SFTP, TFTP is not used over the internet to transfer files. It is used over the local network. It also uses UDP instead of TCP for file transfer, which is connection-less making it a non-reliable protocol. It also lacks security during the transfer and not that it needs that, cause it only used in local networks for file transfers.

## FTP Today
Although many file transfers can be conducted via HTTP(Hyper Text Transfer Protocol), FTP is still commonly used to transfer files behind the scenes in many applications such as banking services. Sometimes it can also be used to download softwares in the browsers.