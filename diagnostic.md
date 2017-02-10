# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.

What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
get '/books/:id', to: 'books#show'
get '/books/:id' => 'books#show'
```

In what file does the above code go?

```md
routes.rb
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
It executes any code found within the Active Record migration files in db/migrate. The migrations make it so that we don't have to modify our database directly.
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
The first command generates routes, a controller and model for foo. The second generates just a foo controller.
```

What is the job of the `serializer`?

```md
Th serializer allows you to filter certain data out of your response. The data stil exists, it's just not shown in the response to users.
```

What do we expect the command `Patient.all` to return?

```md
All of the records in the patients table.
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
In the model.
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
The methods making use of the Patient model are defined within the controller.
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
It allows you to use the CLI to interact with your rails app.
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
It connects you to the underlying database in your rails application, and allows you to interact with it using the CLI.
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
JSON
```
