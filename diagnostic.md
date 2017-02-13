# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
Rails.application.routes.draw do
  resources :books, only: [:new, :edit]
  resources :books, except: [:new, :edit]
```

In what file does the above code go?

```md
routes.rb
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
it runs a migration on the current database using the budle of gemfiles you have in that file
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
rails g scaffold creates all things accociated with things and rails g controller just creates a controller file
```

What is the job of the `serializer`?

```md
to define the attributes of the information in your table.
```

What do we expect the command `Patient.all` to return?

```md
We expect it to return the Patient hash
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
In the model
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
because the code they do hold is responsible for all the database interaction
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
it finds what db were currently working in and drops us into the db
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
same thing as bin/rails dbconsole
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
json
```
