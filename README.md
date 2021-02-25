# Ecommerce_Assignment_Astha_Rijal

1: The database is handled in the following section of project @settings.py: DATABASES = { 'default': { 'ENGINE': 'django.db.backends.sqlite3', 'NAME': BASE_DIR / 'db.sqlite3', } }

a. Project Summary
We initialized Django project: django-admin startproject ecom_lab_exam. After that we ensured that the required database and tables are initialized correctly: python manage.py migrate python manage.py createsuperuser Then, we added a module using code: python manage.py startapp ecommerce. It was registered to ‘INSTALLED APPS’ @settings.py. We then added model LabExam inside module: class LabExam(models.Model): exam_date = models.DateTimeField() exam_name = models.CharField(max_length=20) exam_description = models.CharField(max_length=500) total_marks = models.FloatField() pass_marks = models.FloatField() exam_status = models.BooleanField() The created table shall be migrated into the database. Then the model is registered into @admin.py: admin.site.register(LabExam) CRUD operation was performed after running the server.

Features of our Project
We can perform  1. Create 2. Update 3. Delete 4. Read into the created table 'LabExam'.
