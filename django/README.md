# run it

```bash
docker-compose run web django-admin startproject demo .
```
This will build the project

```python
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql',
        'NAME': 'postgres',
        'USER': 'postgres',
        'HOST': 'db',
        'PORT': 5432,
    }
}
```

Run it

```bash
docker-compose up
```
