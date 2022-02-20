# Backend Template with Django and devops

## Included Frameworks
- Django
- Tailwind CSS
- Django Live Reload


## Devops
- Prometheus
- Cadvisor
- Nginx
- Certbot

## Before Running

Edit SERVER_NAME variable inside `deployment/nginx/app.conf` and `./init-letsencrypt.sh`

## For Live Reload

```
{% load livereload_tags %}
...
{% livereload_script %}
</head>
```