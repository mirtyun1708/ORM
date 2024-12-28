# Ex02 Django ORM Web Application
# Date:07.10.2024
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
from django.db import models
from django.contrib import admin

# Create your models here.
class Bank_Loan(models.Model):
    loan_id = models.CharField(max_length=20,primary_key=True)
    loan_type = models.CharField(max_length=30)
    loan_amd = models.FloatField()
    cust_acno = models.IntegerField()
    cust_name = models.CharField(max_length=50)


class Bank_LoanAdmin(admin.ModelAdmin):
    list_display = ('loan_id', 'loan_type','loan_amd','cust_acno','cust_name')

admin.py

from django.contrib import admin
from.models import Bank_Loan, Bank_LoanAdmin

# Register your models here.
admin.site.register( Bank_Loan,Bank_LoanAdmin)
```
# OUTPUT
![WhatsApp Image 2024-12-19 at 2 04 41 PM](https://github.com/user-attachments/assets/1787b628-dff8-45a3-8012-7605e4007ecd)
![WhatsApp Image 2024-12-19 at 2 04 42 PM](https://github.com/user-attachments/assets/894b8076-0668-4c64-be59-155de9ff07af)



# RESULT
Thus the program for creating a database using ORM hass been executed successfully
