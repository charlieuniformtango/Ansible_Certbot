# Ansible_Certbot

## Certbot Instructions

To obtain a new certificate:

```
certbot certonly --dns-route53 --domain <whatever>.charlietango.com
```

Certificates are renewed automatically via cron job.

## Certificate Installation

```
ansible-playbook --vault-password-file ~/.ansible_vault_password push_certs.yml
```
