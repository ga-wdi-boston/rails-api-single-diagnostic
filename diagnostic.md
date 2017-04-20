# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
To get the books/4 you'd need to do the following:
1. Change router to say SHOW in routes.rb
    resources :books, only: [:show]
2. ?
```

In what file does the above code go?

```md
Found in routes.rb
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
bundle exec is a command to execute a script in the context of the current bundle . 

So bundle exec rake db:migrate executes the rake script with the command db:migrate in the context of the current bundle.

In addtion, Active Record tracks which migrations have already been run so all you have to do is update your source and run rake db:migrate. Active Record will work out which migrations should be run.
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
Rails scaffolding is a quick way to generate some of the major pieces of an application. With the scaffold action, Rails generates all the code it needs dynamically.

The rails g controller things  would generate a route for get '/things' 

```

What is the job of the `serializer`?

```md
The job of the serializer is:
Provides a way of creating custom JSON by representing each resource as a class. Serializers describe which attributes and relationships should be serialized.
```

What do we expect the command `Patient.all` to return?

```md
All the rows in the table Patient.
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
In the app/models folder in Patient.rb
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
 Good question. I was wondering the same thing myself! But if I was to guess, I'd say that they inherit quite a bit of heaving lifting from the parent class, ApplicationRecord.
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
rails console opens a REPL that pre-loads the API.

For example:
~/wdi/trainings/rails-api-cookbook-lab$ bin/rails dbconsole
psql (9.6.2)
Type "help" for help.

rails-api-cookbook-lab_development=# \c
You are now connected to database "rails-api-cookbook-lab_development" as user "conor".
rails-api-cookbook-lab_development=#


The dbconsole allows you to run SQL commands from within rails.
It allows us to query the database directly or to test out SQL scripts before embedding them in Ruby code. Also allows you to validate CURL scripts to ensure they did an insert or update etc..

```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
rails db opens your database client and loads the correct database.
This brings up the pSQL command prompt to then connect into the database as follow:
~/wdi/trainings/rails-api-cookbook-lab$ rails db
psql (9.6.2)
Type "help" for help.

rails-api-cookbook-lab_development=# \c
You are now connected to database "rails-api-cookbook-lab_development" as user "conor".
rails-api-cookbook-lab_development=#


After that you can connect and query the database or look at the table sturctures using /d etc
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
Is it JSON?
```
