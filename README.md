

# Getting Started
This README is a step by step setup guide for PGAdmin + Nginx. Applicable only for Ubuntu/Debian OS.

## Step 1: Clone repository
* Clone repository <br /> **git clone https://github.com/boringproject/Eric-Schwantler-PGAdmin-Nginx.git `<folder>`**

<br/>

## Step 2: Supply Credentials
<br/>

Copy `.env.example` to `.env` and supply the following environment variable.

* **PGADMIN_DEFAULT_EMAIL**=`hello@example.com`
* **PGADMIN_DEFAULT_PASSWORD**=`notsupersecret`

<br/>

## Step 3: Docker Installation
<br/>

* In your terminal run `./install-docker.sh`
* Follow instructions in the terminal.
<br/>

## Step 4: Initialize Certificate
<br/>

* In your terminal run `./init-certificate.sh`
* Supply details in the terminal.
<br/>

## Step 5: Running
<br/>

* In your terminal run `./start.sh`
* Then wait for a few seconds to boot up
* Try visit in the browser using IP https://<`IP Address`>

<br/>
<br/>

# Renew Certificate

* In your terminal run `./renew-certificate.sh`
* Wait for a few seconds to take effect.
* Check issued certificate in browser to confirm.

<br/>

# Software Update

* In your terminal run `./software-update.sh`

<br/>

# Notes/Reminder

Due to nature of IP address host you will notice something like this

because the certificate issued is self-signed it cater medium security that is usually used for internal communication and test environment . See comment thread here `https://www.digitalocean.com/community/questions/ssl-for-ip-address`. Alternative solution is to host the site using domain name.
<br />

SSL Certificate References:
* https://www.digitalocean.com/community/questions/ssl-for-ip-address
* https://www.keyfactor.com/blog/self-signed-certificate-risks/

