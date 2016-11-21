# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```bash
get '/books/4', to: 'books#show'
get '/books/4' => 'books#show'

```

In what file does the above code go?

```bash
routes.rb
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```bash
Takes the modified/edited version of your database and pushes the changes to the
database. This change is kept in your schema file.
```

What do we call the string rendered from our server?

```bash
A response
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```bash
A scaffold sets up controller, model, and routes

The controller command only sets up a controller
```

What is the job of the `serializer`?

```bash
To "filter" the data that the user gets to see. Sometimes you want to hide data
from the user if it is not neccessary or for security reasons.
```

What do we expect the command `Patient.all` to return?

```bash
A table of all of the patients.
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```bash
In the Patient model
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```bash
Fat controller, skinny model.
```

What does typing `rails console` in a directory that houses a rails app do for
us?

```bash
// your response here
```

What does typing `rails db` in a directory that houses a rails app do for us?

```bash
// your response here
```

What is the specific name for the type of string our data will be coming back
from the server in?

```bash
JSON
```
