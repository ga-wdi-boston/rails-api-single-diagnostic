# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
bin/rails require '/books/4'
bin/rails :get => "/books/4"
```

In what file does the above code go?

```md
spec.rb
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
migrate will migrate data to the database.
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
generating a scaffold generates a controller but also generates a model, routes, views and test stubs.
```

What is the job of the `serializer`?

```md
Serialization is the process of converting an object into a stream of bytes in order to store the object or transmit it to memory, a database, or a file.
```

What do we expect the command `Patient.all` to return?

```md
All patients
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
In the model
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
Models are where our classes are defined.
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
rails dbconsole figures out which database you're using and drops you into whichever command line interface you would use with it
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
// your response here
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
// your response here
```
