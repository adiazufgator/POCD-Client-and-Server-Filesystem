# POCD-Client-and-Server-Filesystem

A client-server design that was implemented in order to develop a fault tolerant 
networking system. The core of the design was implementing a client 
in python programming language to interface with four servers that 
serve as a single storage unit from the perspective of the client. The 
design approach taken is similar to RAID1 where redundancy is 
used. This particular design uses a redundancy factor of two. If one 
of the servers go down, the client is able to fetch the data from 
another server. The overall design emulates a linux file system where 
the client provides an interactive window to the user with the 
capabilities to do the following file system commands: mkdir, create, 
mv, read, write, status, rm