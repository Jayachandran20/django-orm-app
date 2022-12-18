# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

Include your ER diagram here

## DESIGN STEPS

### STEP 1:

### STEP 2:

### STEP 3:

Write your own steps

## PROGRAM
'''
from django.db import models
from django.contrib import admin
# create your model here.

class Bankapp(models.Model):
    accountnumber = models.CharField(max_length=10, help_text="Your Reference Number")
    name = models.CharField(max_length=100)
    mobilenumber = models.IntegerField()
    email = models.EmailField()

class BankingappAdmin(admin.ModelAdmin):
    list_display = ('accountnumber','name','mobilenumber','email')
'''





## OUTPUT

Include the screenshot of your admin page.


## RESULT
