# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.

What is the purpose of a backend?

```md
To store and manipulate data for your application.
```

Which layer in the MVC pattern is used by the controller to fetch data?

```md
model
```

Which layer in the MVC pattern communicates with the model?

```md
controller
```

Why don't we use views in our interpretation of the MVC pattern?

```md
Handling views on the front-end allows us to create single page apps as well
as access the same database through multiple apps (web app, desktop app, mobile
app, etc) through the same API.
```

What does C.R.U.D stand for?

```md
Create Read Update Destroy
```

In which part of the MVC pattern can we find C.R.U.D actions?

```md
controller
```

List at least 5 standard actions that C.R.U.D corresponds to?

```md
GET INDEX POST PATCH DELETE
```

A user action fires a `GET` request for `person/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list)

```md
1. GET request reaches router
2. Router sends request to controller
3. Contoller sends request to model
4. Model accesses data in the database
5. Model sends data to client
```

What is the command to start an instance of a rails server?

```bash
rails s
```

What are the commands to drop, create, migrate and seed a database? (4 bullet
points)

```md
* rake db:drop
* rake db:create
* rake db:migrate
* rake db:seed
```

What is the command to scaffold a pet with a name and an age?

```bash
rails g scaffold Pet name:string age:integer
```

List two advantages of using serializers? (2 bullet points)

```md
* control what information is sent to client
* can store data that is useful on the back-end but confidential to those accessing API
```
