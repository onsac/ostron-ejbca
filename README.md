# ostron-ejbca
Setup EJBCA Docker

## Install-EJBCA

Manual de instalação do EJBCA

```sh

sudo yum check-update

```
```sh

curl -fsSL https://get.docker.com/ | sh

```
```sh

sudo systemctl start docker

```
```sh
sudo systemctl status docker

```
```sh

docker.service - Docker Application Container Engine
   Loaded: loaded (/lib/systemd/system/docker.service; enabled; vendor preset: enabled)
   Active: active (running) since Sun 2016-05-01 06:53:52 CDT; 1 weeks 3 days ago
     Docs: https://docs.docker.com
 Main PID: 749 (docker)
 
```
```sh

sudo systemctl enable docker

```
```sh

sudo docker pull primekey/ejbca-ce

```
```sh

sudo docker run -it -d --rm -p 80:8080 -p 443:8443 -h ejbca.ostron.com -e TLS_SETUP_ENABLED="simple" primekey/ejbca-ce

```
```sh

C:\windows\system32\drivers\etc\hosts
192.168.10.9    ejbca.ostron.com

```
```sh

https://ejbca.ostron.com/ejbca/adminweb/

```






 
 
 
