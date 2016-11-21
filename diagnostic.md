# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```bash
get '/books/:id', to: 'books#show'
get '/books/:id' => 'books#show'
```

In what file does the above code go?

```bash
routes.rb
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```bash
It executes any code found within the Active Record migration files in db/migrate.
The migrations make it so we dont have to modify our database directly.
```

What do we call the string rendered from our server?

```bash
A response.
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```bash
The first command generates routes, a controller and a model for things.  The second
command just generates a controller.
```

What is the job of the `serializer`?

```bash
The serializer allows you to filter things out of your response.  The data still
exists, its just not shown to users through the respose.
```

What do we expect the command `Patient.all` to return?

```bash
All of the records in the patients table.
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```bash
In the model.
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```bash
The methods making use of the Patient model are defind within the controller.
```

What does typing `rails console` in a directory that houses a rails app do for
us?

```bash
It allows you to use the command line to interract with your rails app.
```

What does typing `rails db` in a directory that houses a rails app do for us?

```bash
It connects you to the database underlying your rails application and allows
you to interact with it using command line.
```

What is the specific name for the type of string our data will be coming back
from the server in?

```bash
JSON
```
