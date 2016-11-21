# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```ruby
Rails.application.routes.draw do
  resources :books, only: [:index, :show]
  get '/books/:id' => 'books#show'
end

```

In what file does the above code go?

```bash
<project_root>/config/routes.rb
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```bash
Bundle exec rake db:migrate applies transformations to the database schema contained
in unapplied migration files (located in <project_root>/db/migrate).
```

What do we call the string rendered from our server?

```bash
The request
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```bash
Rails g scaffold things generates all of the necessary files (including views)
for a new restful resource.  It also adds RESTful routes to config/routes.db.

Rails g controller thigns simply creates a new file with a new controller class.
```

What is the job of the `serializer`?

```bash
The serialized translates model instances to JSON strings that are appropriate
for consumption by the client.
```

What do we expect the command `Patient.all` to return?

```bash
The command should return a list of all patients in the patient table.
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```bash
In the Patient model.  Most likely located at <project_root>/app/models/patient.rb.
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```bash
There are number of things that may explain this.  If we are dealing with simple
RESTful resources, our models inherit much of the needed functionality from the ActiveRecord class.
It may also be the case that much of the model\'s underlying functionality has been abstracted away
to a module and located in a file in the "concerns" directory
```

What does typing `rails console` in a directory that houses a rails app do for
us?

```bash
Rails concsole opens an interactive REPL (in our configuration, pry), that provides
access to the the application instance as well as the applications models and related functionality.
```

What does typing `rails db` in a directory that houses a rails app do for us?

```bash
'Rails db' provides command line access to the database underlying our application
using whichever CLI is supported by our db.
```

What is the specific name for the type of string our data will be coming back
from the server in?

```bash
Response.
```
