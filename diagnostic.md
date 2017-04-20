# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
•by adding show in a resources only line of code

```

In what file does the above code go?

```md
in the routes file
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
tells rails which db to migrate (pull data) from
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
// your response here
```

What is the job of the `serializer`?

```md
to format JSON
```

What do we expect the command `Patient.all` to return?

```md
all instances of the class Patient
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
in the patient.rb file (in models directory)
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
most of the code goes in the controller so that model stays lean (and mean)
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
// your response here
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
invokes the rails db in that directory
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
JSON
```
