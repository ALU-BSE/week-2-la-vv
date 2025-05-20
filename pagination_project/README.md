# Django Pagination Hands-On Project

A simple Django project demonstrating how to implement pagination using a model populated with AI-generated book data.

## Objective
1.Learn how to:
Set up a Django project
Create a model and populate it with data
Implement pagination to efficiently display large datasets

## Getting Started

📦 Prerequisites
1. Python (3.x)
2. Django (pip install django)

## 🛠️ Project Setup

bash
### Step 1: Create a new Django project and app
django-admin startproject pagination_project
cd pagination_project
python manage.py startapp books
⚙️ Configuration
Add 'books' to INSTALLED_APPS in pagination_project/settings.py.

## Run initial migrations:

bash
python manage.py migrate

## 🧱 Define the Model
Create a Book model in books/models.py:

python
from django.db import models

class Book(models.Model):
    title = models.CharField(max_length=200)
    author = models.CharField(max_length=100)
    published_year = models.IntegerField()

    def __str__(self):
        return self.title


## ✅ Learning Outcomes
By completing this project, you will:

Build a Django project from scratch

Populate a model using AI or data tools

Implement server-side pagination in Django

## Resources

1. Document : https://docs.google.com/document/d/11LCfUEB7kv_ros5wwEB71N1EkE1qndAxdKid5Kv-pCk/edit?usp=sharing

2. Github : "https://github.com/ALU-BSE/week-2-la-vv.git"
