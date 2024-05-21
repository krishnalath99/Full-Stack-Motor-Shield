# Motor Shield (Vehicle Insurance Company)
Pull the entire repository on your system and then follow the steps below:
## Backend using Django.
### (You must have **Python** installed and added in your environment variables path)
1. Open terminal and navigate to the **[Full-Stack-Motor-Shield->Django - Backend]** folder.
2. Create a virtual environment in this directory by typing in cmd : **[virtualenv name_of_env]**
3. Activate the Virtual Environment using **[name_of_env\Scripts\activate]**
4. Install the following dependencies after activating the virtual environment:
   > **pip instll chardet**   
   > **pip install django**   
   > **pip install django-cors-headers**
   > **pip install django-dotenv**   
   > **pip install djangorestframework**   
   > **pip install djangorestframework-simplejwt**   
   > Install the SQL clent for the RDBMS you are using. Ex: **pip install mysqlclient** or **pip install mssql-django**   
   > **pip install django-jazzmin**   
   > **pip install pillow**
5. Create a Database in the SQL client that you installed in your environment.
6. Go to **[Django - Backend->MotorShield->InsuranceProject->settings.py]** file. Scroll down this file and go to "DATABASEs" variable and change the ENGINE, NAME, HOST, USER, PASSWORD, and PORT according to the RDBMS you are using and your newly created database in that RDBMS.
7. Save Everything.
8. Search and delete all the **pycache** and **Migrations** folders from the **MotorShield** directory and also its sub-directories.
9. Now, navigate to the **MotorShield** directory (in **Django - Backend** folder) inside the terminal and make migrations to the RDBMS using the following commaands:
    > **[python manage.py makemigrations MotorInsuranceCompany]**   
    > **[python manage.py migrate]**   
10. Create the super user to login to the admin panel using the command: **[python manage.py createsuperuser]** and enter all the details you want for admin login.
11. Run the server using the command: **[python manage.py runserver]**. Go to the browser and search for this url http://127.0.0.1:8000/admin/
12. Note: **The website that you see when you visit the url http://127.0.0.1:8000/ is not our actual react-website, this website was only created for testing purpose of the backend.** Please refrain from using it or else the backend server might malfunction.
13. Login to the admin panel using the superuser details that you created. If everything goes well then you should see Users, Vehicles, Policy and Claims menu on the left side after logging in to admin panel.
14. Thats it your backend server is now up and running. Now lets move to the frontend part.
<br>
<br>
<br>
## Frontend using React.   
### (You must have **NodeJS* installed and **npm** added in your environment variables path)   
1. Open terminal and navigate to the **[Full-Stack-Motor-Shield->React  - Frontend]** folder.
2. 
