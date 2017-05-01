# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
get '/books/:id' => 'books#show'
resources :books, only: [:show]
```

In what file does the above code go?

```md
config/routes.rb
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
runs all the migration files that are newer than the schema.  they will modify
the schema and reset the version number of the schema to the last migration
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
rails g scaffold things will create a route, a model (including a database table),
a migration, a controller and a serializer for things

rails g controller things will create a route and a controller for things.
```

What is the job of the `serializer`?

```md
to massage the data coming out from the model before sending it back to the web server
```

What do we expect the command `Patient.all` to return?

```md
all the Patient records
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
in the model - models/patient.rb - it is a class that inherits from ApplicationRecord
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
the magic of rails!  it's magic, right?  the magic comes from ApplicationRecord
which model inherits from
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
opens a console interface to the database you are using
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
the same thing as rails dbconsole
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
the response object?
```
