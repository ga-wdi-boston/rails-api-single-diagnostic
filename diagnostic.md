# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What is the purpose of a backend?

```bash
the back end is our database. it stores and serves data as needed
```

Which layer in the MVC pattern is used by the controller to fetch data?

```bash
model
```

Which layer in the MVC pattern communicates with the model?

```bash
controller
```

Why don't we use views in our interpretation of the MVC pattern?

```bash
views is an outdated concept in MVC
```

What does C.R.U.D stand for?

```bash
Create, Read (show & index), Update, Destroy
```

In which part of the MVC pattern can we find C.R.U.D actions?

```bash
the model is what carries out the CRUD actions
```
List at least 5 standard actions that C.R.U.D corresponds to?

```bash
GET INDEX, GET SHOW, POST, PATCH, DESTROY
```

A user action fires a `GET` request for `person/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list)

```bash
1. the route connects to the controller
2. the controller then send the req to the model
3. the model the database to get person if id 1
4. the model then brings that info back to the controller
5. the controller sends that data directly to the client
```

What is the command to start an instance of a rails server?

```bash
rails s
```

What are the commands to drop, create, migrate and seed a database? (3 bullet
points)

```bash
im pretty sure db:nuke_pave does all of those things
drop -  rake db:drop
create - rake db:create
migrate - rake db:migrate
seed - rake db:seed
```

What is the command to scaffold a pet with a name and an age?

```bash
rails g scaffold pet name:string age:date
```

List two advantages of using serializers? (2 bullet points)

```bash
serializers allow us to hide data. it also allows us to show date with correct authorization. e.g. if someone was an admin on a site thay would have access to information the public may not
```
