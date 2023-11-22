# Ex-01-Simple-Web-Server
## Date: 21/11/23
## name: prem.R

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
![web output](https://github.com/PREM3112/ODD2023-WT-Ex-01-Simple-Web-Server/assets/145449383/e7322458-a0cd-4575-a9e1-a3bd9a4aa8a1)



## RESULT:
The program for implementing simple webserver is executed successfully.
