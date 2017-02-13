# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
<form action="/request" method="GET">
  <input type="text" name="books">
  <input type=submit>
</form>
```

In what file does the above code go?

```md
// your response here
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
/running db:migrate runs the change or up method for all the migrations that haven't been run.
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
// a scaffold generates your model, views, controller, and writes to your routes.rb file.
rails g controller things just generates the controller
```

What is the job of the `serializer`?

```md
// returns a hash representing the model
```

What do we expect the command `Patient.all` to return?

```md
// find all patients
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
// Patient model
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
// they define the format of the code not the content
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
// shows the outline of the database structure
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
// generate a blank db
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
//
```
