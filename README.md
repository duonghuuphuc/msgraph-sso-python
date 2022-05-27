# Single Sign-on with Microsoft Graph API

This repository presents a Flask application that demonstrates the implementation of single sign-on based on Microsoft Graph. You can freely clone this project to implement the **Sign in with Microsoft** functionality.


## API functionality demonstrated in this sample

 - Log-in users with Microsoft OAuth2
 - Retrieve users' information with Microsoft Azure Active Directory


## Overview of SSO based on Microsoft Azure AD

![Fig. 1. Overview of SSO based on Microsoft Azure Active Directory](https://www.duonghuuphuc.com/sites/dev/static/img/20220526B/sso-ms-azure-active-directory.png)


## Prerequisite

 - A Microsoft 365 account with an active subscription such as Home or Business plan
 - If you are trying this tutorial within an organization that subscribes to Microsoft 365 Business plan, you also need to have an Administrator account to grant permissions on the created application
 - You should have a background in Python programming language to understand the sample Flask project.


## Step-by-step tutorials

There is an article that presents the procedure to implement the single sign-on functionality for users having either personal Microsoft accounts (Skype, Xbox, Live, and Hotmail) or work accounts. The procedure consists of four main steps, i.e., (1) create an application on Microsoft Azure, (2) issue credentials, (3) add API permissions to the application, and (4) run the demo program.

Read the article at https://www.duonghuuphuc.com/sites/dev/msgraph-sso-python-en.html


## TL;DR

You can jump right into the demo by performing the following steps:

 1. Register an application on [Microsoft Azure](https://go.microsoft.com/fwlink/?linkid=2083908)
 2. Create application credentials on Microsoft Azure
 3. Grant API permissions: `User.Read` and `User.ReadBasic.All`
 4. Clone the demo project from this repository
 5. Configure `CLIENT_ID` and `CLIENT_SECRET` in the **env.sh** file
 6. [Optional] Create a new Python environment to avoid any errors in your current working environment
 7. Install required packages by executing this command in an activated Python environment: `pip install -r requirements.txt`
 8. Run the project by executing this command: `source env.sh`

*Note: step #7 is performed only one time.*


## Application screenshots

![Fig. 2. Homepage of the demo Flask project for anonymous users](https://www.duonghuuphuc.com/sites/dev/static/img/20220526B/app_screenshot_01.png)

![Fig. 3. Homepage of the demo Flask project for authenticated users](https://www.duonghuuphuc.com/sites/dev/static/img/20220526B/app_screenshot_02.png)

![Fig. 4. Print the requested permissions of the application](https://www.duonghuuphuc.com/sites/dev/static/img/20220526B/app_screenshot_03.png)

![Fig. 5. Application homepage (client side)](https://www.duonghuuphuc.com/sites/dev/static/img/20220526B/app_screenshot_04.png)

![Fig. 6. Get and render the user profile with basic information such as email address, name, and user id obtained from Microsoft Azure Active Directory](https://www.duonghuuphuc.com/sites/dev/static/img/20220526B/app_screenshot_05.png)

![Fig. 7. Get and render the Access Token on a web page](https://www.duonghuuphuc.com/sites/dev/static/img/20220526B/app_screenshot_06.png)


## Known issues

 - If you run this sample project on a web server on a home network without a static IP address and/or without an assigned domain name, you may need to use a [DDNS](https://www.cloudflare.com/learning/dns/glossary/dynamic-dns/) provider, and then forward the corresponding network ports to your web server.


## Further Reading

 - Tutorial: [Microsoft Graph — Send Mail API](https://www.duonghuuphuc.com/sites/dev/msgraph-sendmail-python-en.html)
 - Tutorial: [Microsoft Graph — Single Sign-on](https://www.duonghuuphuc.com/sites/dev/msgraph-sso-python-en.html)
 - [Microsoft Azure - Authentication vs. authorization](https://docs.microsoft.com/en-us/azure/active-directory/develop/authentication-vs-authorization)
 - [Microsoft Authentication Library (MSAL) for Python](https://docs.microsoft.com/en-us/python/api/overview/azure/active-directory?view=azure-python)
 - [Azure Active Directory B2C](https://azure.microsoft.com/en-us/services/active-directory/external-identities/b2c/#overview)


## Contributors

 - Phuc H. Duong / [www.duonghuuphuc.com](https://www.duonghuuphuc.com/) / `dhpit [at] m.dhpit.com`

