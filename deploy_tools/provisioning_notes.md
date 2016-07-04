Provisioning a new site
=======================

## Required packages:

* nginx
* Python 3
* Git
* pip
* virtualenv

## Nginx Virtual Host config

* see nginx.template.conf
* replace SITENAME with, eg, staging.my-domain.com

## Systemd service

* see gunicorn.template.service
* replace SITENAME with, eg, staging.my-domain.com

## Folder structure:
Assume we have user account at /home/username
```
/home/username<br/>
└── sites<br/>
    └── SITENAME
        ├── database
        ├── source
        ├── static
        └── virtualenv
```