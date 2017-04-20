# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
resources :books, only: [:index]
get '/books', to: 'books#index'
```

In what file does the above code go?

```md
config/routes.rb
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
It migrates and changes that have been made to the database.
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
Generating a controller only generates the model, whereas the scaffold creates
much more preconfigured for you (controllers, views, etc.)```

What is the job of the `serializer`?

```md
Provides us a way to render custom JSON.
```

What do we expect the command `Patient.all` to return?

```md
All patients within a given table
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
In the Patient model.
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
They inherit most of their attributes from the ActiveRecord```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
Figures out your working database and drops you into that command line.
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
Shorthand for above?
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
JSON
```
