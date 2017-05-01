# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
get '/books/4' => 'books#show'
resources :books, only: [:show]
```

In what file does the above code go?

```md
config/routes.rb
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
Prior to running this code you have created a migration that will alter the database in some way.  The above code will execute the migration so that the database will actually be changed and the schema updated.
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
The generate scaffold command is a superset of the generate controller command.  Generate scaffolding will generate a model file with some specs, a route, some serializers, and a migration in addition to a controller.
```

What is the job of the `serializer`?

```md
It allows us to customize the output that rails sends as JSON from our server.  It's taking the place of the View in the MVC paradigm.
```

What do we expect the command `Patient.all` to return?

```md
Every instance that has been created off of the class Patient.
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
The Model.
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
Becuase they are inheriting hundreds of class and instance methods from Application Record and Object.
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
Figures out which database you're using and drops you into whichever command line interface you would use with it.
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
Same as previous question I believe
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
JSON.
```
