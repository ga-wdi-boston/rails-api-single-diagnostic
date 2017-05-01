# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
get '/books/:id' to: 'books#show'

resources :books, only: [:show]


```

In what file does the above code go?

```md
config/routes.rb
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
It executes the rake script to run db migrations that haven't ran yet and are queued.
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
g scaffold sets up a model, db migration, controller, view, and test suite.

g controller would just generate a controller.
```

What is the job of the `serializer`?

```md
creating custom json
```

What do we expect the command `Patient.all` to return?

```md
all patients
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
patient_spec.rb
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
They inherit from Application Record so they many things from it you don't see in the model.
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
Opens the console for the database for that app.
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
Also opens the console for the database for that app
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
JSON
```
