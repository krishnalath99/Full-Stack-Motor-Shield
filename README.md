# Motor Shield (Vehicle Insurance Company)
Pull the entire repository on your system and then follow the steps below:
## Backend using Django and Frontend Using React
### (You must have **Python** and **NPM(NodeJS)** installed and added in your environment variables path)
1. Open terminal and navigate to the **[Full-Stack-Motor-Shield->Django - Backend]** folder.
2. Create a virtual environment in this directory by typing in cmd : **[virtualenv name_of_env]**
3. Activate the Virtual Environment using **[name_of_env\Scripts\activate]**
4. Install the following dependencies after activating the virtual environment:
```sh
pip instll chardet   
pip install django   
pip install django-cors-headers   
pip install django-dotenv   
pip install djangorestframework   
pip install djangorestframework-simplejwt   
> Install the SQL clent for the RDBMS you are using. Ex: **pip install mysqlclient** or **pip install mssql-django   
pip install django-jazzmin   
pip install pillow
```
6. Create a Database in the SQL client that you installed in your environment.
7. Go to **[Django - Backend->MotorShield->InsuranceProject->settings.py]** file. Scroll down this file and go to "DATABASES" variable and change the ENGINE, NAME, HOST, USER, PASSWORD, and PORT according to the RDBMS you are using and your newly created database in that RDBMS.
8. Save Everything.
9. Search and delete all the **pycache** and **Migrations** folders from the **MotorShield** directory and also its sub-directories.
10. Now, navigate to the **MotorShield** directory (in **Django - Backend** folder) inside the terminal and make migrations to the RDBMS using the following commaands:
```sh
python manage.py makemigrations MotorInsuranceCompany   
python manage.py migrate   
```
11. Create the super user to login to the admin panel using the command: **[python manage.py createsuperuser]** and enter all the details you want for admin login.
12. Run the server using the command: **[python manage.py runserver]**. Go to the browser and search for this url http://127.0.0.1:8000/admin/
13. Note: **The website that you see when you visit the url http://127.0.0.1:8000/ is not our actual react-website, this website was only created for testing purpose of the backend.** Please refrain from using it or else the backend server might malfunction.
14. Login to the admin panel using the superuser details that you created. If everything goes well then you should see Users, Vehicles, Policy and Claims menu on the left side after logging in to admin panel.
15. Thats it your backend server is now up and running.
16. Let your backend server run in the background and now lets move on to the frontend part.
17. Open terminal and navigate to the **[Full-Stack-Motor-Shield->React  - Frontend->MotorShield]** folder.
18. Now install all the dependencies using the following commands :
```sh
npm install axios   
npm install prop-types   
npm install react    
npm install react-dom   
npm install react-router   
npm install react-router-dom   
npm install react-scroll   
npm install react-toastify
```   
20. Now run the React Frontend server using the command : **[npm run server]**. Since I have used **[vite]** to create this react app.
21. Go to the browser and visit the url http://localhost:5173/. If everything goes well you will have the React frontend website on your browser.
22. You can SignUp to create a new account, then login, apply for a policy by adding a vehicle, make payment for policy upon background verification done in the admin panel file for a claim and do many such things what you do on a Vehicle Insurance Company's website.
