## Introduction
---
- Focus: Running a Heartbleed attack.
- Assumption: Running on VMs created in week 1.

## Setup
### Installing Necessary Packages
---
- Command: `sudo apt install libpcre3-dev zlib1g-dev`.

### Setting Up Vulnerable OpenSSL
---
- Download OpenSSL 1.0.1f: `wget https://www.openssl.org/source/openssl-1.0.1f.tar.gz`.
- Unpack it: `tar xvf openssl-1.0.1f.tar.gz`.

### Configuring Web Server (nginx)
---
- Download nginx: Commands involve variables and downloading specific versions.
- Build process: Includes configuring with OpenSSL and compiling.

### SSL Certificate Preparation
---
- Creating RSA key pair and self-signed certificate.
- Modifying nginx configuration for SSL.

## Running the Server
---
- Steps to start the nginx server with vulnerable OpenSSL.

## Attacking the Server
---
- Python script overview for executing the Heartbleed attack.
- Details on modifying the script for the target IP and executing it.

