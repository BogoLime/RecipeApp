<h1 align="center">
  <br>
  <a href="https://recipe-app-2022.herokuapp.com/#467"><img src="https://res.cloudinary.com/dawb3psft/image/upload/v1647878417/Portfolio/logo.png" alt="RecipeAPP" width="300"></a>
</h1>

<h4 align="center">Personal Project - Creating a Frontend JS App </h4>

<p align="center">
  <a href="https://img.shields.io/badge/Made%20with-JavaScript-yellow"><img src="https://img.shields.io/badge/Made%20with-JavaScript-yellow"></a>
  <a href="https://img.shields.io/badge/Made%20with-Python-blue">
    <img src="https://img.shields.io/badge/Made%20with-Python-blue"
         alt="Gitter">
  </a>
  <a href="https://img.shields.io/tokei/lines/github/Bogo56/RecipeApp">
      <img src="https://img.shields.io/tokei/lines/github/Bogo56/RecipeApp">
  </a>
  <a href="https://img.shields.io/github/languages/count/Bogo56/RecipeApp?color=f">
    <img src="https://img.shields.io/github/languages/count/Bogo56/RecipeApp?color=f">
  </a>
  <a href="https://badgen.net/github/commits/Bogo56/RecipeApp">
    <img src="https://badgen.net/github/commits/Bogo56/RecipeApp">
  </a>
</p>

<p align="center">
  <a href="#about-the-project">About The Project</a> •
  <a href="#check-out-the-project">Check out the Project</a> •
  <a href="#about-the-api">About the API</a> 
</p>

## Built With
###  Languages
<p>
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white">
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white">
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white">
<p>
  
### Frameworks
<p>
<img src="https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white">
</p>

### Databases
<p>
<img src="https://img.shields.io/badge/SQLite-07405E?style=for-the-badge&logo=sqlite&logoColor=white">
</p>

### Additional Libraries and Technologies
<p>
  <img src="https://img.shields.io/badge/Heroku-430098?style=for-the-badge&logo=heroku&logoColor=white">
  <img src="https://img.shields.io/badge/OS-Ubuntu-orange?style=for-the-badge">
   <img src="https://img.shields.io/badge/Security-JWT-green?style=for-the-badge">
  <img src="https://img.shields.io/badge/Web Scrape-Pandas-blue?style=for-the-badge">
</p>

## About The Project
The main motivation behind this project was to greatly improve my ability in building and working with API's. I have already build a couple of API's in Python(with Flask). 
Since JavaScript(NodeJS) was a relatively new addition in my tech stack, this was a great opportunity to both upgrade my skills in back-end development with Node and 
to enhance my understanding of what a proper API structure is. I really wanted to make this project more authentic, so I decided to do a small website for booking tours in Bulgaria.

The **main focus of this project is the API** - where I have spent about **75%** of my efforts. I also decided to create a simple front-end (vanilla JS, HTML, CSS) that showcases an
example of how the API might be consumed.

Most of the webpages are **rendered server-side - EJS templates**. To improve experience and user notifications I have also included some frontend JS - mainly with form submition and admin menu.

I have **deployed the project on my own Ubuntu 18.04 server**, so you can check it out for yourself. You'll find a link below

## Check out the Project
As I mentioned, I have created an example frontend that uses part of the API's functionality. You can check the project at:
https://bultravel.bogoapps.site/

There are different types of user roles[user,guide,admin], which have different permissions.

You can log **as an user** with:
**USERNAME**: "marto@example.com"
**PASSWORD**: "password"
OR create an account yourself(No spam - promise :D)

You can log in **as an admin** (access to the admin menu) with:
**USERNAME**: "admin@admin.com"
**PASSWORD**: "admin"
* I have restricted the update operations to superadmins(myself) intentionally - to keep it simple 😅.

I'm using **Stripe in TEST mode** - so just type **4242 4242 4242 4242** as payment card.

## About the API
### API Reference
I have used POSTMAN for testing and building the API. I also used it to generate a simple documentation, so you can easily check it's structure. This is the link to the documentation:
https://documenter.getpostman.com/view/16479105/UVsQriWC

### Features
* Standart CRUD operations for creating and modifying Tours, Users, Bookings, Reviews
* Filtering on resources - searching, pagination, less than/greater than, exclude/include fields, sort asc/desc, limit number of results etc.
* Priviliges based on user role - lead-guides and admins can modify tours, only admins can modify users, only users can write reviews etc.
* Forget password functionality. Sends a restoration link on email (expires in 10 min) for password reset.
* Payment with Stripe - e.g receiving webhooks from strype on successfull payment.
