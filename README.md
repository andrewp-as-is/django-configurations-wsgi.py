<!--
https://pypi.org/project/readme-generator/
https://pypi.org/project/python-readme-generator/
-->

[![](https://img.shields.io/badge/language-Python-blue.svg?longCache=True)]()
[![](https://img.shields.io/pypi/v/django-configurations-wsgi.svg?maxAge=3600)](https://pypi.org/project/django-configurations-wsgi/)
[![](https://img.shields.io/badge/License-Unlicense-blue.svg?longCache=True)](https://unlicense.org/)
[![Travis](https://api.travis-ci.org/andrewp-as-is/django-configurations-wsgi.py.svg?branch=master)](https://travis-ci.org/andrewp-as-is/django-configurations-wsgi.py/)

#### Installation
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

if __name__ == "__main__":
    os.environ.setdefault('DJANGO_SETTINGS_MODULE', 'settings')
    os.environ.setdefault('DJANGO_CONFIGURATION', 'Dev')

    from configurations.wsgi import get_wsgi_application

    application = get_wsgi_application()

```

#### Links
+   [django-configurations](https://github.com/jazzband/django-configurations)

<p align="center">
    <a href="https://pypi.org/project/python-readme-generator/">python-readme-generator</a>
</p>