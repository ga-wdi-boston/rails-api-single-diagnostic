# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
resources :books, only: [:index]
get '/books/' => '#id'
```

In what file does the above code go?

```md
routes.rb
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
For the command above, db is a namespace and migrate is the task being defined.  Essentially, the command executes the rake script with the db:migrate being the context of the bundle
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
rails g scaffold things uses the scaffold generator in rails.  It generates migrations, models, views, controllers, unit tests, and helpers (among other things).  The rails g controller things, on the other hand, would only generate a controller (i.e. only one part of the scaffold command)
```

What is the job of the `serializer`?

```md
The serializer is a method for creating custom JSON where each resource is represented as a class.
```

What do we expect the command `Patient.all` to return?

```md
It will retrieve everything listed in the patient column of our database
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
Patient will actually be defined in a model
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
Because they inherit from the ApplicationRecord
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
It allows us to test out our code.
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
It opens the database associated with our rails app.
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
JSON
```
