# Ex-01-Simple-Web-Server
## Date:

## AIM:
To develop a simple webserver to serve html pages.

## DESIGN STEPS:
### Step 1: 
HTML content creation.

### Step 2:
Design of webserver workflow.

### Step 3:
Implementation using Python code.

### Step 4:
Serving the HTML pages.

### Step 5:
Testing the webserver.

## PROGRAM:
```
from http.server import HTTPServer, BaseHTTPRequestHandler

content="""
<html>
<head>
</head>
<body>
<h1>Welcome</h1>
</body>
</html>
"""
class HelloHandler (BaseHTTPRequestHandler):
    def do_GET(self):


        self.send  (200)
        self.send_header('content-type', 'text/html; charset=utf-8')
        self.end_headers()
        self.wfile.write(content.encode())
```

## OUTPUT:
![Alt text](<web output-1.png>)


## RESULT:
The program for implementing simple webserver is executed successfully.
