# HAPROXY WITH TLS1.3, HTTP/2

### Spin up HAPROXY backends

- docker run -p 2222:9999 -d -e APPID=2222 mavewrick1/haproxy:v1.0
- docker run -p 3333:9999 -d -e APPID=3333 mavewrick1/haproxy:v1.0
- docker run -p 4444:9999 -d -e APPID=4444 mavewrick1/haproxy:v1.0
- docker run -p 5555:9999 -d -e APPID=5555 mavewrick1/haproxy:v1.0

### HAPROXY

- Install haproxy
- mkdir proxy; cd proxy
- vim test.cfg
- haproxy -f [cfg-filename]
- (Visit port :80) By default, haproxy runs on TCP mode/ as a layer 4 proxy; the browser would create a stateful TCP connection with one of the servers. Once one is established, on page refresh, subsequent requests would become sticky to that server and forwarding to other servers would not be possible.
