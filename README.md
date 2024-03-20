# Ex02 Django ORM Web Application
## Date: 5-3-2024

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![WhatsApp Image 2024-03-21 at 00 10 34_467c52f6](https://github.com/SwaminathanV23000747/ORM/assets/148931113/cddb8ce6-c27a-4f74-a655-904f1205e0d4)



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
model.py
from django.contrib import admin
from django.db import models
class Books(models.Model):
    name=models.CharField(max_length=50);
    author=models.CharField(max_length=20);
    price=models.IntegerField();
    dateofpublication=models.DateField();
    genre=models.CharField(max_length=30);
    code=models.CharField(max_length=20,primary_key=True);
class bookAdmin(admin.ModelAdmin):
      list_display=("name","author","price","dateofpublication","genre","code");

admin.py
from django.contrib import admin
from .models import book,bookAdmin
admin.site.register(book,bookAdmin)

```
## OUTPUT


![Screenshot 2024-02-28 102810](https://github.com/SwaminathanV23000747/ORM/assets/148931113/55d08f13-6225-4997-9959-8674d804f41d)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
