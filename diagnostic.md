# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
index and show
```

In what file does the above code go?

```md
routes.rb
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
The command setups the rails db with any newly define tables.
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
  The first creates the data model for things, while the second creates
  a new controller called Things
```

What is the job of the `serializer`?

```md
provides a way of creating custom JSON by representing each resource as a class
```

What do we expect the command `Patient.all` to return?

```md
All the patients in the patients table.
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
app/models/patient.rb
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
They inherit functionality from other classes(ApplicationRecord)
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
allows us to inspect the db using db commands
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
opens a psql session.
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
JSON formatted data
```
