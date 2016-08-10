# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What is the purpose of a backend?

```bash
The purpose of a backend is to store data in a database for usage in a front end
environment.
```

Which layer in the MVC pattern is used by the controller to fetch data?

```bash
The model layer fetches data as requested by the controller.
```

Which layer in the MVC pattern communicates with the model?

```bash
The controller communicates with the model
```

Why don't we use views in our interpretation of the MVC pattern?

```bash
Views were used when the webpage was displaying information directly from the
database, while now the information is displayed directly by the front end.
```

What does C.R.U.D stand for?

```bash
Create Read Update Destroy
```

In which part of the MVC pattern can we find C.R.U.D actions?

```bash
They take place in the database/server.
```
List at least 5 standard actions that C.R.U.D corresponds to?

```bash
Creating a new entry, reading from all entries, reading from 1 entry, updating
an entry and destroying an entry.
```

A user action fires a `GET` request for `person/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list)

```bash
1. The user actio is used by a router to find the correct controller for a GET
    request of 1 person by ID.
2. The controller finds the correct model used for finding a person and requests
    that the model fetch the person data from the database.
3. The model finds the data for person/1 in the database, if present.
4. The model returns to the controller with the data for person/1, or an error if
    person1 does not exist.
5. The controller now has the information and sends it back to the user to be viewed.
```

What is the command to start an instance of a rails server?

```bash
bundle exec rails server
```

What are the commands to drop, create, migrate and seed a database? (3 bullet
points)

```bash
- create => rails g scaffold model key:type key:type key:type
- migrate => rails g migration AddName keys:string
- seed => bundle exec rake db:migrate
- drop => rake db:rollback
```

What is the command to scaffold a pet with a name and an age?

```bash
rails g scaffold pet name:string age:integer
```

List two advantages of using serializers? (2 bullet points)

```bash
// your response here
```
