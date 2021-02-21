# ![alt text](https://assets.breatheco.de/apis/img/images.php?blob&random&cat=icon&tags=breathecode,32) StarWars Blog API

It is recomended to develop this project in conjuntion with the [StartWars Blog Reading List](https://github.com/breatheco-de/exercise-starwars-blog-reading-list), you will eventually integrate both projects and have a fully functional applications with backend and front-end.

Today we are going to build one API to manage a blog (about StartWars), uses on this blog will be able to list planets, list characters and create or remove favorites.

To allow users to do all of this, we must follow these steps:

1. Start by modeling the database: Create a database and the tables needed to store that information, you may have already done this when you did the [StartWars DataModeling project](https://github.com/breatheco-de/exercise-starwars-data-modeling).
2. Build your endpoints using Flask.
3. Constantly test your endpoitns with postman.

## 💻 Installation

Use the [Flask API boilerplate](https://github.com/4GeeksAcademy/flask-rest-hello) to start this project, open it on Gitpod to avoid any local issues in your computer because you will need to have a database installed and python 3.7+ installed (all of that it's already installed on Gitpod).

## 📝 Instructions

Create an API that connects to a database and implements the following Endpoints (very similar to SWAPI.dev or SWAPI.tech):

- `[GET] /people` Get a list of all the people in the database
- `[GET] /people/<int:people_id>` Get a one single people information
- `[GET] /planets` Get a list of all the planets in the database
- `[GET] /planets/<int:planet_id>` Get one single planet information

Aditionally create the following endpoints to allow your StartWars blog to have users and favories:

- `[GET] /users` Get a list of all the blog post users (⚠️ Note: your blog users, this en)
- `[GET] /users/<int:user_id>/favorites` Get all the favorites that belong to the user with the id = `user_id`.
- `[POST] /users/<int:user_id>/favorites` Add a new favorite to the user with the id = `user_id`.
- `[DELETE] /favorite/<int:favorite_id>` Delete favorite with the id = `favorite_id`.

Your current API does not have an authentication system (yet), that is why the only at to create users is directly on the database using the flask admin.

## 📖 Fundamentals

This exercise will make you practice the following fundamentals:

1. Building an RESTful API.
2. Building a database with SQLAlchemy.
3. Database Migrations.

## 😎 Feeling confident?

`+1` Create also an enpoint to add (POST), update (PUT), and delete (DELETE) planets and people, that way all the database information can be manage using the API instead of having to rely on the flask admin to create the plantes and people.