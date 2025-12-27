# Ex02 Django ORM Web Application
## Date: 

## AIM
To develop a Django application to store and retrieve data from a Car Inventory Database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM



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
models.py
from django.db import models
from django.contrib import admin
# Create your models here.
class Student(models.Model):
    student_name = models.CharField(max_length=20, help_text="Enter Student Name")
    age = models.IntegerField(help_text="Enter age between 18 to 22")
    dob = models.DateField()
    reg_no = models.IntegerField(help_text="Enter the Register Number")

class StudentAdmin(admin.ModelAdmin):
    list_display = ['student_name', 'age', 'dob', 'reg_no']


admin.py
from django.contrib import admin
from .models import Student, StudentAdmin
# Register your models here.
admin.site.register(Student, StudentAdmin)


## OUTPUT

![WhatsApp Image 2025-12-27 at 4 11 26 PM](https://github.com/user-attachments/assets/a66f1220-88cd-47fd-ad9a-ad6c5cee4be5)
![WhatsApp Image 2025-12-27 at 4 12 52 PM](https://github.com/user-attachments/assets/54f831e9-a8d1-4e6f-b76b-9260bd960c05)
![WhatsApp Image 2025-12-27 at 4 13 45 PM](https://github.com/user-attachments/assets/9410a92b-6324-4b1a-9769-d26105d7d38a)



## RESULT
Thus the program for creating car inventory database database using ORM hass been executed successfully
