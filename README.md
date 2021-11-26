# Solution-for-SSH-Unable-to-Negotiate-Errors
Solution for SSH Unable to Negotiate Errors

ssh swcore  

Unable to negotiate with 192.168.2.254 port 22: no matching host key type found. Their offer: ssh-dss

vi /.ssh/config 

Host swcore

Hostname 192.168.2.254

User sgs

Ciphers aes256-cbc,aes128-ctr,aes192-ctr,aes256-ctr,aes128-cbc,3des-cbc

KexAlgorithms +diffie-hellman-group1-sha1

HostKeyAlgorithms=+ssh-dss


Link detail: https://www.infosecmatter.com/solution-for-ssh-unable-to-negotiate-errors/
