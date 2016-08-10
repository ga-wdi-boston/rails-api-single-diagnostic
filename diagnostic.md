# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What is the purpose of a backend?

```bash
The back end interacts with the database giving you the ability to store and
retreive data.
```

Which layer in the MVC pattern is used by the controller to fetch data?

```bash
the models
```

Which layer in the MVC pattern communicates with the model?

```bash
the controllers
```

Why don't we use views in our interpretation of the MVC pattern?

```bash
We let the front end handle the construction of HTML
```

What does C.R.U.D stand for?

```bash
Create
Read
Update
Destroy
```

In which part of the MVC pattern can we find C.R.U.D actions?

```bash
The controllers
```
List at least 5 standard actions that C.R.U.D corresponds to?

```bash
- Index
- Show
- Update
- Delete
- Create
```

A user action fires a `GET` request for `person/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list)

```bash
- The request hits the router and it decides which conroller is appropriate
- It picks the people controller
- The controller parses the request and tells the model to carry it out
- The person model makes the request to the data base
- The database looks for person with id 1 in the people table and gives it to the model
- The model hands the data off to the controller
- The controller sends the data to the front end to be constructed for viewing
```

What is the command to start an instance of a rails server?

```bash
[bundle exec] rails s[erver]
```

What are the commands to drop, create, migrate and seed a database? (4 bullet
points)

```bash
- dropdb tablename
- createdb tablename
- rails g migration AddThisToTable this:string
- bundle exec rake db:migrate
```

What is the command to scaffold a pet with a name and an age?

```bash
rails g scaffold pet name:string age:integer
```

List two advantages of using serializers? (2 bullet points)

```bash
- You can hide information from the users of your app
- You can choose levels of access to be different for admins
```
