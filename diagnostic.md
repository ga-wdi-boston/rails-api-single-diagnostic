# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
Rails.application.routes.draw do
  resources :books, only: [:show]

  post '/sign-up' => 'users#signup'
  post '/sign-in' => 'users#signin'
  delete '/sign-out/:id' => 'users#signout'
  patch '/change-password/:id' => 'users#changepw'
  resources :users, only: [:index, :show]
end

or

Rails.application.routes.draw do
  resources :books, except: [:new, :edit, :create, :destroy, :update, :index]

  post '/sign-up' => 'users#signup'
  post '/sign-in' => 'users#signin'
  delete '/sign-out/:id' => 'users#signout'
  patch '/change-password/:id' => 'users#changepw'
  resources :users, only: [:index, :show]
end

But that latter one is kind of excessive.
```

In what file does the above code go?

```md
config/routes.rb
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
It creates a migration for your database with correct labelling (e.g. CreateBooks instead of CreateBook), and the migration lets you make changes to your database.
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
I believe using `rails g scaffold things` generates a serializer file, a model file, and a controller file, whereas `rails g controller things` will just generate a controller file.
```

What is the job of the `serializer`?

```md
The serializer is used to send data back to the client... it works kind of like a filter for what the server can send out or receive.
```

What do we expect the command `Patient.all` to return?

```md
A list of all the patients in the Patient database.
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
app/models/patient.rb
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
They're subclasses of ActiveRecord, so whatever code they're lacking in, we can look to the parent class for it.
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
It opens up pry in the database of the rails app.
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
It opens up the database for that rails app? (I can't 100% remember to be honest)
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
JSON
```
