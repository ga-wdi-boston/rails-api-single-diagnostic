# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
get '/books/4', to: 'books#show'
get '/books/4' => 'books#show'

```

In what file does the above code go?

```md
routes.rb
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
It prevents executables that don't pull in any gems (that would conflict with your bundle) from cauing issue.
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
When you use rails g controller and specify the method names, the generator only maps specific routes to the routes file.
Scaffolding is a quick way to generate major pieces of an application in a single operation, rather than specific methods.
```

What is the job of the `serializer`?

```md
A serializer is an app that allows us to customize the JSON output rails sends to our server
```

What do we expect the command `Patient.all` to return?

```md
To see a list of all records in table
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
In the model
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
Because they inherit from other classes
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
it allows us to interact with the rails console in that db. Similar to Pry or Node.
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
It is a shortcut to the above command. It immeadiately opens a console in the accurate database.
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
JSON
```
