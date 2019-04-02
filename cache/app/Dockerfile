FROM python:3.8.0a3-alpine3.9

RUN mkdir -p /app
COPY index.html /app/index.html
RUN pip install simple-http-server

WORKDIR /app
EXPOSE 5000

ENTRYPOINT [ "python", "-m", "http.server", "5000" ]
