
`#html` `#css` `#js` `#php`  `#basics`  `#master-in-software-engineering`

# PHP Employee Management v1<!-- omit in toc -->

>This project is part of the Master in Software Development. The objective was to create an application able to manage a json with all the employees from a company.
 ### Main functionality:
- Login and logout with a json file as user storage
-  Controlled user session set to 10 minutes
- Show data from a JSON in a JS Grid
- Pagination of the data configured by the grid
- Employees CRUD Create Read Delete and Update with a json file as employees storage
- Employee page with employee detail
- External web service to get employees images
- Employee avatar through web service images  
- 
## Index <!-- omit in toc -->
- [Where to start?](#where-to-start?)
- [Requirements](#requirements)
- [Install](#install)
- [Deployment](#deployment)
- [Documentation](#documentation)
- [Project structure](#project-structure)
- [Tools and tecnologies used](#tools-and-tecnologies-used)
- [How to use](#how-to-use)
- [Project requirements](#project-requirements)
- [Resources](#resources)

## Where to start?🚀

### Requirements📋

To run this project you need yo have XAMPP installed in your PC (or MUMP in the case of Mac users). For more information about XAMPP visit [their website](https://www.apachefriends.org/es/index.html).

### Install🔧

To clone this repository you have make in terminal:

```
git clone https://github.com/mhfortuna/php-employee-management-v1.git
```
Then you need to copy this folder to `htdocs` or change the server root variable.

## Deployment📦

To open the file explorer just open a browser and go to [localhost](localhost)
You'll have to login, the credentials are:
```
email: admin@assemblerschool.com
pass: 123456
```

## How to use 💻

### Dashboard page
After you have logged in the application you'll see a grid with some of the employees data. From there you can add new employees or delete them. If you double click on an employee you can see more data in a new page called the **employee page**. If you press on the employee icon it will redirect you to the **employee page** too, but this time you'll have a form to create a new employee.

### Employee page
This page renders conditionaly of how you accesed it:
- Case 1 - double click on employee from dashboard:
In this view you will see the available employee data, and you can update any of the fields. It the `id` doesn't exist it will show an error and redirect you to the dashboard.
- Case 3 - Click on the employee icon from dashboard:
In this view you'll see the empty form to create a new employee. There are mandatory fields to fill. When you submit the new employee it will show a modal and redirect you to the dashboard.

## Project structure 📁

```
assets/
resources/
src/
 /library
```

- Assets contains html, css, js & images
- Css just css files.
- Resources folder contains users.json and employees.json
- Src folder contains PHP files which contain HTML or JS
- Src/library folder contains PHP files that contain just PHP



We use some naming conventions when create code files. For instance a file which handles HTTP request we name it as `Controller`.

In the other hand we have also the concept of `Manager` which typically implements an abstraction layer over a storage system, in this case as we are going to work with json files for a while (bear on mind later we refactor it to MySQL and then we will also have a `Model` file) we would need to create on it all functions we need to access the json file.

The user is stored in `resouces/users.json` file there you have an admin user work with it.

The employees are stored `resouces/employees.json` file you have to make a CRUD over this file

## Tools and tecnologies used 🛠️

* PHP
* HTML
* CSS
* JavaScript
* jQuery
* jsGrid
* Bootstrap 

## Project requirements 📏

- All code included comments need to be write in English
- Use a code style like camelCase
- HTML never use inline styles
- It is recommended to divide the tasks into several subtasks so that you can associate each particular step of the construction with a specific commit
- You should try as much as possible that the commits and planned tasks are the same
 - You must create a correctly documented README.md file in the root directory of the project (see guidelines in Resources)

## Resources

- [File system](https://es.wikipedia.org/wiki/Administrador_de_archivos)
- [PHP FileSystem W3C](https://www.w3schools.com/php/php_ref_filesystem.asp)
- [PHP FileSystem Oficial](https://www.php.net/manual/es/book.filesystem.php)
- [README Guidelines Example](https://gist.github.com/PurpleBooth/109311bb0361f32d87a2)
-  [What can PHP do?](https://www.php.net/manual/es/intro-whatcando.php)

-  [Sample guide for README](https://gist.github.com/Villanuevand/6386899f70346d4580c723232524d35a)

-  [XAMPP](https://www.apachefriends.org/es/index.html)

-  [How to install XAMPP on Windows](https://www.youtube.com/watch?v=h6DEDm7C37A)

-  [What is a web server?](https://www.youtube.com/watch?v=Yt1nesKi5Ec)

-  [Web server basics](https://www.youtube.com/watch?v=3VqfpVKvlxQ)
