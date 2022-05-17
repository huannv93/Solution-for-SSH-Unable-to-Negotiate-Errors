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



////// loi SSH 

<img width="857" alt="image" src="https://user-images.githubusercontent.com/64687828/168730448-93fffa14-90b1-4a59-be7d-044c7b4b601e.png">


**sulotion** : ssh-keygen -f "/Users/huannv/.ssh/known_hosts" -R "113.160.222.222"   /// "113.160.222.222"  ip server linux
