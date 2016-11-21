# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```bash
get '/books/:id', to: 'books#show'
resources :books, only: [:show]
```

In what file does the above code go?

```bash
routes.rb
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```bash
The above command 'migrates' the way you have your Database setup in Rails into
an SQL database, forming the tables and relationships as specified in the way
you configured Rails.
```

What do we call the string rendered from our server?

```bash
A response
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```bash
`rails g controller things` just generates a ThingsController, while using
scaffold will generate a lot of things for us, like the controller, model, and
some other stuff.
```

What is the job of the `serializer`?

```bash
The job of a 'serializer' is to 'hide' certain columns in a model from the user
when the user makes requests. 
```

What do we expect the command `Patient.all` to return?

```bash
All the Patient rows in the Patients table
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```bash
Patient is defined in Patient.rb, as it is a model.
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```bash
Because Rails is a beautiful thing; if we took a look at what a model is inheriting
from ActiveRecord I bet our eyes would fall out. So Rails takes care of a lot of
things for us.
```

What does typing `rails console` in a directory that houses a rails app do for
us?

```bash
The above command opens a console to our Rails app, allowing us to run commands
like 'Patient.all' or 'Patient.new' to show, test and modify our database directly.
```

What does typing `rails db` in a directory that houses a rails app do for us?

```bash
It opens psql and connects us to the database that rails is using for that app.
```

What is the specific name for the type of string our data will be coming back
from the server in?

```bash
... a response? Again?
```
