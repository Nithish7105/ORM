# Ex02 Django ORM Web Application
## Date: 1.04.2024

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
```
# Register your models here.
from django.contrib import admin
from .models import footballPlayer,footballPlayerAdmin
admin.site.register(footballPlayer,footballPlayerAdmin)
```
```
# Create your models here.
from django.db import models
from django.contrib import admin
class footballPlayer(models.Model):
	name=models.CharField(max_length=30)
	age=models.IntegerField()
	goals=models.IntegerField()
	jerseynumber=models.IntegerField()
	team=models.CharField(max_length=25)
	NumberofMatches=models.IntegerField()
class footballPlayerAdmin(admin.ModelAdmin):
	list_display=["name","age","goals","jerseynumber","team","NumberofMatches"]
```

## OUTPUT
![WhatsApp Image 2024-04-25 at 9 40 23 AM](https://github.com/Nithish7105/ORM/assets/149516932/207ebdd5-d744-4a0d-a6a4-9ad46131dd2f)



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
