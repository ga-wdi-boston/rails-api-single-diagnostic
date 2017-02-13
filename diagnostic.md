# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
get '/books', to: 'books#index'
```

In what file does the above code go?

```md
config/routes.rb
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
rake db:migrate generates a migration file. In the file, Rails creates a class that inherits from ActiveRecord:: Migration. In other words, this is Rails way of telling the database what to do. The class will have generated methods specified by what you command.
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
rails g scaffold things - Scaffolding is merely an automatism that does the work for us for some basic things.
rails g controller things - if I want more control 
```

What is the job of the `serializer`?

```md
ActiveModelSerializers brings convention over configuration to your JSON generation.
ActiveModelSerializers works through two components: serializers and adapters.
Serializers describe which attributes and relationships should be serialized.
Adapters describe how attributes and relationships should be serialized.

wraps a serializable resource and exposes an attributes method, among a few others. It allows you to specify which attributes and associations should be represented in the serializatation of the resource.
```

What do we expect the command `Patient.all` to return?

```md
To return all patients from the table.
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
in the file .csv
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
they work with data from the database
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
switches to pry where we can test our database
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
opens my database client and loads the correct database
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
JSON
```
