# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

Include your ER diagram here

## DESIGN STEPS

### STEP 1:
Fork and clone the repositary in to your IDE

### STEP 2:
Create a django project and an app and a superuser account and run the server

### STEP 3:
Modify changes in settings and write your code on models and admin and run the server.

### STEP 4:
login in to admin using your superuser account and populate the record.

## PROGRAM

```python
from django.db import models
from django.contrib import admin

class Employee (models.Model):
   emp_id=models.CharField(primary_key=True,max_length=4,help_text='Employee ID')
   ename=models.CharField(max_length=50)
   post=models.CharField(max_length=20)
   phonenumber=models.IntegerField()
   salary=models.IntegerField()

class EmployeeAdmin(admin.ModelAdmin):
    list_display=('emp_id','ename','post','phonenumber','salary')
```

## OUTPUT

Include the screenshot of your admin page.


## RESULT
