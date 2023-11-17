# Ex02 Django ORM Web Application
## Date: 

## AIM
To develop a Django application to store and retrieve data from a Football Players database using Object Relational Mapping(ORM).

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
Execute Django admin and create 10 Football players

## PROGRAM:
```
models.py
from django.db import models
from django.contrib import admin
class Football_player (models.Model):
    name=models.CharField(max_length=20)
    age=models.IntegerField()
    country=models.CharField(max_length=20)
    height=models.IntegerField()
    email=models.EmailField()
class Football_playerAdmin(admin.ModelAdmin):
    list_display=['name','age','country','height','email']
from django.contrib import admin
from .models import Football_player,Football_playerAdmin
admin.site.register(Football_player,Football_playerAdmin)

```

## OUTPUT:
![Screenshot 2023-10-19 114748](https://github.com/HariharanJayavel/ORM/assets/144870546/853cb75f-0204-4b91-8697-196f9cb6d0be)

## RESULT
Thus the program for creating a database using ORM hass been executed successfully
