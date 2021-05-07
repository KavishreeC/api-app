# Rails Rest API

Rails API-only app using rails 6.

### About

* This is a simple rails api-only app
* This application contains JSON Web Token authentication(JWT)
* Token based authentication(JWT) is used to handle the authentication of user in application
* User can login and get API data

## Getting Started

### Basic Setup

* Ruby version - 3.0.0
* Rails Version - 6.1.3.1
* GitHub

To get started with the app:

* `git clone git@github.com:KavishreeC/Job-portal.git` to clone this repo

* `bundle install` to install all required gems

* Update `database.yml` file

* `rails db:create` to create database

* `rails db:migrate` to make all database migrations

* `rails s` to start the rails server

### Authentication

#### create new user

```
curl -H "Content-Type: application/json" -X POST -d '{"email":"test1@mail.com","password":"123456789"}' http://localhost:3000/authenticate

```

`{"auth_token": <token>}` will be returned.

#### Authenticate user

```
curl -H "Authorization: <token>" http://localhost:3000/users

```



