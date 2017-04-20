# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
get '/books', to: 'books#index'
```

In what file does the above code go?

```md
routes.rb
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
It executes code within our directory, bringing in data.
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
the first generates a route, controller, and views. the second just generates a controller.
```

What is the job of the `serializer`?

```md
the serializer filters out data.
```

What do we expect the command `Patient.all` to return?

```md
return all the data from Patient
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
in the model
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
because they are actually defined in the controller
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
lets you to use the terminal to test your code
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
lets you connect to the database
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
JSON
```
