# Ex02 Django ORM Web Application
## Date: 

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

## PROGRAMmodels.py
from django.db import models
from django.contrib import admin
class BookDetails(models.Model):
   student_name=models.CharField(max_length=20);
   id_no=models.IntegerField();
   email=models.EmailField();
   BookName=models.CharField(max_length=100,primary_key="True");
   author_name=models.CharField(max_length=20);
   Total_page=models.IntegerField();

class BookDetailsAdmin(admin.ModelAdmin):
  list_display=("student_name","id_no","email","BookName","author_name","Total_page")


admin.py
from django.contrib import admin
from .models import BookDetails,BookDetailsAdmin
admin.site.register(BookDetails,BookDetailsAdmin)



## OUTPUT

![image](https://github.com/yogeshwaran72/ORM/assets/153492924/616c935b-775c-4f46-950c-b79faccc12fc)



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
