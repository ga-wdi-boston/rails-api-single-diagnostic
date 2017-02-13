# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
// find and update
```

In what file does the above code go?

```md
// the controller
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
// bundle exec rake will update the gem files and bd:migrate will migrate a database
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
// rails g scaffold will create a whole framework while rails g controller just makes the controller folder
```

What is the job of the `serializer`?

```md
// it converts the data into json
```

What do we expect the command `Patient.all` to return?

```md
// the params for the patient
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
// in the model
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
//  because it is just validating the content types not the content itself
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
// it brings the databa
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
// it opens a psql session
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
// json
```
