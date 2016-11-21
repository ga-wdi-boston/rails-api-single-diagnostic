# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```bash
get '/books/:id', to: 'books#show'
get '/books/:id' => 'books#show'
```

In what file does the above code go?

```bash
Routes.rb
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```bash
This is a rake command that loads starting data (if any exists) and/or migrates/pushes changes made to the database.
```

What do we call the string rendered from our server?

```bash
Response
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```bash
The scaffold command generates a scaffold controller that creates the full MVC stack from model, through controller, to the views.

This regualr controller simply creates a controller file by appending controller.rb to 'things', the file name supplied.
```

What is the job of the `serializer`?

```bash
They control what information is sent to the client and can be seen as JSON formatters.
```

What do we expect the command `Patient.all` to return?

```bash
Return a list of all resource instances of the class Patient.
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```bash
In the model.
```

Why do our `model` files appear to be lacking so much code, when they are doing
so much for us?

```bash
The methods used by the model are defined in the controller.
```

What does typing `rails console` in a directory that houses a rails app do for
us?

```bash
It allows us to make use of our models by letting us interact with Rails from the command line.
```

What does typing `rails db` in a directory that houses a rails app do for us?

```bash
This command invokes the dbconsole, which figures out which database you’re using and drops you into whichever command line interface you would use with it (and figures out the command line parameters to give to it).
```

What is the specific name for the type of string our data will be coming back
from the server in?

```bash
JSON
```
