# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
resources :books, only: [:show]
resources :books, except: [:new, :edit]
```

In what file does the above code go?

```md
This goes into the routes.rb file.
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
This command looks for migrations created by the user and runs the up code for any migrations that are in the down position.
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
`rails g controller things` will only create an empty controller file for the things model.  `rails g scaffold things` will create a serializer, a controller, a model, routes, and will also populate the CRUD routes for the things controller.
```

What is the job of the `serializer`?

```md
A serializer controls which attributes of the object to return in a GET request, in JSON format.  So far I have used the serializer to prevent the different timestamps from showing up in my requests so that my screen isn't cluttered by them.
```

What do we expect the command `Patient.all` to return?

```md
It will return a hash of all of the patient objects stored in the patients database.
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
Patient is defined in the model file, patient.rb.
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
Most of the things that are happening with the model is defined on ApplicationRecord, from which our models inherit.  Rails allows us to change and manipulate only the things most important to our program and not the bones that make up rails.
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
It allows us to open and view our current database in PSQL(or I guess whichever program we have installed that interprets SQL).  This allows us to quickly check the results of any migrations made and inputs and changes to the database.
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
This does the same thing as bin/rails dbconsole.
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
JSON
```
