# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb


get '/books/:id', to: 'books#show'

Or

get '/books/:id' => 'books#show'

```

In what file does the above code go?

```md
in the routes.rb file

```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
Bundle exec rake is a bundler command that will excecute the script db:migrate and when db:migrate migrates the data in the database.

```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
the scaffold command generates routes, a controller and model for things. rails g controller generates just makes the  controller for things.

```

What is the job of the `serializer`?

```md


```

What do we expect the command `Patient.all` to return?

```md
all the patient in the db

```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md

in the model

```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md


```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md

it allows us to interact with our rails models in the commandline

```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
It opens the database client and loads the database

```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
JSON

```
