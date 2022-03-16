FROM python:3.9

RUN pip install \
    Django>=4.0 \
    ipdb==0.13.9 \
    opentelemetry-api>=1.3.0 \
    opentelemetry-instrumentation>=0.25b0 \
    opentelemetry-sdk>=1.3.0 \
    requests

# install applicable auto-instrumentation libraries
RUN opentelemetry-bootstrap --action=install
