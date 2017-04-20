# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
esources :books, only: [:index, :show]
or
resources :books, except: [:new, :edit]
```

In what file does the above code go?

```md
config/routes.rb
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
we are calling the bundler to execute any/all scripts in db/migrate directory
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
you are generateing a model and generating a controller, respectively
the scaffold will create a model, a controller for that model, as well as default views
```

What is the job of the `serializer`?

```md
the serializer is used to serve up JSON
```

What do we expect the command `Patient.all` to return?

```md
expecting access to all methods within the Patient class
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
I see the class Patients in the model file, but think it is in the Active Record?
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
i don't think we have gotten here yet ...
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
it provides an interface to the API. We can run our curl commands here
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
gives us access to our database
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
the data returned will be in JSON format
```
