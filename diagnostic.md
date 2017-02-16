# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
#we want show, because we are returning a single instance of a book, not the entire index. I can not think of another way at the moment, but will try to come back to this and finish it if I have time

get '/books', to: 'books#show'

#2nd attempt from:http://edgeguides.rubyonrails.org/routing.html
get 'book/:id' to: 'books#show'
```

In what file does the above code go?

```md
The routes file: routes.rb
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
It executes the rake script with the db:migrate command for the current bundle so we do not have to manually type it in that file.
Migrations let us change parts of the database at a time which makes the process of altering databses go much quicker.

```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
The first one will create our model, view and controller, while the second one will create just our controller.
```

What is the job of the `serializer`?

```md
When we have an attribute that we need saved to the database as an object, then we use a serializer, which represents the object as a text/string.
```

What do we expect the command `Patient.all` to return?

```md
All instances of the Patient saved in the database.
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
It is defined in the model.
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
Because model is just defining the classes. The methods we will actually be using on them are defined in the controller, so there is more code there. Neither can do anything without the other.
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
It allows us to work with the database in the console with the CLI you choose. We have been mainly using postgres.
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
It allows us to interact with the database, but is usually followed by a command like :migrate or :create. My understanding is that typing rails db by itself will display the database in the console, but will not "do" anything to it.
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
We want everything parsed as JSON.
```
