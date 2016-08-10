# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What is the purpose of a backend?

```bash
store data and send the data back to client
```

Which layer in the MVC pattern is used by the controller to fetch data?

```bash
route
```

Which layer in the MVC pattern communicates with the model?

```bash
controller
```

Why don't we use views in our interpretation of the MVC pattern?

```bash
Becasuse controller can send data directly to client by Json
```

What does C.R.U.D stand for?

```bash
create, read, update, delete
```

In which part of the MVC pattern can we find C.R.U.D actions?

```bash
controller
```
List at least 5 standard actions that C.R.U.D corresponds to?

```bash
create, index, show, update, destroy
```

A user action fires a `GET` request for `person/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list)

```bash
Route get the client request and send it to controller.
Controller ask model to fetch the data.
Model get the data from database and send it back to controller.
Controller send the data by Json to client.
```

What is the command to start an instance of a rails server?

```bash
rails c
```

What are the commands to drop, create, migrate and seed a database? (4 bullet
points)

```bash
rails db:create
rails db:drop
rails db:migrate
rails db:seed
```

What is the command to scaffold a pet with a name and an age?

```bash
rails g scaffold pet name:string age:integer
```

List two advantages of using serializers? (2 bullet points)

```bash
Easy to change Json presentation 
```
