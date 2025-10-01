# Ex.06 Book Front Cover Page Design
# Date:
# AIM:
To design a book front cover page using HTML and CSS.

# DESIGN STEPS:
## Step 1:
Create a Django Admin project.

## Step 2:
Create an app in the Django interface.

## Step 3:
Create a folder named 'static' in the app folder.

## Step 4:
Create a new HTML file in the static folder.

## Step 5:
Write the HTML code with relevant CSS properties.

## Step 6:
Choose the appropriate style and color scheme.

## Step 7:
Insert the images in their appropriate places.

## Step 8:
Publish the website in the LocalHost.

# PROGRAM:
views.py 

from django.shortcuts import render

# Create your views here.
def book(request):
return render(request,'book.html')


urls.py


from django.contrib import admin
from django.urls import path
from book import views
urlpatterns = [
path('admin/', admin.site.urls),
path('',views.book)
]


book.html


    {% load static %}

    <head>
    <title>Book Cover</title>
      </head>
      <body style="margin: 0; padding: 0; display: flex; justify-content: center; align-items: center; height: 100vh; background: #fff;">

      <div style="width: 350px; height: 500px; background: linear-gradient(135deg, #040404ff, #363333ff); color: white; padding: 20px; position: relative; border: 5px solid #fff;">

    <p style="font-size: 14px; font-weight: bold;">SEC Insights</p>

    <h1 style="font-size: 22px; font-weight: bold; text-align: center; line-height: 1.4;">FUNDAMENTALS OF<br>WEB APPLICATION DEVELOPMENT</h1>

    <p style="font-size: 14px; text-align: center;">Deep Dive in HTML, CSS & JS Basics</p>
    <p style="font-size: 14px; text-align: center;">Top seller of 2025</p>

    <div style="display: flex; align-items: center;">
        
        <div style="position:absolute;bottom:100px;right:30px;width: 80px; height: 80px;border:5px solid grey;border-radius:25%;overflow:hidden;">
        <img src={%static "naveen.png"%} alt="naveen.png" style="width: 100%; height: 100%;"></div>
            
    
        <div><p style="position:absolute;bottom:80px;right:56px;font-size: 14px; margin: 0;text-shadow:-1px -1px 0 #000,1px -1px 0 #000,-1px 1px 0 #000,1px 1px 0 #000;">Naveen</p>
        <p style="position:absolute;bottom:65px;right:56px;font-size: 14px; margin: 0;text-shadow:-1px -1px 0 #000,1px -1px 0 #000,-1px 1px 0 #000,1px 1px 0 #000;">SEC</p></div>
    
    </div>

    <div style="position: absolute; bottom: 20px; left: 20px; background-color: #ff4500; font-size: 14px; font-weight: bold;">
      <p style="margin: 0;">SPECIAL EDITION</p></div>
    

      </div>

    </body>
    </html>



# OUTPUT:
# RESULT:
The program for designing book front cover page using HTML and CSS is completed successfully.
