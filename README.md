# Ex02 Django ORM Web Application
## Date: 22-03-2024
## Name: Mugil Raj S A
## Reg.no: 212223220062
## Dept: IT

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![Screenshot 2024-03-22 154650](https://github.com/MugilRaj1105/ORM/assets/154905390/3b3bfe50-e1c3-4228-81d8-1c463e45cb09)



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

from django.db import models
from django.contrib import admin
class Employee (models.Model):
    eid=models.CharField(max_length=20,primary_key=True)
    name=models.CharField(max_length=100)
    salary=models.IntegerField()
    age=models.IntegerField()
    email=models.EmailField()
 
class EmployeeAdmin(admin.ModelAdmin):
    list_display=('eid','name','salary','age','email')

models.py

from django.contrib import admin
from .models import Employee,EmployeeAdmin
admin.site.register(Employee,EmployeeAdmin)

````

## OUTPUT

![Screenshot 2024-03-22 154511](https://github.com/MugilRaj1105/ORM/assets/154905390/a008c747-be0a-4833-a855-5b7aaa7928ef)




## RESULT
Thus the program for creating a database using ORM hass been executed successfully
