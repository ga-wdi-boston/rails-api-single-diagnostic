# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
resources :books, except: [:new, :edit]
resources :books, only: [:index, :show]
```

In what file does the above code go?

```md
routes.rb
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
It looks to see which migrations are pending and still need to be applied to the database and adds them. It ignores migrations that have already been completed.
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
'rails g controller things' generates only a controller of things. 'rails g scaffold things' generates a model, database migration for the model, controller, views and a test suite for the model.
```

What is the job of the `serializer`?

```md
It controls the way that the JSON response is formatted when coming back to the client.
```

What do we expect the command `Patient.all` to return?

```md
all the patients in the database
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
The model
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
Because it inherits from the Active Record :: Base which gives it additional
functionality.
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
It places you in to the command line interface associated with whatever directory or database you are using.
This could include a SQL command line interface.
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
It sends us into a SQL environment where we can interact with the database.
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
JSON
```
