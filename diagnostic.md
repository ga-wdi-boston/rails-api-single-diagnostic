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
It allows you to make changes to database schema i.e. It determines how to turn a ruby model into columns and rows in the database
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
'rails g scaffold' sets up the model, database migration, controller, and views-it give you everything. 'rails g controller' creates just the controller and its views.
```

What is the job of the `serializer`?

```md
helps the developer build JSON objects
```

What do we expect the command `Patient.all` to return?

```md
returns all records from Patient table
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
patient.rb
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
Because they get most of their functionality from Application Record
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
loads the database into memory and allows you to interact with it through the command line interface
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
rails db is short for rails dbconsole, which loads the database into memory and allows user to interact with it through the command line interface
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
JSON
```
