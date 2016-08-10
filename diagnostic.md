# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What is the purpose of a backend?

```bash
The purpose of the backend is managage and communicate(CRUD) information to and
from the the server, the client and the database. Without the backend the
information which the client displays would just sit there without doing anything
it would not go anywhere, or get stored. It would just sit there or vaish forever
```

Which layer in the MVC pattern is used by the controller to fetch data?

```bash
the model
```

Which layer in the MVC pattern communicates with the model?

```bash
the controller
```

Why don't we use views in our interpretation of the MVC pattern?

```bash
Because it is a single page app so that means that there will only ever be one
view
```

What does C.R.U.D stand for?

```bash
Create Read Update Delete/Destroy
```

In which part of the MVC pattern can we find C.R.U.D actions?

```bash
in the routes
```

List at least 5 standard actions that C.R.U.D corresponds to?

```bash
new - creates new, but does not save it to the database
Create creates something new and saves it to the database
Destroy deletes something that was on the database
index shows what is on the database
update changes the thing you want to update
```

A user action fires a `GET` request for `person/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list)

```bash

The client sends a request
This request is asking to retrieve information.
This request comes from the controller.
The controller goes to the model, which is holding all the information
The controller then goes to the database where the information is stored
The database checks to see if the information is there
If the information is there it goes back to the model to give the information
The model then goes to the controller
The controller can then send the information to the client
```

What is the command to start an instance of a rails server?

```bash
rails s
```

What are the commands to drop, create, migrate and seed a database? (3 bullet
points)

```bash
bundle exec rake db:nuke_pave
rails g scaffold patient object1:string object2:string object3:integer
bundle exec rake db:migrate
bundle exec rake db:seed
```

What is the command to scaffold a pet with a name and an age?

```bash
rails g scaffold pet name:string age:integer
```

List two advantages of using serializers? (2 bullet points)

```bash
// your response here
```
