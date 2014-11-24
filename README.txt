How to run it:

./proxyFilter 9001
The server is starting…
(For now just ignore the filter file)

Open another terminal:
nc -v localhost 9001
GET http://www.cs.ubc.ca/~acton/lawler.txt HTTP/1.1   (Comment: Accepted)
GET http://www.facebook.com HTTP/1.1   (Comment: Refused)

Or open any a browser tab:
http://localhost:9001/http://www.cs.ubc.ca/~acton/lawler.txt    (Accepted)
http://localhost:9001/http://www.facebook.com                        (Refused)

Still need to know the format of the filter file in order to read and import.
Multi-thread need to be implemented.

GET http://www.renren.com HTTP/1.1
GET http://www.google.com HTTP/1.1
GET http://www.yahoo.ca HTTP/1.1