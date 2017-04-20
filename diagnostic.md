# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
@books = Book.find(params[4])
```

In what file does the above code go?

```md
In the routes.rb file
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
This command runs migrations that have not been run yet, specifically for new databases or controllers.
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
Scaffolding things creates a resource called things where rails g controller things creates just a controller for things.
```

What is the job of the `serializer`?

```md
The serializer represents each resource as a class, usually rendered in JSON.
```

What do we expect the command `Patient.all` to return?

```md
An object array containing all of the patients objects.
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
Patient is actually defined in the model patient.rb.
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
Most of the logic is defined in the controller, which contains the business logic.
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
This creates a direct link to the rails database we are working with, allowing us to directly write SQL.
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
It is the same as bin/rails dbconsole, just shorthand.  Better for migrations.
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
JSON?  Render?  I have no idea.  This was never explained.
```
