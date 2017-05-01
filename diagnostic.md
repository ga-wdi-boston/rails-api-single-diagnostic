# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
get '/books', to: 'books#index'
resources :books, only: [:index]
```

In what file does the above code go?

```md
routes.rb
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
It activates the migration files you have. It is going to change the schema on of project.
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
Controller is part of what is created with scaffold. Scaffold is going to generate everything you need on the MVC structure. (Model, View and Controller).
```

What is the job of the `serializer`?

```md
To make tables communicate with themselves. The serializer provides the id necessary to find the relationship (one-to-one, one-to-many) between information in 2 different tables.
```

What do we expect the command `Patient.all` to return?

```md
A list of instance objects of Patient class.
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

In the Model.
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
As of now there is no block of code being executed on the Model. The Model is used to execute the code, before sending data back to the controller. If there is no code, it is going to return all the information in the table.
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
It opens a psql environment where the tables of that app are stored.
```

What does typing `rails db` in a directory that houses a rails app do for us?

Same thing as `bin/rails dbconsole`
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
JSON
```
