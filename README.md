# Ex02 Django ORM Web Application
## Date: 5-3-2024

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram


![Screenshot 2024-03-05 101827](https://github.com/SwaminathanV23000747/ORM/assets/148931113/c0433462-03ea-42db-b51f-a64c33673738)


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
class libraryBook(models. Model):
    title=models.CharField(max_length=15);
    BookID=models.IntegerField(primary_key=True);
    author=models.CharField(max_length=10);
    publisher=models.CharField(max_length=8);
    price=models.IntegerField();
    pages=models.IntegerField();
class libraryBookAdmin(admin.ModelAdmin):
   list_display=("title","BookID","author","publisher","price","pages");

admin.py
from django.contrib import admin 
from .models import libraryBook,libraryBookAdmin
admin.site.register(libraryBook,libraryBookAdmin)
```
## OUTPUT


![Screenshot 2024-02-28 102810](https://github.com/SwaminathanV23000747/ORM/assets/148931113/55d08f13-6225-4997-9959-8674d804f41d)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
