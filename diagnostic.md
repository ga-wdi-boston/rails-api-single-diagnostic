# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
// Add a resource to the routes file and a show action for that resource
```

In what file does the above code go?

```md
The routes file
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
// modifies the schema of our DB so that we can add/retreive things from it.
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
/
rails g scaffold thing with create a a full set of boilerplate files- model, db migration, controller and views

rails g controller things will create a thing controller boilerplate file.
```

What is the job of the `serializer`?

```md
// your response here
```

What do we expect the command `Patient.all` to return?

```md
// Returns all the patients in the DB
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
// Application Controller
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
Within the model file, the classes you created are inheriting from Application Record which has the functionality.
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
// switches you to postgresSQL in terminal for the db your using
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
// same answer as previous question
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
// json
```
