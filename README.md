# Ex02 Django ORM Web Application
## NAME: AVINASH T
## REG NO: 212223230026
## Date: 

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

Include your ER diagram here

## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create details for 10 books

## PROGRAM

```c
models.py

from django.db import models
from django.contrib import admin
class bookdetails(models.Model):
       bookid=models.IntegerField(primary_key=true);
       bookname=models.CharField(max_length=25);
       author=models.CharField(max_length=20);
       publishedyear=models.DateField();
       price=models.IntegerField();
       publishedcompany=models.CharField(max_length=20);
class bookdetailsAdmin(admin.ModelAdmin):
      list_dispaly=("bookid","bookname","author","publishedyear","price","publishedcompany");

admin.py

from django.contrib import admin
from .models import bookdetails,bookdetailsAdmin
Admin.site.register(bookdetails,bookdetailsAdmin)

```
## OUTPUT

Include the screenshot of your admin page.


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
