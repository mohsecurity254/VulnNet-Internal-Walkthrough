# VulnNet-Internal-Walkthrough

![image](https://github.com/mohsecurity254/VulnNet-Internal-Walkthrough/assets/147415543/ac445041-e1af-445e-b2cd-0256c0bd924f)

### Reconnaisance
|PORT  |   STATE    SERVICE     REASON      VERSION
|------|-----------|
|22/tcp |  open     |ssh         |syn-ack     |OpenSSH 7.6p1 Ubuntu 4ubuntu0.3 |(Ubuntu Linux; protocol 2.0)|
|111/tcp | open     |rpcbind     |syn-ack     |2-4 (RPC #100000)|
|139/tcp | open     |netbios-ssn |syn-ack     |Samba smbd 3.X - 4.X (workgroup: WORKGROUP)|
|445/tcp  |open     |netbios-ssn |syn-ack     |Samba smbd 3.X - 4.X (workgroup: WORKGROUP)|
|873/tcp  |open     |rsync       |syn-ack     |(protocol version 31)|
|2049/tcp |open     |nfs         |syn-ack     |3-4 (RPC #100003)|
|9090/tcp |filtered |zeus-admin  |no-response |

