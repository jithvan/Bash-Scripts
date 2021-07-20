# Bash Scripts

The following sections will detail requirements for the usage of the scripts in this repository.

## SSL Reverse Proxy
Install NGINX
```bash
sudo apt update
sudo apt-get -y install nginx
```
Add Certbot PPA
```bash
sudo apt-get install software-properties-common
sudo add-apt-repository universe
sudo add-apt-repository ppa:certbot/certbot
sudo apt-get update
```
Install Certbot
```bash
sudo apt-get -y install certbot python3-certbot-nginx
```
Download and run proxy script

```bash
wget https://raw.githubusercontent.com/jithvan/Bash-Scripts/master/reverse_proxy.sh && bash reverse_proxy.sh
```
Reload NGINX
```bash
sudo service nginx reload
```