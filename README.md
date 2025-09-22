# Ex02 Django ORM Web Application
# Date:22-09-25
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

# ENTITY RELATIONSHIP DIAGRAM
## DESIGN STEPS
## STEP 1:
Clone the problem from GitHub

## STEP 2:
Create a new app in Django project

## STEP 3:
Enter the code for admin.py and models.py

## STEP 4:
Execute Django admin and create details for 10 books

# PROGRAM
```
Models.py
from django.db import models
from django.contrib import admin
class Car_Inventory(models.Model):
    Car_name=models.CharField(max_length=20,default="no name")
    Car_color=models.CharField(max_length=30)
    Car_model=models.CharField(max_length=20,default="null")
    Car_Id=models.IntegerField(primary_key=True,default="0")
    Car_Engine=models.CharField(max_length=20,default="no")

    
class Car_InventoryAdmin(admin.ModelAdmin):
    list_display=('Car_name','Car_color','Car_model','Car_Id','Car_Engine')

Admin.py
from django.contrib import admin
from .models import Car_Inventory,Car_InventoryAdmin
admin.site.register(Car_Inventory,Car_InventoryAdmin)
```

# OUTPUT
![alt text](<Screenshot 2025-09-22 104510.png>)
![alt text](<Screenshot 2025-09-22 103351.png>)

# RESULT
Thus the program for creating a database using ORM hass been executed successfully
