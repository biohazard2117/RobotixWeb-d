# Steps
### First generate certificate
#### Using *nginx-proxy.conf*
#### Using *dhparam* at _dhparam/dhparam-2048.pem_
```
openssl dhparam -out dhparam-2048.pem 2048
```
#### Than switch to *nginx-proxy-ssl.conf*