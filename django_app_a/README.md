# Django App (Automatically Instrumented)

This app is a very simple Django app which generates OpenTelemetry data by using the OTel auto-instrumentation.

For ease of use, this directory provides a Dockerfile which has all dependencies needed pre-installed.

## Django Instrumentation

### Auto Instrumentation

Run the django app with ``opentelemetry-instrument python manage.py runserver 0.0.0.0:8008 --noreload`` which will automatically instruments the app using OpenTelemetry.
