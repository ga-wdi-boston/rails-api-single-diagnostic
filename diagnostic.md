# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
resources :books, only: [:show]
post '/books/4' => 'books#show'
```

In what file does the above code go?

```md
In the routes.rb folder file in the config folder```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
It runs that latest migration or migrations to update the database.

```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
rails generate scaffold thing will generate the entire scaffold, including the thing's controller, for the object things.  rails genrerate controller things will only generate the things controller
```

What is the job of the `serializer`?

```md
The serializer controls what attributes are displayed when data from an object is shown.
```

What do we expect the command `Patient.all` to return?

```md
Patinent.all will return all instances of the Patients class.  It should be an array of hashes with whatever attributes Patient has.

```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
Patients is definited in the schema (which is created through migrations).  When we create the class Patient in the database we can then reference is through the Patients controller.
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
Most of what the model does is recieving commands from the controller.  It does a lot but doesn not need so much required code because of its connection to the controller. It also inherites from Application Record so it doesn't need to spell out all the methods it has available to it.
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
It launches pry using the rails files so that you can references them, and even make changes to the database using .save straight from the rails console.
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
// your response here
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
a JSON string.
```
