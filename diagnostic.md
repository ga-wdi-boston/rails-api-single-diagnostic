# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
resources :books, only: %i[show]
# - or -
get '/books/:id' => 'books#show'
```

In what file does the above code go?

```md
config/routes.rb
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
bundle exec calls the Ruby bundler to execute the rake script for db:migrate,
which calls the migrations in db/migrate necessary to update the database and
its schemas to the latest configuration in the local repo.
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
rails g controller things generates a Rails controller for the Things object.
rails g scaffold things generates all of the resources needed for Things,
including model, routes, controller, and migrations.
```

What is the job of the `serializer`?

```md
The job of the serializer is to filter data being returned by the model before
sending it back to the client to be rendered.
```

What do we expect the command `Patient.all` to return?

```md
Patient.all is a class method on Patient that returns an array of all objects
of the Patient class in the database.
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
Patient is defined in the patient model (patient.rb)
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
Models inherit most of their functionality from the `ApplicationRecord` class.
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
`bin/rails dbconsole` opens the psql terminal window automatically connected to
the current applicaiton database.
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
`rails db` opens the psql terminal window automatically connected to
the current applicaiton database. (same as `bin/rails dbconsole`)
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
Our response from ther server will be coming back as a JSON string.
```
