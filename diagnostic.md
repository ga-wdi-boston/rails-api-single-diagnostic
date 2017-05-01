# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
get '/books/:id' => 'books#index'
resources books, only [:index, :show]
```

In what file does the above code go?

```md
routes.rb
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
It runs your migration files, so if you're creating or editing a new table, once you've done all your editing, you run
the migration to make your changes to the schema.
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
'rails g scaffold things' builds a model
'rails g controller things' builds a controller
```

What is the job of the `serializer`?

```md
it is part of the view and kind of acts as a gatekeeper, in that it has specific items that it will show the user when
requests are made to the database by the controller.  That way, when the user requests information about a patient, the serializer will
filter out certain things the user shouldn't see.
```

What do we expect the command `Patient.all` to return?

```md
Every Patient object
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
in the patient.rb file, in the models directory.
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
model's inherit from other classes and the attributes for the model are in the schema/database.  methods will go in the model files.
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
it allows us to run rails commands and access our database, so we can test the app/database in our terminal
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
seemingly the same thing, drops you into your database
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
TEXT 
```
