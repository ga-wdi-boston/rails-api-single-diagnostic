# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
1) `resources :books, only: [:show]`
2) `get '/books/:id' => books:#getbookmethod`

```

In what file does the above code go?

```md
Inside the railes api directory and then config/routes.rb file.
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
Creates tables in a database.
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
rails g scaffold things would create model, views, controller for things and writes to the routes.rb file.

rails g controller things will create controller actions for things such as new, create, update, edit, destory, index, show.
```

What is the job of the `serializer`?

```md
It makes it possible to utilize a custom defined JSON by representing each resource as a class.
```

What do we expect the command `Patient.all` to return?

```md
A full index of patients via a GET requrest.
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
Inside the models/patient.rb file which is the model for the PatientsController.
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
It inherits from the ApplicationRecord class.
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
switches from the OS Shell CLI to the DB CLI
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
switches from the OS Shell CLI to the DB CLI
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
JSON: JavaScript Object Notation
```
