# VulnNet-Internal-Walkthrough

![image](https://github.com/mohsecurity254/VulnNet-Internal-Walkthrough/assets/147415543/ac445041-e1af-445e-b2cd-0256c0bd924f)

### Reconnaisance
|PORT  |   STATE   | SERVICE    | REASON      |VERSION|
|------|-----------|:------------:|-------------|-------------|
|22/tcp |  open    |ssh         |syn-ack     |OpenSSH 7.6p1 Ubuntu 4ubuntu0.3|
|111/tcp | open    |rpcbind     |syn-ack     |2-4 (RPC #100000)|
|139/tcp | open    |netbios-ssn |syn-ack     |Samba smbd 3.X - 4.X |
|445/tcp |open     |netbios-ssn |syn-ack     |Samba smbd 3.X - 4.X |
|873/tcp |open     |rsync       |syn-ack     |(protocol version 31)|
|2049/tcp|open     |nfs         |syn-ack     |3-4 (RPC #100003)|
|9090/tcp|filtered |zeus-admin  |no-response |

We have some intresting ports 
port 22,111,445,2049

Lets start with port 445 smb and see what we can find 

![image](https://github.com/mohsecurity254/VulnNet-Internal-Walkthrough/assets/147415543/408472ff-dd39-4445-a435-7174202372d8)

There are 3 shares we can further enumearate to find clues

Lets try and see if we can login without a password 

we find 2 directories

![image](https://github.com/mohsecurity254/VulnNet-Internal-Walkthrough/assets/147415543/7b483d11-6197-4d85-9373-e7762316e2d0)

after searching through the temp directory we find our first flag

![image](https://github.com/mohsecurity254/VulnNet-Internal-Walkthrough/assets/147415543/d34ef805-ba27-44d3-bf9f-7960110c6a0a)

Lets look into the other directory and see what we find 

![image](https://github.com/mohsecurity254/VulnNet-Internal-Walkthrough/assets/147415543/6f34ccbc-6852-4fbf-a2ec-809bae6825ae)

![image](https://github.com/mohsecurity254/VulnNet-Internal-Walkthrough/assets/147415543/d18add54-58b5-4b68-b86c-eaae377f8263)

We find some intresting info about a document, lets check out the other ports to see if we can find that document 





