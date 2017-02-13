# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
get '/books', to: 'books#4'
```

In what file does the above code go?

```md
config/routes.rb
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
bundle exec rake db:migrate will take existing information from one table and migrate them into a whole new database.
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
generating scaffold will create all the major pieces of an application(model, controller, etc), while generate controller will generate a controller for things.
```

What is the job of the `serializer`?

```md
The job of the serializer is to serialize which specific attributes and relationships are important for our data in json. 
```

What do we expect the command `Patient.all` to return?

```md
Patient.all will return all patient objects within the scope.
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
The model
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
// your response here
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
This will start rails in the terminal.
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
This will give list a variety of options regarding a potential rails app
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md

```
