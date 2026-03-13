# Article CMS (FlaskWebProject)

This project is a Flask web application deployed on Microsoft Azure.  
The application allows users to log in, create articles, edit articles, and upload images. Article data is stored in Azure SQL Database, while images are stored in Azure Blob Storage.

Authentication is implemented using OAuth2 with Microsoft Sign-In (MSAL library), and logging has been added to track successful and failed login attempts.

---

# Live Application

The application is deployed on Azure App Service.

URL:

https://cmsapp123-h2dmfmhvg3dha6c5.westeurope-01.azurewebsites.net

---

# Features

- User login and logout
- Create and edit articles
- Upload images for articles
- Article data stored in Azure SQL Database
- Images stored in Azure Blob Storage
- Microsoft OAuth2 login using MSAL
- Logging for successful and invalid login attempts
- Deployment using Azure App Service

---

# Azure Resources Used

The following Azure resources were created for this project:

- Azure Resource Group
- Azure App Service
- Azure App Service Plan
- Azure SQL Server
- Azure SQL Database
- Azure Storage Account (Blob Storage)
- Microsoft Entra ID App Registration

These services work together to host the web application, store data, and manage authentication.

---

# Application Login

You can log in using the following credentials:

Username: admin  
Password: admin

Alternatively, click Sign in with Microsoft, which automatically logs into the admin account.

---

# Article Example

To verify the application works, an article was created with the following information:

Title: Hello World!  
Author: Jane Doe  
Body: My name is Jane Doe and this is my first article!

An image was uploaded and stored in Azure Blob Storage.

---

# Logging

Application logging was implemented to track login activity.

Examples include:

- Invalid login attempt
- Successful login

Logs can be viewed in the Azure App Service Log Stream.

---

# Project Structure

FlaskWebProject/

- init.py  
- views.py  
- models.py  
- forms.py  
- templates/  
- static/  

Other project files:

- application.py  
- config.py  
- requirements.txt  
- WRITEUP.md  

---

# Deployment

The application was deployed using Azure App Service.

Azure App Service was selected instead of a Virtual Machine because it simplifies deployment, automatically manages infrastructure, and integrates easily with Azure services such as SQL Database and Blob Storage.

More details about this decision can be found in WRITEUP.md.

---

# Dependencies

- Python 3.12
- Flask
- Flask-Login
- Flask-SQLAlchemy
- MSAL
- Azure Storage SDK

All dependencies are listed in:

requirements.txt

---

# Screenshots Provided

The following screenshots were captured as part of the project submission:

- Article created in the CMS with URL visible
- Azure Resource Group showing deployed resources
- SQL Database query showing stored article data
- Azure Blob Storage container with uploaded image
- Blob storage endpoint
- Redirect URIs for Microsoft authentication
- Log stream showing login attempts

---

# Cleanup

After grading, the Azure Resource Group should be deleted to avoid unnecessary charges.
