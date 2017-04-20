# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
curl --include --request GET http://localhost:4741/books/4
```

In what file does the above code go?

```md
.sh file
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
 The command executes a database migration
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
rails g controller things creates a controller, and rails g scaffold things creates
 model, db migration, controller, views and a test suite
```

What is the job of the `serializer`?

```md
To create  text/string representations of objects (encoded using YAML)
```

What do we expect the command `Patient.all` to return?

```md
A list of all patients
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
In the Patient class
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
// your response here
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
figures out which database you’re using and drops you into whichever command line interface you would use with it 
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
// your response here
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
// your response here
```
