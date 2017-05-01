# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
resources :books, only: [:show]
or
get ‘/books/:id‘, to: ‘books#show’
```

In what file does the above code go?

```md
routes.rb in the config folder
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
Migrations which have not been run previously will be run, updating the schema.
This only runs migrations in the development environment.
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
'rails g scaffold things' generates a full set -- a migration file, a model,
specs, a route, serializer, a controller, and controller specs. Whereas
'rails g controller things' generates a controller file, a view file, tests,
a JS file, and a stylesheet file. 
```

What is the job of the `serializer`?

```md
Serializer is a file that allows us to customize the output that rails sends as JSON from our server. It essentially filters what's being displayed on the browser.
```

What do we expect the command `Patient.all` to return?

```md
All patient objects, including id and whatever key value pairs we have stored.
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
It is defined in the model -- the patient.rb file in the models folder.
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
The model inherits methods from the class ApplicationRecord, allowing us to
use methods defined in that class.
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
It pre-loads the API and gives us an environment to run Ruby on Rails code.
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
Loads an environment where you can type PSQL commands.
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
JSON
```
