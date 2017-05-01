# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
get /books, to: 'books#index'
resources :books, only: [:index]
```

In what file does the above code go?

```md
routes.rb
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
It's telling the command line to rake and migrate the db.
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
Scaffold is used to generate the columns within the database for example books and assigns each column the stated properties name:string id:integer and is loaded and saved in the schema.rb file

Controller is used to handle requests for a particular type. The controller responds to requestes for a resource i.e Books.
```

What is the job of the `serializer`?

```md
Serializer decscribes which attribute and relationships should be serialized.
```

What do we expect the command `Patient.all` to return?

```md
It should return all the data within the patients db.
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
It is defined in the csv saved file.
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
// your response here
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
It alows developers to work in the files directory.
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
Executing rails db allows us to work directly in the db.
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
// your response here
```
