# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
resources :books, only: [:show]
resources :books, except: [:new, :edit, :index, :create, :update]
```

In what file does the above code go?

```md
routes.rb
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
It takes the ruby data model and creates a SQL table to that coresponeds to that ruby data model
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
The scaffold sets up a ruby model, the SQL migration fo rth model, a controller and views to view the data.
The controller will jus set up a controller file in the controlers directory.  So it is not creating as many things.
```

What is the job of the `serializer`?

```md
The searilizers basically allows you to use the .from_json OR .as_json methods to manipulate objects with JSON.  That's basically me just quoting the rubyonrails.org definition
```

What do we expect the command `Patient.all` to return?

```md
A list of all the patients in an array or an object depening on how it is stored
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
In the /models/patient.rb file, which is super weired.
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
A question I keep asking myself!
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
It determines which database the commond line file is in and just plops you down in there.
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
// your response here
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
JSON
```
