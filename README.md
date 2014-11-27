CPSC 317 Assignment 3: HTTP Proxy Server

How to run it:

./proxyFilter 9001 filter.txt

Open another terminal:
nc -v localhost 9001
GET http://www.cs.ubc.ca/~acton/lawler.txt HTTP/1.1   (Comment: Accepted)
GET http://www.facebook.com HTTP/1.1   (Comment: Refused)

Or open any a browser tab:
http://localhost:9001/http://www.cs.ubc.ca/~acton/lawler.txt    (Accepted)
http://localhost:9001/http://www.facebook.com                   (Refused)

Other Tests: 
GET http://www.renren.com HTTP/1.1
GET http://www.google.com HTTP/1.1
GET http://www.yahoo.ca HTTP/1.1
