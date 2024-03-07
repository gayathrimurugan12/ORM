# Ex02 Django ORM Web Application
## Date: 06-03-2024

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![WhatsApp Image 2024-03-06 at 22 30 03_c75f8031](https://github.com/gayathrimurugan12/ORM/assets/149365374/a0aad5cc-ed86-443c-9762-5840d227bee1)


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
admin.py

from django.contrib import admin
from .models import Book,BookAdmin
admin.site.register(Book,BookAdmin)

models.py
from django.db import models
from django.contrib import admin
class Book(models.Model):
   serialno=models.IntegerField(primary_key=True);
   Bookname=models.CharField(max_length=30);
   Author=models.CharField(max_length=20);
   publishedDate=models.DateField();
   Booktype=models.CharField(max_length=20);
   pic=models.ImageField();
class BookAdmin(admin.ModelAdmin):
   list_display=("serialno","Bookname","Author","publishedDate","Booktype","pic");

```


## OUTPUT


![Screenshot 2024-03-01 205059](https://github.com/gayathrimurugan12/ORM/assets/149365374/6cf869a2-c8e6-4526-909f-e15a8db487e4)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
