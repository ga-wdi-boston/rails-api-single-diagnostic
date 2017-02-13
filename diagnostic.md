# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
With curl and from browser
I were not able to write curl command 
```

In what file does the above code go?

```md
The requests first will be going to routes to see if the resources are defined, Then it will be going to controller, to modals and modals will be looking into database.
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
It executes the scripts in the rake and migrates the database
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
while `rails g controller things` is creating only the controllers, `rails g scaffold things` will be creating routes, controllers and models
```

What is the job of the `serializer`?

```md
It checks if the defined attributes are exists.
```

What do we expect the command `Patient.all` to return?

```md
It will be returning eveytihing related with Patient class. As methods and data
from the database.
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
It is defined in the models.
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
Because aplicataion record does most of the job.
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
It will be getting the terminal in to PostgreSql.
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
It will be getting the terminal in to PostgreSql.
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
json
```
