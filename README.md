# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![er](/a.jpeg)

## DESIGN STEPS

### STEP 1:
Create a project and inside the project folder, create an application using - django-admin startproject and django-admin startapp .Inside the applicaton folder, open setiings.py and allow all the hosts.

### STEP 2:
Now in the application folder, open models.py and write the code for your desired table here. Go to admin.py and migrate all your data.

### STEP 3:
On running the server, open the html page.Here you can add or get the desired data from the table you have created.


## PROGRAM:
```py
from django.db import models
from django.contrib import admin
# Create your models here.
class train(models.Model):
    trainnumber = models.IntegerField(max_length=10, help_text="Your Train Number")
    name =models.CharField(max_length=100)
    age = models.IntegerField() 
    email = models.EmailField()
    destination = models.CharField(max_length=100)
    stationname = models.CharField(max_length=100)
    destination = models.CharField(max_length=100)
    classtype = models.CharField(max_length=128)
    depaturedate = models.DateField()
class TrainAdmin(admin.ModelAdmin):
    list_display = ('trainnumber','name','age','email','stationname','destination','classtype','depaturedate')    

```


## OUTPUT

![output](/arshatha.png)


## RESULT:
Thus Django application to store and retrieve data from a database using Object Relational Mapping(ORM) is successfully executed.
