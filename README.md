# Ex02 Django ORM Web Application
## NAME: AVINASH T
## REG NO: 212223230026
## Date: 05.03.24

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram
![alt text](PIC.png)

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

```
models.py

from django.db import models
from django.contrib import admin
class bookdetails(models.Model):
       bookid=models.IntegerField()
       bookname=models.CharField(max_length=25)
       author=models.CharField(max_length=20)
       publishedyear=models.DateField()
       price=models.IntegerField()
       publishedcompany=models.CharField(max_length=20)
class bookdetailsAdmin(admin.ModelAdmin):
      list_display=("bookid","bookname","author","publishedyear","price","publishedcompany")

admin.py

from django.contrib import admin
from .models import bookdetails,bookdetailsAdmin
admin.site.register(bookdetails,bookdetailsAdmin)

```
## OUTPUT

![Alt text](<Screenshot (76).png>)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
