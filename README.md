# EX01 Developing a Simple Webserver

# Date:
# AIM:
To develop a simple webserver to serve html pages and display the configuration details of laptop.

# DESIGN STEPS:
## Step 1:
HTML content creation.

## Step 2:
Design of webserver workflow.

## Step 3:
Implementation using Python code.

## Step 4:
Serving the HTML pages.

## Step 5:
Testing the webserver.

# PROGRAM:
```
views.py:
from django.shortcuts import render
from django.http import HttpResponse
def index(request):
    return render(request,'ed/index.html')
html code:
{%load static%}
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Laptop Configuration</title>
   <link rel="stylesheet" href="{%static 'css/style.css' %}">
    
</head>
<body>
    <div class="container">
        <header>
            <h1>My Laptop Configuration</h1>
        </header>
        <section class="config-details">
            <h2>Specifications</h2>
            <ul>
                <li><strong>Processor:</strong> Intel Core i7-12700K</li>
                <li><strong>RAM:</strong> 16 GB DDR4</li>
                <li><strong>Storage:</strong> 512 GB SSD</li>
                <li><strong>Graphics:</strong> NVIDIA GeForce RTX 3060</li>
                <li><strong>Display:</strong> 15.6" Full HD</li>
                <li><strong>Operating System:</strong> Windows 11</li>
                <li><strong>Battery:</strong> 6-cell Li-ion, 50Wh</li>
            </ul>
        </section>
        <footer>
            <p>Created by: prabanjan</p>
        </footer>
    </div>
</body>
css code:


body {
    font-family: Arial, sans-serif;
    background-color: #f4f4f9;
    color: #6d6464;
    line-height: 1.6;
}


.container {
    width: 80%;
    max-width: 800px;
    margin: auto;
    margin-top: 3%;
    padding: 70px;
    background-color: #1d1d1d;
    box-shadow: 0 2px 10px rgb(254, 0, 0);
    border-radius: 50px;
}


header {
    text-align: center;
    margin-bottom: 300x;
}

header h1 {
    font-size: 2.5em;
    color: #2464ee;
    text-shadow: #534e4e;
    
    
}


.config-details {
    margin-bottom: 30px;
}

.config-details h2 {
    font-size: 1.8em;
    color: #534e4e;
    margin-bottom: 10px;
}

.config-details ul {
    list-style-type: none;
}

.config-details ul li {
    margin-bottom: 10px;
    font-size: 1.5em;
}

.config-details ul li strong {
    color: #007BFF;
}


footer {
    text-align: center;
    font-size: 0.5em;
    color: #777;
}
```

# OUTPUT:
![alt text](<Screenshot 2024-11-29 112147.png>)
![alt text](<Screenshot 2024-11-29 112137.png>)
# RESULT:
The program for implementing simple webserver is executed successfully.
