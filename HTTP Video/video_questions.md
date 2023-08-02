1. What are the required components of an HTTP request? What are the additional optional components?

My answer:

The required components of the HTTP request are the path (resource name, query parameters), the HTTP method, the headers and message body.

LS answer:

The HTTP method and the path are required, and form part of what is known as the start-line or request-line. As of HTTP 1.0, the HTTP version also forms part of the request-line. The Host header is a required component since HTTP 1.1. Parameters, all other headers, and message body are optional.

Technically speaking the 'path' portion of the request-line is known as the 'request-URI', and incorporates the actual path to the resource and the optional parameters if present. In practice, most people simply refer to this part of the request-line as the 'path'.

2. What are the required components of the HTTP response? What are the additional optional components?

My answer:

The required component of an HTTP response is the Status code. The Status code is a three-digit number sent back by the server that signifies that status of the request.

The optional components are the headers and body. Headers contain metadata about the data being sent back, and the body contains the raw response data.

LS answer:

A status line with a status code is required. Headers and body are optional.

3. What determines whether a request should use GET or POST as its HTTP method?

My answer:

The action in which we are attempting to perform will determine which method our request will use. If we are trying to retrieve data or files from the server, then a GET request will be used. If we are attempting to perform some sort of action on the server, such as uploading files or submitting data to the server, then the POST method will be used.

LS answer:

GET requests should only retrieve content from the server. They can generally be thought of as "read only" operations, however, there are some subtle exceptions to this rule. For example, consider a webpage that tracks how many times it is viewed. GET is still appropriate since the main content of the page doesn't change.

POST requests involve changing values that are stored on the server. Most HTML forms that submit their values to the server will use POST. Search forms are a noticeable exception to this rule: they often use GET since they are not changing any data on the server, only viewing it.