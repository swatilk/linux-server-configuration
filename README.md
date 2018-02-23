# Deploy Item Catalog app on linux server
1) The IP address and SSH port so your server can be accessed

IP Address: 35.165.86.32
SSH Port: 220

2) The complete URL to your hosted web application.
http://ec2-35-165-86-32.us-west-2.compute.amazonaws.com/


3) A summary of software you installed and configuration changes made.
## Installed Software
PostgreSQL
Apache 2
Mod_WSGI
Flask
venv

https://www.digitalocean.com/community/tutorials/how-to-deploy-a-flask-application-on-an-ubuntu-vps

## Configurations made
- Enabled mod_wsgi
- Cloned the existing Flask App for ItemCatalog https://github.com/swatilk/item-catalog and configured it to follow mod_wsgi folder structure
- Created a PostgreSQL Database (newcategory)
- Created a user to be able to access the database, with the same name
- Created Apache configuration file
- Configured Virtual Host with the Amazon public IP address and path to wsgi file
- Restart Apache and access it the URL in step 2


4) A list of any third-party resources used to complete this project
Amazon LightSail
Google+ OAuth

5) Locate the SSH key for grader user

 $ cat ~/.ssh/GraderKeyPair




