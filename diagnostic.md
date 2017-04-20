# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
get '/books/:id', to: 'books#show'
resources :books, only: [:show]
```

In what file does the above code go?

```md
routes.rb
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
Migrations are used to update schemas or the data in a database itself. Running db:migrate applies the changes.
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
'rails g scaffold' generates a model file/directory, a migratio file/directory and a controller file/directory. In other words, a full set of model, database migration for that model, controller to manipulate it, views to view and manipulate the data, and a test suite for each of the above.
'rails g controller' generates a singler controller, specifically.
```

What is the job of the `serializer`?

```md
Converts a response to JSON format.
```

What do we expect the command `Patient.all` to return?

```md
All instances of Patient class.
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
Patient class, within the Model.
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
Patient inherits from the ApplicationRecord class which contains most of the methods used. We don't need to define them again in Patient.
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
Opens a SQL environment to view the database tables, query etc.
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
Same as bin/rails dbconsole. Opens a SQL environment to view the database tables, query etc.
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
JSON
```
