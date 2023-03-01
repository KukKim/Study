## 1. Internet  
# 1-2. What is HTTP?  
The HTTP(Hyper Text Transfer Protocol) is the foundation of the World wide web.

## The HTTP Request Circle  
A typical HTTP request/response circle:
1. The browser requests an HTML page. The server returns an HTML file.
2. The browser requests a style sheet. The server returns a CSS file.
3. The browser requests an JPG image. The server returns a JPG file.
4. The browser requests Javascript code. The server returns a JS file.
5. The browser requests data. The server returns data (in XML or JSON).

## HTTP request looks like...
A typical HTTP request contains...  
1. HTTTP version type
2. a URL
3. an HTTTP methtod
4. HTTP request headers
5. optional HTTP body

- What is an HTTP method?  
HTTP method refers to the purpose of sending a request when the client sends a request to the server. The HTTP method includes GET, POST, and so on.
- What are HTTP request headers?  
The HTTP request header has multiple pairs of HTTP information in key/value form. The HTTP request header looks like the following image.
![HTTPRequestHeader](https://www.cloudflare.com/img/learning/ddos/glossary/hypertext-transfer-protocol-http/http-request-headers.png)
<!-- - What is in an HTTP request body?  -->

## HTTP response looks like...
The server sends an HTTP response to the client in response to the HTTT request. A typical HTTP response contains...
1. an HTTP status code
2. HTTP response headers
3. optional HTTP body

- What's an HTTP status code?
The HTTP status code lets you know the result of HTTP requests being processed by the server. The HTTP status code can be found through the following link.  
[HTTP status code](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status)
- What are HTTP response headers?  
HTTP response has a header, just like HTTP requests. The HTTP response header looks like the following image.
![HTTPResponseHeader](https://www.cloudflare.com/img/learning/ddos/glossary/hypertext-transfer-protocol-http/http-response-headers.png)

## XHR - XML Http Request
All browsers have a build-in XML HTTP request object(XHR).


***
#### Keywords
- WWW
- HTML
- CSS
- Javascript
- XHR
- XML

#### Reference
- https://www.w3schools.com/whatis/whatis_http.asp
- https://developer.mozilla.org/ko/docs/Web/HTTP/Overview
- https://www.cloudflare.com/en-gb/learning/ddos/glossary/hypertext-transfer-protocol-http/
- https://developer.mozilla.org/en-US/docs/Web/HTTP/Status