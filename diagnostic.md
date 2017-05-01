# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb

```

In what file does the above code go?

```md

```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
You perform db:migrate on any database when you need to either update or revert that database's scheme to a newer or older version
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
one generates a new scaffold and one generates a new controller
```

What is the job of the `serializer`?

```md
I believe the serializer translates different data structures into a format that can be stored and then reconstructed later.
```

What do we expect the command `Patient.all` to return?

```md
return all patients
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md

```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
I think because they're inheriting a bunch of functionality from a parent that rails provides
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
It figured out what database you're in and then delivers you into the associated command line.
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md

```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
json I believe
```
