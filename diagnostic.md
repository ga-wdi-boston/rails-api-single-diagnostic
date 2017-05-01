# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
// your response here
1)using the scaffolding method where it can create it automatically along with controllers, models etc
2)doing it manually by writing the syntax in routes file using resources :books, only [:index, :show]

```

In what file does the above code go?

```md
// your response here
in the routes file
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
// your response here
bundle exec is a Bundler command that runs a script in context of the current bundle. Altogether, it
executes the rake script with the command db:migrate in the context of the current bundle
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
// your response here
```

What is the job of the `serializer`?

```md
// your response here
The serializer converts an abstract datatype to something that is read/writtable
```

What do we expect the command `Patient.all` to return?

```md
// your response here
the command returns all the instances of Patient
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
// your response here
in the schema
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
// your response here
The model is
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
// your response here
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
// your response here
it figures out which database you're using 
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
// your response here
```
