# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
get '/books', to: 'books#index'
resources :books, only: [:index]
```

In what file does the above code go?

```md
routes.rb
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
Creates tables based on the migration files in your project - acts like a template for your DB.
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
`rails g scaffold things` - does a db migration
`rails g controller things` - generates a controller file
```

What is the job of the `serializer`?

```md
Interacts with JSON objects. Make it possible to do object oriented programming with hash driven language.
```

What do we expect the command `Patient.all` to return?

```md
All the patients in a table called Patient
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
from the Patient model
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
They inherit their functionality from ApplicationRecord
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
opens the rails db cosole
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
same things as bin/rails dbconsole - opens the db console
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
JSON
```
