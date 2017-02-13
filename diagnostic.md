# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
// your response here
```

In what file does the above code go?

```md
// your response here
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
db:migrate checks which missing migrations still need to be applied to the database without caring about the previouse ones.
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
when you scaffold you create 3 files controllers model and serializer```

What is the job of the `serializer`?

```md
to show us what type of data to export to json
```

What do we expect the command `Patient.all` to return?

```md
a list of all patients
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
Controller classes inherit from ApplicationController, which is the other file in the controllers folder: application.rb.
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
// your response here
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
open up the console with the data base that we work on. we could test our code there. it opens rails from the command line. ```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
open psql with the database that we work on
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
json
```
