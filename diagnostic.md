# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
resources :books only: [:show]

# OR

get '/books/:id' => 'books#show' # This is my best guess for the second method, based on how the default user actions are defined
```

In what file does the above code go?

```md
The above would go in the `config/routes.rb` file
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
This command executes all migrations defined in the `db/migrate` directory, in the order they are stored in that directory. These files define a number of actions for rails to perform on the database, typically creating and modifying the relational database tables required by the app.
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
The scaffold command will generate all of the necessary files to handle a resource called `things`, namely controller, model, migration and serializer, whereas the controller command will only generate the file and framework for ThingsController. Additionally, a controller generated via scaffold will come with the index, show, create, update and destroy actions predefined whereas a controller generated from the controller command will be empty and these actions will need to be defined manually.
```

What is the job of the `serializer`?

```md
The serializer is the rails replacement for the view layer of the standard MVC model, which is to say that it handles the translation of data returned from the database into json that can be returned to the client.
```

What do we expect the command `Patient.all` to return?

```md
We expect this command to return an array of all entries in the `patients` table formatted as Patient objects.
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
The constant Patient is a model object defined in `app/models/patient.rb`
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
While the specific model objects have very little, if anything, defined in their files, they all inherit from the rails class called ApplicationRecord, in which most of the standard methods used to interact with the database are defined.
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
This command will open the rails console, which is essentially a REPL for rails APIs, allowing us to manually test the functionality of certain parts of the API.
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
This command will open the database being used by the app. In the case of the apps we are programming at GA, this means a specific Postgres database, but rails is generally database agnostic, so any number of other SQL databases could also work.
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
An API should return a JSON (javascript object notation) string to the client, at least in the APIs we have been writing.
```
