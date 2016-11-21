# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```bash
resources :books, only: [:show]
get '/books/4', to: 'books#show'

```

In what file does the above code go?

```bash
routes.rb
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```bash
Using the gems, which have been installed in the repo, the gem rake makes changes to the database.
```

What do we call the string rendered from our server?

```bash
// your response here
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```bash
A scaffold creates all of the basic file structure need for an app along with the controller, model and view.

`rails g controller things` will only create a things controller
```

What is the job of the `serializer`?

```bash
A serializer acts a filter and determines what parts of a table can be used by the front end.
```

What do we expect the command `Patient.all` to return?

```bash
All the patients
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```bash
in the migration
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```bash
because the controller is telling the model what to do
```

What does typing `rails console` in a directory that houses a rails app do for
us?

```bash
It opens up the rails REPL so that you can directly interact with the database.
```

What does typing `rails db` in a directory that houses a rails app do for us?

```bash
It places you in the databaseb that the app uses.
```

What is the specific name for the type of string our data will be coming back
from the server in?

```bash
a secure string ?
```
