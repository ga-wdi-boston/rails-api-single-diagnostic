# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
you can look at the your scripts examples or go into your migrate folder
```

In what file does the above code go?

```md
you need need to go into routes.rb and controllers
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
So bundle exec rake db:migrate executes the rake script with the command db:migrate
in the context of the current bundle.
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md

The Scaffold name needds to be:
lower_snake_case
SINGULAR

The controller name needs to be:
UpperCamelCase
PLURALIZED

```

What is the job of the `serializer`?

```md
it gives us a better way of testing compared to other methods. It can also be
tested in isolation regardless of how the data retrieval is done in the controller.
```

What do we expect the command `Patient.all` to return?

```md
to show all patients in the db
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
Application controller
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
because it inheritance from the applicaiton record
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
rails dbconsole figures out which database you're using and drops you into
whichever command line interface you would use with it
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
its the short hand of dbconsole
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
json
```
