# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
get '/books/4', to: 'books#show'
get '/books/4' => 'books#show'
```

In what file does the above code go?

```md
config/routes.rb
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
This command is used to create and update database tables from staged migration
files.  These staged migration files can be found in the db/migrate directory and
this process assists the developer to not have to update the database directly
using straight SQL.
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
The `rails g scaffold things` command will build a router, controller and a
model of `things`.

The `rails g controller things` command will only build a controller of `things`.
```

What is the job of the `serializer`?

```md
Serializers allow filtering of data within a response that is given back to the
user.
```

What do we expect the command `Patient.all` to return?

```md
The `Patient.all` command will return all database rows from the `patients`
database table.
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
`Patient` is defined within the `Patient` model located in the
app/models/patient.rb file.
````

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
The `Patient` CRUD methods are found in the `Patient` controller located in the
app/controllers/patient_controller.rb file.
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
It allows the developer to use the command line interface.
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
It allows the developer to connect to the database that is being used by the
rails application.  It also allows the developer to use the command line interface.
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
JSON
```
