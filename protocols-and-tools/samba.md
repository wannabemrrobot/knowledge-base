---
description: A brief overview on Samba networking protocol.
---

# Samba

Samba is an extremely useful networking tool, especially for whom who has both Unix and Windows systems on his network.

Samba running on the Unix systems, can allow Windows to access, the shares such as files and printers on the Unix systems and when running on Windows machines, it can enable Unix systems to access resources shared by the Windows.

## What is Samba?

Samba is a suite of Unix applications that speaks SMB\(Server Message Block\) protocol. [more on SMB protocol](SMB.md)

It might seem natural to use Windows server to serve files and printers to a network containing only Windows clients, but there are good reasons for using Samba server in such cases.

As Samba is a suite of Unix applications, which is reliable resulting in a lower maintenance cost. In some scenarios, Samba even outperforms Windows 2000 Server by a factor of 2 to 1 on identical PC hardware, according to some third-party benchmarks.
Most of all, Samba is free! Ever wondered, how softwares like VMware enables sharing of files, between host and VMs? It's on Samba.
The Samba suite also includes client tools that allow users on a Unix system to access folders and printers that Windows systems and Samba servers offer on the network.

## Services offered by the Samba:

- Share one or more directory trees
- Share one or more Distributed File System(DFS) trees
- Share printers installed in the server among Windows clients
- Assist clients in [network browsing](https://web.mit.edu/rhel-doc/5/RHEL-5-manual/Deployment_Guide-en-US/s1-samba-network-browsing.html)
- Authenticate clients logging onto a Windows domain
- Provide or assist with Windows Internet Name Service(WINS) Name-Server resolution.

## Samba Daemons:
Samba suite revolves around a pair of Unix daemons, which provide shared resources called `shares` or `services` to the SMB clients on the network.

They are:
- smbd
  - A daemon that handles file and printer sharing and provides authentication and authorization for SMB clients.
- nmbd
  - A daemon that supports NetBIOS Name Service and WINS, which is Microsoft's implementation of a NetBIOS Name Server (NBNS). It also assists with network browsing.