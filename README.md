CPSC 317 Assignment 3: HTTP Proxy Server
========
> A simple http proxy server with fitering

[Assignment Description](/description/CS317A3.html)

How to run it:

```bash
./proxyFilter PORT FILTER_LIST.txt
eg: ./proxyFilter 9001 filter.txt
```
Open another terminal tab:
```bash
nc -v localhost 9001
GET http://www.cs.ubc.ca/~acton/lawler.txt HTTP/1.1   (Comment: Accepted)
GET http://www.facebook.com HTTP/1.1   (Comment: Refused)
```

Or open any a browser tab:
```bash
http://localhost:9001/http://www.cs.ubc.ca/~acton/lawler.txt    (Accepted)
http://localhost:9001/http://www.facebook.com                   (Refused)
```

Other Tests: 
```bash
GET http://www.renren.com HTTP/1.1    (Refused)
GET http://www.google.com HTTP/1.1    (Accepted)
GET http://www.yahoo.ca HTTP/1.1      (Accepted)
```
