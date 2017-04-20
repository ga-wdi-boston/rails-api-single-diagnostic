# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
get '/books/:id' => 'books#show'
resources :books, only: [:show]
```

In what file does the above code go?

```md
config/routes.rb
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
It runs the scripts found in db/migrate. These scripts will create the database
tables
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
rails g scaffold things creates a db migration file for things. rails g controller things
creates a controller file for things
```

What is the job of the `serializer`?

```md
Not sure - but I think this is what creates the JSON response which is sent
back to the client for a given request
```

What do we expect the command `Patient.all` to return?

```md
This will return every Patient, or every row in the patient table.
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
In the Patient model.
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
The model functionality is inherited from the super class of ApplicationRecord
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
Opens pry with the api completed loaded, so all of the controllers and models
are available.
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
Opens psql and connects to the database for the rails app.
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
JSON
```
