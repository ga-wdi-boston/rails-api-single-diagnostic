# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
resources :books, only: [:index]
get '/books' => 'books#index'
```

In what file does the above code go?

```md
routes.rb
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
Runs your latest migration file
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
`rails g scaffold things`: Generates the whole MVS structure for a single resource.
`rails g controller things`: Creates a new controller for 'things' resource
```

What is the job of the `serializer`?

```md
Filters info coming from the API, and display into browser. For example, it filters out password information so that will not be displayed on the client side.
```

What do we expect the command `Patient.all` to return?

```md
All instances of the Patient class that you have defined. In other words, all our data of patients in our patients table.
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
Patient model
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
Since ApplicationRecords won't let you access the properties in model files, you can check in schema to see the properties of a table.
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
Opens a REPL that pre-loads the API
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
Opens your database client and loads the correct database.
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
JSON
```
