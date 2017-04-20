# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.

What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
resources :books, only: [:index, :show]
resources :books, except: [:view, :new]
```

In what file does the above code go?

```md
routes.rb
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
Runs all the migrate files that have been created since the last version, basically updating the database
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
* scaffold creates the model, view, and controller
* controller just creates the controller
```

What is the job of the `serializer`?

```md
To convert objects into text/string format so they can be saved to the database easily
```

What do we expect the command `Patient.all` to return?

```md
An array of Patient objects
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
In the Patient model
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
They inherit from pre-defined Rails classes, specifically ActiveRecord
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
It gives us a command line interface to interact with our database
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
The same thing as rails dbconsole
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
JSON
```
