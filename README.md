# E-commerce Web Project
> An e-commerce web application built with the Django framework. Media & static files hosted on AWS S3, and website hosted on Heroku.
> Live demo [_here_](https://garcia-ecommerce-project.herokuapp.com/). <!-- If you have the project hosted somewhere, include the link here. -->

## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Features](#features)
* [Screenshots](#screenshots)
* [Setup](#setup)
* [Usage](#usage)
* [Project Status](#project-status)
* [Room for Improvement](#room-for-improvement)
* [Acknowledgements](#acknowledgements)
<!-- * [License](#license) -->


## General Information
The purpose of this project was to create a fully-functioning e-commerce website using Python and Django. I have used popular e-commerce website builder frameworks such as Wordpress and Shopify, and noticed the limited features available so I decided to create my own e-commerce website for educational purposes.
<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- Django - version 3.2.13
- Python - version 3.10.4
- AWS S3
- PostgreSQL
- Heroku
- Bootstrap 4


## Features
- Login/Sign Up Component
- User Dashboard
- Store Catalog
- PayPal payment system
- Product Galleries
- Cart Functionalities 


## Screenshots
#### Home Page
<img width="400" alt="ecommerce-1" src="https://user-images.githubusercontent.com/38366630/166820695-a8dd77a7-7e69-4f03-b2ad-95ef26dc869d.png">

#### Store Catalog 
<img width="400" alt="ecommerce-2" src="https://user-images.githubusercontent.com/38366630/166820706-9e79c840-94b4-465b-a985-16b85595e331.png">

#### Product Info
<img width="400" alt="ecommerce-3" src="https://user-images.githubusercontent.com/38366630/166820718-5ac8f735-c03f-4ac3-9fff-76be0d3bcd52.png">

#### User Dashboard
<img width="400" alt="ecommerce-4" src="https://user-images.githubusercontent.com/38366630/166820731-b71d923b-724a-47d1-b265-ba3d4f3b9c64.png">

#### Cart Functionality 
<img width="400" alt="ecommerce-5" src="https://user-images.githubusercontent.com/38366630/166820744-44106ecf-c40a-451b-bbde-98292f743a64.png">

#### Checkout Form
<img width="400" alt="ecommerce-6" src="https://user-images.githubusercontent.com/38366630/166820751-5a7349c8-ca85-43ad-9b33-e91e6f70225a.png">

#### Order Form
<img width="400" alt="ecommerce-7" src="https://user-images.githubusercontent.com/38366630/166820760-a6ae982d-97f3-4a29-b373-5338badce4d2.png">

<!-- If you have screenshots you'd like to share, include them here. -->


## Setup
Make sure to have Python, Django, and Heroku installed on your operating system.
Clone this repository.
`git clone https://github.com/garcia116/ecommerce-django.git`

Decide upon a directory, create a virtual environment and activate it.

On the project directory, install the requirements.txt file.
`pip install requirements.txt`

Create a new AWS S3 bucket. Inside the bucket, create a media folder and a static folder.

Create a new Heroku app.
`Heroku create example`

On the project directory, go to the file named '.env.sample'. Copy its content and create a new '.env' file. Paste the content onto the file and fill in all the required secrety keys and passwords from Django, AWS S3, and Heroku.

On your Heroku Dashboard, add onto the 'Config Vars' all the data that is in your .env file. This will ensure that all your key-values will get passed on to Heroku. 

Run migrations to update/create database on Heroku.
`python manage.py makemigrations`
`python manage.py migrate`

Finally, on the project directory shell, add, commit, and push to your heroku project.
`git add -a`
`git commit -m "migrations"`
`git push heroku main`


## Usage
On the project directory shell, run the local server to view the project.
`python manage.py runserver`
Navigate to to http://127.0.0.1:8000

Alternatively, in your shell deploy the project on Heroku to view it.
`heroku deploy`


## Room for Improvement

Room for improvement:
- Enhancing the mobile device UI by making changes to the navbar and toggler
- Having the product gallery to be responsive. For example, when the user selects a product color variation, the product image should change to the color variation selected to allow the user to see their product selection.

To do:
- Adding the price range search function
- Adding a filter search function to the store catalog


## Acknowledgements
- This project was based on [this tutorial](https://www.udemy.com/course/django-ecommerce-project-based-course-python-django-web-development).
- Many thanks to Rathan Kumar.

<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->
