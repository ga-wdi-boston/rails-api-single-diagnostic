# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
In the routes file, write the following code:
resources :entity, only [:index, :show]

OR

GET '/actionORentity' => entityController#method
```

In what file does the above code go?

```md
routes.rb
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
That command makes table changes including creating tables that don't already
or altering the table schema
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
The scaffold tells rails to generate all the boilerplate files like the
controller files and the model files.

The controller command tells rails to generate just the boilerplate controller
files.
```

What is the job of the `serializer`?

```md
To translate object data into a specific format like JSON.
```

What do we expect the command `Patient.all` to return?

```md
All the records in the patients table.
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
Patient is defined as a class in the patient.rb model file.
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
The model in inheriting from an existing object (ApplicationRecord) that has all
the attributes and methods that it needs (for now).
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
This starts up psql console in the database within which our local data is stored.
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
This executes db commands such as db:drop db:create db:migrate db:seed
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
JSON
```
