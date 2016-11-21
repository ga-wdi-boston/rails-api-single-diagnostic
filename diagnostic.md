# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```bash
get '/books/:id', to: 'books#show'

or

resources :books, only: [:show]
```

In what file does the above code go?

```bash
config/routes.rb
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```bash
it completes changes made to a database table, such as creating a new table, or adding a column
```

What do we call the string rendered from our server?

```bash
the... response?
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```bash
scaffold creates the controller, as well as the model, whereas controller only creates the controller
```

What is the job of the `serializer`?

```bash
the serializer limits which attributes of your table a user can see
```

What do we expect the command `Patient.all` to return?

```bash
all of the patients created by the Patient class
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```bash
app/models/patient.rb
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```bash
model uses macros, which is code that creates other code
```

What does typing `rails console` in a directory that houses a rails app do for
us?

```bash
it opens the rails console, in which our databases are already loaded
```

What does typing `rails db` in a directory that houses a rails app do for us?

```bash
it opens a psql console, in which our databases are already loaded
```

What is the specific name for the type of string our data will be coming back
from the server in?

```bash
json
```
