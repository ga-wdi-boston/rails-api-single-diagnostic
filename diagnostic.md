# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
resources :books, only: [:index]
resources :books, except: [:new, :edit, :show, :create, :update, :destroy]
```

In what file does the above code go?

```md
config/routes.rb
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
It runs the migrations inside the current bundle
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
`rails g controller things` generates a controller for things, while `rails g scaffold things` generates a model, migration, controller, and views for things.
```

What is the job of the `serializer`?

```md
The serializer formats the response into proper JSON
```

What do we expect the command `Patient.all` to return?

```md
This should return all of the patients in the table
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
It is a model, defined in models/patient.rb
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
Because they inherit from ApplicationRecord
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
It opens a rails console in that directory
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
This also opens a rails console in that directory
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
JSON
```
