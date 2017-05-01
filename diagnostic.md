# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
// resources :books, only: [:index]
get '/books', to: 'books#index'
```

In what file does the above code go?

```md
// it goes into a 'config/routes.rb' file
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
// Running the bundle exec rake db:migrate command just ensures that the changes youve made to tyour routes are now applied to your database.
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
// A scaffold controller things file is one that is created from running the 'rails g scaffold things' command.
```

What is the job of the `serializer`?

```md
// Serializers enable us to add attribute keys to an entity
```

What do we expect the command `Patient.all` to return?

```md
// All patients, if this constant is initialized.
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
// 
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
// your response here
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
// This command opens up a REPL in our terminal.
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
// It opens that directories database client, loading the correct database.
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
// JSON
```
