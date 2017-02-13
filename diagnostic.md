# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
get 'books/:id' to: 'books#show'
get 'books/:id' => 'books#show'

```

In what file does the above code go?

```md
config/routes.rb
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
this command will migrate all changes applied to our current tables. These changes can include new columns, rows, or any other edited information. Migrations are good because it allows us to keep our tables flexible over time.
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
rails g scaffold things will create all necessary files for us including the controller, router, serializer, and models while the second command will only create the controller for us.
```

What is the job of the `serializer`?

```md
The job of the serializer is to serialize ActiveModel/ActiveRecord
objects into JSON or XML (JSON in our case)
```

What do we expect the command `Patient.all` to return?

```md
We expect this command to return information stored in our Patient model.
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
Patient is actually defined in our model file
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
most of the code to access data from the database is actually behind the scenes, although the developer must code the actions associated with the model including show, index, create, update, and destroy
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
allows us to access the console for our databases in rails.
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
brings us into our database using SQL
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
JSON
```
