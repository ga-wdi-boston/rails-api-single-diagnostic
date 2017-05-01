# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
get '/books', to: 'books4'
resources :books, only: [4]
```

In what file does the above code go?

```md
config/routes.rb
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
sets up migration
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
scaffold is used when generating code by hand, controller uses rails
```

What is the job of the `serializer`?

```md
"gatekeeper", it is a file that allows us to customize the output that rails sends as JSON from our server
```

What do we expect the command `Patient.all` to return?

```md
it will return an array of multiple patients
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
patient.rb
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
rails provides a generator for creating models
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
used to figure out which database you are using and puts you to the command line inteface
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
help with troubleshooting and telling you what the current version of the database is
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
TEXT
```
