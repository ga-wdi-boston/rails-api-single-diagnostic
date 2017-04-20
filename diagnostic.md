# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
resources :books, only: [:show]
get '/books/4', to: 'books#show'
```

In what file does the above code go?

```md
routes.rb
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
It is a command to execute the db:migrate script in which db is the namespace
and migrate is the name of the task.
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
Scaffold will generate an entire resource - model, view, controller.
Controller will only generate the controller.
```

What is the job of the `serializer`?

```md
It allows you to create custom JSON.
```

What do we expect the command `Patient.all` to return?

```md
It will return all records in the Patient table.
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
In the model.
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
The methods are defined in the controller file.
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
Determines which database you're using and puts you into the appropriate
command line interface to use with the database.
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
It provides information about the database and help resources/guidelines.
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
JSON
```
