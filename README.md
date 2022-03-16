# otel-python-duplicate-request-spans

## Prerequisites

* docker
* docker-compose

## Run and Trigger Trace

To build `django-app-a-ot`:
```
docker-compose build
```

To run `django-app-a-ot` on http://0.0.0.0:8008:

```
PYTHON_DEBUG_LEVEL=DEBUG docker-compose up
```
where `PYTHON_DEBUG_LEVEL` can be one of: `DEBUG`, `INFO`, `WARNING`, `ERROR`, `CRITICAL`.

To trigger trace output to console:

```
curl -v http://0.0.0.0:8008/home_a/
```