# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
resources :books, only: [:show]
resources :books, except: [:new, :edit]
```

In what file does the above code go?

```md
routes.rb
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
Executes the rake script with the command of db:migrate which will change the
database.
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
scaffold will generate controller, model, and serializer, whereas controller will
only generate controller.
```

What is the job of the `serializer`?

```md
The view/output
```

What do we expect the command `Patient.all` to return?

```md
All of the rows and columns in the table patient.
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
// your response here
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
Because the class inside model inherits from the Activemodel
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
It drops you into the rails command line interface.
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
It also drops you into the rails command line interface.
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
json
```
