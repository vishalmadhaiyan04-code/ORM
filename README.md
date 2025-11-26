# Ex02 Django ORM Web Application
# Date:25/11/2025
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

# DESIGN STEPS
## STEP 1:
Clone the problem from GitHub

## STEP 2:
Create a new app in Django project

## STEP 3:
Enter the code for admin.py and models.py

## STEP 4:
Execute Django admin and create details for 10 cars

# PROGRAM
```
admin.py

from django.contrib import admin
from.models import Car,CarAdmin

admin.site.register(Car,CarAdmin)

models.py

from django.db import models
from django.contrib import admin

class Car(models.Model):
    brand = models.CharField(max_length=10)
    car_name = models.CharField(max_length=10)
    enginenum = models.IntegerField()
    release = models.DateField()

class CarAdmin(admin.ModelAdmin):
    list_display=('brand', 'car_name', 'enginenum', 'release')



 
```
# OUTPUT

<img width="1919" height="1079" alt="Screenshot 2025-11-24 222200" src="https://github.com/user-attachments/assets/c5d253fd-6447-4af0-ba7d-6c83391cfa72" />


<img width="1920" height="1080" alt="Screenshot 2025-11-24 223139" src="https://github.com/user-attachments/assets/65fb86fc-b654-4200-802d-44acbc21058f" />


# RESULT
Thus the program for creating a database using ORM hass been executed successfully
