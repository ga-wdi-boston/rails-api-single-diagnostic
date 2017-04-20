# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
I am assuming that you are talking about the routing file.
resources :books, only: [:show]
resources :books, except: [:new, :edit, :destroy, :update, :index, :create]
```

In what file does the above code go?

```md
It goes in the routes.rb file.
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
It goes through your migration files in your bundle (or migrate folder) and creates tables, modifies schema, and adds entries based on the code in the file.
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
rails generate scaffold - this generates everything need like controllers, routes, and db. Basically eveything you need
rails generate controller - would generate just controller files for things by contrast.
```

What is the job of the `serializer`?

```md
The serializer seems to convert the data that we give it for storage.  In this case, the serializer
must be used to translate thing to and from JSON.
```

What do we expect the command `Patient.all` to return?

```md
We expect this to return all the object instances of class Patient.
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
The Class of Patient is defined by our model
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
They are lacking code because they are inheriting the methods associated with ApplicationRecord
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
It will load up the appropriate database that your are using and allow you to interact with it directly using your tool.
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
It seems to work the same way as bin/rails dbconsole.
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
JSON
```
