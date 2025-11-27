# Ex02 Django ORM Web Application
## Date: 27-11-2025

## AIM
To develop a Django Application to store and retrieve data from a E-Commerce Website Database for Amazon or Flipkart using Object Relational Mapping(ORM).


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

```

models.py

from django.db import models
from django.contrib import admin

class Car_DB(models.Model):
    car_brand=models.CharField(max_length=10)
    order_id=models.IntegerField(primary_key=True)
    car_model=models.CharField()
    price=models.IntegerField()
    purchase_date=models.DateField()

class Car_DBAdmin(admin.ModelAdmin):
    list_display=["car_brand","order_id","car_model","price","purchase_date"]
admin.py

from django.contrib import admin
from.models import Car_DB,Car_DBAdmin
admin.site.register(Car_DB,Car_DBAdmin)

```


## OUTPUT

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/dbe4a5b6-3a5a-439f-a4fe-2f07f0f3d77c" />

## RESULT
Include the screenshot of your admin page.


## RESULT
Thus the program for creating E-commerce website database using ORM hass been executed successfully
