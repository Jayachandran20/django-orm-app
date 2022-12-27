# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram
![Screenshot (20)](https://user-images.githubusercontent.com/118447015/209692606-19bfc1b1-1614-433c-967b-dfa2053df371.png)



## DESIGN STEPS

### STEP 1:
create a new django project using "django_admin startproject",get into the project terminal and use "python3 manage.py startapp" command

### STEP 2:
Define a model for the bankingapp in the models.py and allow host access and add the app
name under installed apps in settings.py

### STEP 3:
Register the models with the Django admin side.In admin.py under app folder,register the
models with Django admin site

## PROGRAM
```
from django.db import models
from django.contrib import admin

class Bankapp(models.Model):
    accountnumber = models.CharField(max_length=10, help_text="Your Reference Number")
    name = models.CharField(max_length=100)
    mobilenumber = models.IntegerField()
    email = models.EmailField()

class BankingappAdmin(admin.ModelAdmin):
    list_display = ('accountnumber','name','mobilenumber','email')
```





## OUTPUT




![Screenshot (15)](https://user-images.githubusercontent.com/118447015/209692669-30537f4a-1e2f-42dd-99d9-6e9fc5f2ddc7.png)




## RESULT
The program is executed sucessfully
