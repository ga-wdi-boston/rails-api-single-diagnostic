# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
long-hand: get '/books/4', to 'books#id'
short-hand: resources :books, only: [:index, :id]
```

In what file does the above code go?

```md
routes.rb
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
It will run whatever migration files are present in time order.
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
The scaffold command will create files for you in the database, including a controller file for things. The controller command simply creates a controller file by appending the one that scaffold created.
```

What is the job of the `serializer`?

```md
They describe which attributes and relationships should be serialized.
```

What do we expect the command `Patient.all` to return?

```md
The data in a patients table.
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
patient.rb
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
The files are inheriting code that will essentially 'model' the data for us. We just have to provide the proper attributes that are defined in the controller.
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
It will open up pry for you to run scripts in that file and test code for the db.
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
It opens up psql in the terminal to interact with the db.
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
json
```
