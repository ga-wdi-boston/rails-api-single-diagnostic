# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
get '/books', to: 'books#index'
resources :books, only: [:index]
```

In what file does the above code go?

```md
routes.rb
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
this command executes the rake script with the command db:migrate in the context


```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
rails g controller with generate just a controller shell while rails g
scaffold will generate shells for model, view and controller
```

What is the job of the `serializer`?

```md
allows you to store almost any object in a single database field
```

What do we expect the command `Patient.all` to return?

```md
all of the objects associated with the class Patient
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
it is defined in the model as patient.rb
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
That is the beauty of Rails
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
it takes us to the psql console and connects us to our database
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
looks to be the same as above for bin/rails dbconsole
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
json
```
