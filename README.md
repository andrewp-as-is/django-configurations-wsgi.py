<!--
https://readme42.com
-->


[![](https://img.shields.io/pypi/v/django-configurations-wsgi.svg?maxAge=3600)](https://pypi.org/project/django-configurations-wsgi/)
[![](https://img.shields.io/badge/License-Unlicense-blue.svg?longCache=True)](https://unlicense.org/)
[![](https://github.com/andrewp-as-is/django-configurations-wsgi.py/workflows/tests42/badge.svg)](https://github.com/andrewp-as-is/django-configurations-wsgi.py/actions)

### Installation
```bash
$ [sudo] pip install django-configurations-wsgi
```

#### Examples
```bash
gunicorn django_configurations_wsgi:application -b 0.0.0.0:8080
```

`requirements.txt`
```
...
django_configurations_wsgi
...
```

P.S. default `wsgi.py`:
```python
import os

os.environ.setdefault('DJANGO_SETTINGS_MODULE', 'settings')
os.environ.setdefault('DJANGO_CONFIGURATION', 'Dev')

from configurations.wsgi import get_wsgi_application

application = get_wsgi_application()
```

#### Links
+   [django-configurations](https://github.com/jazzband/django-configurations)

<p align="center">
    <a href="https://readme42.com/">readme42.com</a>
</p>
