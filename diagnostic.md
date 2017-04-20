# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
// your response here
resources :books, only: [:index, :show]
resources :books, except: [:new, :edit, :create, :delete, :update]
```

In what file does the above code go?

```md
// your response here
routes.rb
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
// your response here
Does it make a working copy of the table you want to work in? I know it's a step that comes after db:create and before db:seed and db:example.
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
// your response here
The first one creates a model? and the second creates a controller for things.
```

What is the job of the `serializer`?

```md
// your response here
Don't recall learning this in class. Did a quick Google search -- does it have something to do with automatically passing in attributes?
```

What do we expect the command `Patient.all` to return?

```md
// your response here
Grabs all the patients within the Patient database.
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
// your response here
Active Record
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
// your response here
Active Record is simplifying the process and doing all the work.
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
// your response here
I think this puts you in the SQL console environment.
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
// your response here
Shows you the types of commands you can run in rails.
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
// your response here
JSON
```
