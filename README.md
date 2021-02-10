# HAPROXY WITH TLS1.3, HTTP/2

### Spin up HAPROXY backends

- docker run -p 2222:9999 -d -e APPID=2222 mavewrick1/haproxy:v1.0
- docker run -p 3333:9999 -d -e APPID=3333 mavewrick1/haproxy:v1.0
- docker run -p 4444:9999 -d -e APPID=4444 mavewrick1/haproxy:v1.0
- docker run -p 5555:9999 -d -e APPID=5555 mavewrick1/haproxy:v1.0
