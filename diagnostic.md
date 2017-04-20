# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
resources :books, only: [:index, :show]
resources :books, except: [:edit, :view, :destroy, :update, :create]
```

In what file does the above code go?

```md
routes.rb
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
It configures the database that you created to the specifics that you hold in your
migrate file. i.e what columns and what type of data fields it should have.
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
Scaffold gives you all of the MVC components whereas controller would just give you
the controller.
```

What is the job of the `serializer`?

```md
It translates the data from the db into a specific model that can be stored as a representation
of the actual data.
```

What do we expect the command `Patient.all` to return?

```md
all of the patients
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
It is a class within the model. On the model.
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
Because rails does all the work for us. We inherit the rails class and use the methods there.
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
It drops us into a postgres enviornment hooked up to our rails API
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
the same thing.
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
JSON
```
