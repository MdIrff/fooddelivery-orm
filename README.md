Ex01 Django ORM Web Application
Date:
AIM
To develop a Django application to manage an online food delivery platform like Zomato/Swiggy using Object Relational Mapping (ORM).

ENTITY RELATIONSHIP DIAGRAM
DESIGN STEPS
STEP 1:
Clone the problem from GitHub

STEP 2:
Create a new app in Django project

STEP 3:
Enter the code for admin.py and models.py

STEP 4:
Execute Django admin and create details for 10 books

PROGRAM
admin.py
```
from django.contrib import admin
from .models import Restaurant

admin.site.register(Restaurant)
```
models.py
```
from django.db import models
class Restaurant(models.Model):
    restaurant_id = models.AutoField(primary_key=True)
    restaurant_name = models.CharField(max_length=100)
    owner_name = models.CharField(max_length=100)
    food_type = models.CharField(max_length=50)
    rating = models.FloatField()
    location = models.CharField(max_length=100)
    delivery_time = models.IntegerField()

    def __str__(self):
        return self.restaurant_name
```

OUTPUT
<img width="1919" height="1010" alt="image" src="https://github.com/user-attachments/assets/7cc8e60f-32d8-41ea-bdd8-39e62e1e8382" />


RESULT
Thus the program for creating a database using ORM hass been executed successfully
