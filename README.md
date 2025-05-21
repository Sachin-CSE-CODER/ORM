# Ex02 Django ORM Web Application
## Date: 21-05-2025

## AIM
To develop a Django application to store and retrieve data from a Movies Database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM
C:\Users\theri\ORM\Screenshot 2025-05-21 143555.png


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
admin.py
'''


from django.contrib import admin
from .models import Book, BookAdmin
admin.site.register(Book, BookAdmin)
'''
models.py
'''

from django.db import models
from django.contrib import admin

class Book(models.Model):
  Name= models.CharField(max_length=100)
  Email= models.EmailField()
  Book_No= models.CharField(max_length=100)
  Book_Name= models.CharField(max_length=100)
  Address= models.CharField(max_length=255)
  Phone_No= models.CharField(max_length=15)
class BookAdmin(admin.ModelAdmin):
    list_display = ('Name','Email','Book_No','Book_Name','Address','Phone_No')
'''


## OUTPUT
C:\Users\theri\ORM\Screenshot 2025-05-21 142647.png


## RESULT
Thus the program for creating movies database using ORM hass been executed successfully
