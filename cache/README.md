
# Set up Nginx Cache for a simple http web server

docker volume create --name=cache

docker-compose up

## Result

hit the url

$ curl -v http://localhost

Cache status MISS or HIT

```log
proxy_1  | ip=172.23.0.1 user=- req="GET / HTTP/1.1" status=200 bytes_sent=28 req_time=0.003 ref="-" ua=" curl/7.54.0" forwarded="-" cache_status=MISS transaction_id="-" request_id="-" upstream_response_time=0.000
proxy_1  | ip=172.23.0.1 user=- req="GET / HTTP/1.1" status=200 bytes_sent=28 req_time=0.000 ref="-" ua=" curl/7.54.0" forwarded="-" cache_status=HIT transaction_id="-" request_id="-" upstream_response_time=-
```

## Guide

[Nginx Caching Guide](https://www.nginx.com/blog/nginx-caching-guide/)