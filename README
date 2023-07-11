# Ansible Playbook to Configure NGINX as a Reverse Proxy

## Table of Contents
**[Intro](#intro)**  
**[Using This PlayBook](#using-this-playbook)**  
**[Using Custom Certificates](#using-custom-certificates)**  
**[License](#license)**  
**[Author](#author)**  

## Intro
This playbook was created to help me manage my homelab, I use Nginx as reverse
proxy for all applications running in Docker and Virtual Machines.

### Sequence Diagram for Reference
```mermaid
sequenceDiagram
    participant Client
    participant Nginx Proxy
    participant App1
    participant App2
    Client->>Nginx Proxy: Access App1.proxy/
    Nginx Proxy->>App1: Forward to app at PROTO://HOST:PORT/
    App1->>Nginx Proxy: Response from App1
    Nginx Proxy->>Client: Response from App1
    
    Client->>Nginx Proxy: Access App2.proxy/
    Nginx Proxy->>App2: Forward to app at PROTO://HOST:PORT/
    App2->>Nginx Proxy: Response from App2
    Nginx Proxy->>Client: Response from App2
```

## Using This Playbook
This code was developed and tested on a Raspberry Pi 3/4 using Raspberry Pi OS
Lite as starting point.

You can use the [How to use Raspberry Pi Imager](https://youtu.be/ntaXWS8Lk34)
quick video to help you getting the OS installed. For mor information check this
page [Raspberry Pi OS](https://www.raspberrypi.com/software/).

### Video
[![How to use Raspberry Pi Imager](https://img.youtube.com/vi/ntaXWS8Lk34/0.jpg)](https://www.youtube.com/watch?v=ntaXWS8Lk34)

### Custom Options
The `example.config.yml` has all available options you can create a `config.yml`
with your custom options and configuration. The file `inventory.ini` contains 
the example of a host using a domain name, you will need to fill in all of your
own hosts.

### The `.gitignore`
The following files **are not tracked** so be carefull and make a backup of your
configurations.

- `files/*.crt`
- `files/*.pem`
- `config.yml`
- `inventory.ini`

## Using Custom Certificates
If you have a valid certificate for your domain you can use it using the info in
this page [Custom Certificates](files/README)

## License
MIT

## Author
Created by [@hebertluiz](https://github.com/hebertluiz) | [My Page](https://site.hev.dev.br/) | 2023



