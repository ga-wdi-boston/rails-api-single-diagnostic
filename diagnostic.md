# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
get '/books', to: 'books#index'
resources :books, only: [:index]
```

In what file does the above code go?

```md
config/routes.rb
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
this command updates the migrate files and runs them. Once this command is fired, the app can go live, but the migration files become immutable, and any changes require essentially starting from scratch.
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
rails scaffold creates the entire file architechture for a single resource, including routes, controllers and models. Generate controller has fairly similar functionality, but it works on a smaller scale, generating only the controller, rather than a fully functional file system.
```

What is the job of the `serializer`?

```md
Serializers mutate the JSon which is sent to and recieved from the server in a specified manner.
```

What do we expect the command `Patient.all` to return?

```md
A list of all instantiated patient objects in the working directory
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
In the patient model file
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
They are lacking code partially because they are inheriting all the functionality of the ApplicationRecord class and partially because we are going to define most of their custom functionality.
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
Opens up a rails console which allows you to access the working database
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
Basically the same as above
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
JSON? Honestly not at all sure about this one.
```
