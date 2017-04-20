# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
index or show using the URL/books/4
```

In what file does the above code go?

```md
controller script
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
it migrates the rails api to
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
Scaffold will generate the entire rails database structure.  Controller only the controller files.
```

What is the job of the `serializer`?

```md
Serializers replace all the views.
```

What do we expect the command `Patient.all` to return?

```md
Return all the instances of the class Patient.
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
In the model file.
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
When we db:migrate rails is migrating the database structure used for a model.   Rails is in the background supporting the models.
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
It helps us in testing by opening a REPL that loads the API.
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
Opens the database client and loads correct database
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
JSON
```
