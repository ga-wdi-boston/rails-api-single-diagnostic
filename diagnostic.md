# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
get '/books/:id', to: 'books#show'
OR
resources :books, except: [:new, :edit]
```

In what file does the above code go?

```md
routes.rb
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
run all te migration files to modify the database.
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
The first command generates all the files, including controller, model, serilizer, and the migraton, for the things. The second command only generates a controller.
```

What is the job of the `serializer`?

```md
declear the attributes for a table
```

What do we expect the command `Patient.all` to return?

```md
It returns all the rows in patients table.
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
model
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
Because the model class inherits the ApplicationRecord from rail. The methods in model will be called in controllers or in migration to get or modify the tables.
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
Turn on the psql iteractive terminal for the current database in the file.
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
Open up the current data base in the directory in psql interactive terminal.
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
json.
```
