# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```bash
curl request or AJAX call
```

In what file does the above code go?

```bash
Routes files.
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```bash
Prepares your database to be set up properly based on any changes you make
from a data-structure standpoint. (i.e. you add a coloumn to the table, when
you do db:migrate then your database should show that new column so you can then
  pass acutal info to the db and it will understand what to do with it.)
```

What do we call the string rendered from our server?

```bash
not entirely sure.
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```bash
Not entirely sure. Scaffold gives us a template?
```

What is the job of the `serializer`?

```bash
to filter what can be viewed / modified on a data object.
```

What do we expect the command `Patient.all` to return?

```bash
all patients.
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```bash
Defined as a class in models file.
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```bash
They inherit from the ActiveRecord.
```

What does typing `rails console` in a directory that houses a rails app do for
us?

```bash
Drops us into the console within our app and allows us to look at our database
(I think!)
```

What does typing `rails db` in a directory that houses a rails app do for us?

```bash
drops us into the db within that rails app rather than ALL databases.
```

What is the specific name for the type of string our data will be coming back
from the server in?

```bash
JSON?
```
