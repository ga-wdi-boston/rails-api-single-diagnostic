# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
get '/books/:id' => 'users#show'
resources :books, only: [:index]
```

In what file does the above code go?

```md
routes.rb
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
Selects the version of rake thats specified in the gem file
for the project. Then applies our latest migration(s)
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
Scaffold sets up the model, view and controller files for a table.
Controller only generates the controller for a table
```

What is the job of the `serializer`?

```md
To Format or change the Json that the API is sending to represent a resource.
```

What do we expect the command `Patient.all` to return?

```md
display all of the patients in the patients table
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
patient.rb
Patient Model
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
They are inheriting from ApplicationRecord
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
Figures out which database where using and opens the command line interface we can use with it. In our case its psql.
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
In the clicnic-code-along directy it told me I am in psql (9.6.2) and dropped me
into the psql command line.
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
 a Query string?
```
