# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.

What is the purpose of a backend?

```bash
To store and send data
```

Which layer in the MVC pattern is used by the controller to fetch data?

```bash
M, the Model
```

Which layer in the MVC pattern communicates with the model?

```bash
C, the Controller
```

Why don't we use views in our interpretation of the MVC pattern?

```bash
V, views are the new pages after refresing. B/c we are makeing single page
applications we only have one view
```

What does C.R.U.D stand for?

```bash
Create, Read, Updated, Delete
```

In which part of the MVC pattern can we find C.R.U.D actions?

```bash
C, the Controller
```

List at least 5 standard actions that C.R.U.D corresponds to?

```bash
Post, Index, Show, Patch, Destroy
```

A user action fires a `GET` request for `person/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list)

```bash
Client sends request
Router recives request and sends it to the appropriate Controller
Controller recives request and sends it to the appropriate Model
Model checks the request and sends it to the database
Database returns information
Model recives information and sends it to the Controller
Controller recives and sends it to the client.
```

What is the command to start an instance of a rails server?

```bash
rails server
```

What are the commands to drop, create, migrate and seed a database? (4 bullet
points)

```bash
rake db:drop name
rake db:create name
rake db:migrate name
rake db:seed name
```

What is the command to scaffold a pet with a name and an age?

```bash
rails g scaffold pet name:string age:integer
```

List two advantages of using serializers? (2 bullet points)

```bash
hide important information
show necessary information
```
