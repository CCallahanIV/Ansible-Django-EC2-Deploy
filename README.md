# Ansible-Django-EC2-Deploy

This repo contains a playbook and templates for deploying a django application on an EC2 instance with RDS database.  It utilizes a gunicorn proxy to serve to an nginx server.

The correct file structure for using this repo is as follows:

```
.
├── hosts
├── playbooks
│   ├── playbook-django-imager.retry
│   └── playbook-django-imager.yml
├── templates
│   ├── nginx_config.jinja2
│   └── upstart_config.jinja2
└── vars
    └── vars.yml
```

The vars.yml file (not included in this repo) should include all app-specific and environment variables.
