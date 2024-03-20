# Ex02 Django ORM Web Application
## Date: 15/03/2024

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![alt text](image-1.png)

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
from django.contrib import admin
# Register your models here.
from.models import Book,BookAdmin
admin.site.register(Book,BookAdmin) 

models.py 

from django.db import models
from django.db import models
from django.contrib import admin
# Create your models here.
class Book(models.Model):
    book_id= models.IntegerField(primary_key=True)
    book_name= models.CharField(max_length=50)
    publisher_name= models.CharField(max_length=50)
    author_name= models.CharField(max_length=50)
    publish_year= models.DateField()

class BookAdmin(admin.ModelAdmin):
    list_display= ('book_id','book_name','publisher_name','author_name','publish_year')
```    
## OUTPUT

![alt text](<Screenshot 2024-03-15 144332.png>)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
