# Custom Certificates

Place the certificates here, you can use a automated routine to create the files
using [ACME CertBot](https://certbot.eff.org/). 


This playbook will use three files, I'll use the domain `example.com` for this
certificate.

- Certificate:
    `example.com.crt`
- Certificate and Chain:
    `example.com-fullchain.crt`
- Certificate Key:
    `example.com.key`

This certificate needs to be a Wildcard Certificate so all subdomains of this
proxy will have a valid certificate
