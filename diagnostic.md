# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```bash
The purpose of a backend is to store data in a database for usage in a front end
environment.
```

In what file does the above code go?

```bash
The model layer fetches data as requested by the controller.
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```bash
The controller communicates with the model
```

What do we call the string rendered from our server?

```bash
Views were used when the webpage was displaying information directly from the
database, while now the information is displayed directly by the front end.
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```bash
Create Read Update Destroy
```

What is the job of the `serializer`?

```bash
They take place in the database/server.
```

What do we expect the command `Patient.all` to return?

```bash
Creating a new entry, reading from all entries, reading from 1 entry, updating
an entry and destroying an entry.
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

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

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```bash
bundle exec rails server
```

What does typing `rails console` in a directory that houses a rails app do for
us?

```bash
- create => rails g scaffold model key:type key:type key:type
- migrate => rails g migration AddName keys:string
- seed => bundle exec rake db:migrate
- drop => rake db:rollback
```

What does typing `rails db` in a directory that houses a rails app do for us?

```bash
rails g scaffold pet name:string age:integer
```

What is the specific name for the type of string our data will be coming back
from the server in?

```bash
// your response here
```
