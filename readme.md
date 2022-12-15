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

```
# Create virtual Environment
# install requirements
$ cd backend
# activate virtual environment
$ python manage.py tailwind init
$ python manage.py tailwind install

# For running tailwind dev server
$ python manage.py tailwind start

```

## For Live Reload

```
{% load livereload_tags %}
...
{% livereload_script %}
</head>
```