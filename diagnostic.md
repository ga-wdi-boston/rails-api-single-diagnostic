# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
def show
  @book = Book.find(4)

  render json: @book
end
```

In what file does the above code go?

```md
app/controllers/books_controller.rb
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
Migrate takes an existing database and applies a change or changes to it.
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
scaffold  will create the model and default routes as well as the controller,
whereas the controller command will only create the controller for things.
```

What is the job of the `serializer`?

```md
The serializer converts data into JSON for the database to read.
```

What do we expect the command `Patient.all` to return?

```md
the full list of the Patients database.
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
The Patient class is defined by the model
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
Rails does the heavy lifting for models behind the scenes where we can't see the code -
almost all of this is inhereted from the ApplicationRecord class that Patient
inherets from.
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
it opens up a command line interface to interact with the database directly via
SQL commands.
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
same as above answer, just in fewer characters because programmers are lazy.
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
json. # we hates the filthy json stringses.
```
