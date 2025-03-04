# SSH

You can continue from the diagram you created in the configuration repository  
```
enable
configure terminal
ip domain-name example.com
crypto key generate rsa general-keys modulus 1024
username Noro secret black
line vty 0 15
login local
transport input ssh
exit
exit
copy running-config startup-config
```





### Test Telnet

```
C:\>telnet 192.168.1.33
Trying 192.168.1.33 ...Open

[Connection to 192.168.1.33 closed by foreign host]
```
### Test SSH
```
C:\>ssh -l Noro 192.168.1.33

Password: 
SW1>
```