# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
get '/books/4' => 'books#show'
resources :books/4, only: [:show]

```

In what file does the above code go?

```md
config/routes.rb
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
It makes rails run a migration, which means it updates the server with the latest
data and routes.
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
A scaffold generates the boilerplate necessary to add a table; the model, the views,
and the controller and migration are all included. When you generate a controller you're
only generating the means to controll the routes of a new table. This is just one part
of what the scaffold does.
```

What is the job of the `serializer`?

```md
// your response here
```

What do we expect the command `Patient.all` to return?

```md
Patient.all will return all separate instances of patients.
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
// your response here
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
They inherit from Application Record.
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
It opens up the pry command line.
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
The same thing?
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
JSON
```
