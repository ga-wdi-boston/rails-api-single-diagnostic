# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
resources :books, only: [:show]
get '/books/:id', to: 'books#show'
```

In what file does the above code go?

```md
config/routes.rb
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
The command modifies the app's existing database schema by reconciling pending migration files with the schema.rb file.
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
Scaffold creates everything needed for crud operation on a new resource (resource routes, controller, model, serializer). Generating a controller only generates a controller file for a given resource.
```

What is the job of the `serializer`?

```md
The serializer produces JSON based on the resource's model.
```

What do we expect the command `Patient.all` to return?

```md
An active record collection object containing a patient object for every patient record in our app.
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
Patient is defined as a model in the models directory.
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
When using rails our models are inherting from ActiveRecord which provides a lot of functionality, including interactions with a database.
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
It opens a SQL console using the database for the current app.
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
The same thing as above. `db` is an alias for the command `dbconsole`.
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
JSON
```
