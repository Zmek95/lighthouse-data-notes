### JSON
* textual description of python (javascript actually) objects
* arrays and dictionaries

```
{
'library': [
           {'title': 'For Whom the Bell Tolls', 'author': 'Ernest Hemingway'},
           {'title': 'Trump: The Art of the Deal', 'author': 'Good Question'}
           ]
}
```

### XML   
• hierarchical description of tagged data  

```
<library>
<book>
<title>
For Whom the Bell Tolls
</title>
<author>
Ernest Hemingway
</author>
</book>
<book>
<title>
Trump: The Art of the Deal
</title>
<author>
Good Question
</author>
</book>
</library>
```

### Getting JSON Data

We need to select the output format using API:
* e.g., http header: accept = application/json


View in browser or Postman
* good for exploration / debugging

Use request .get
* this returns a python array or dictionary

Get a string and parse
* import json
* x = json .loads(aJSONString)

## HTTP Requests
- Hypertext Transfer Protocol

- When you access a website (through an URL), you are:
    - "sending a HTTP GET request to the server to retrieve data"
    - "data" can be a webpage that is displayed, it can be JSON
- When you access a website, you know it worked if it loaded
    - Status codes are helpful when you're working with code

- Common HTTP status codes:
    - 200 OK
    - 400 Bad Request
    - 401 Unauthorized
    - 404 Not Found

### The Anatomy Of A Request

It’s important to know that a request is made up of four things:

1. The endpoint

2. The method

3. The headers

4. The data (or body)

1. The endpoint (or route) is the url you request for

root-endpoint/?

https://api.github.com

2. The Method is the type of request you send to the server. You can choose from these types below:

a. GET - Used to get resource from server

b. POST - Used to create new resource on server

c. PUT/PATCH - update resource on server

d. DELETE - delete a resource on the server

