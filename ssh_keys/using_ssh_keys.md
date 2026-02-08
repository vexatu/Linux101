# SSH Keys
Using ssh keys for Secure Shell (SSH) conncection can benifit the user in protecting his own home server or public server from different attackers. Using ssh key it is a safer and easier method to log in multiple servers or one server based on challange-response authentication.

## General Information
When generating a set of keys, the output will be a public key that can be shared with the server and a private key that should be kept safe. 
This is working based on challange-response authentification protocol, the most used protocol like this is passowrd authentification when the user is promted for a passowrd in order to acces the content or to log in.
The downside of using a password authentificcation is that when devices are connected on public networks or unsecure networks in general the password can be intercepted by diffrent attackers using different hacking methods.

**_Working principle_**

When using ssh keys you will recieve two types of keys the private one and the public one imagine having one Linux machine as principal and a remote Linux machine as secondary. On the host_machine you will keep the private key that you will not share with anyone, the public key must be shared with the remote_host you are trying to connect via SSH.
After sharing the public key the remote_host will generate a puzzle for the host_machine, the host_machine based on the private key will solve the puzzle and connect with the remote_host without promting the user for a passowrd.
What makes this connection secure is that the challange sent by the remote_host can be understood only by the key holder for that type of challange and only the key holder will be able to generate a response for the challange.

## Practice

1. Installing dependecies

   In order to connect via SSH it is needed to install the openssh client.

> sudo apt install openssh-client

   After installing the client, to check if the ssh server is running can be done with the following command:

> systemctl status ssh

   After executing the command the systems comes up with this error: 
   
   **_Unit ssh.service could not be found._**

   To solve the issue we need to install also the openssh-server with this command: 
   
   > sudo apt install openssh-server 
   
   Running this command not only will install the package but also will start the ssh server, so for safety reasons try to do this on a personal local network to not be prone to attackers.
   

   
