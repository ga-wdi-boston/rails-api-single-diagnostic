# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```bash
get '/books/:id', to: 'books#show'
resources :books, only: [:show]
```

In what file does the above code go?

```bash
config/routes.rb
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```bash
bundle exec makes sure that the proper rake is used rather than a global install.
The rake command checks for any un-run db migrations and runs them.
```

What do we call the string rendered from our server?

```bash
JSON
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```bash
The scaffold also generates the controller, however, additionally adds
other code such as RESTful routes.
```

What is the job of the `serializer`?

```bash
The serializer allows us to filter which parameters are returned.
```

What do we expect the command `Patient.all` to return?

```bash
Return a string of all patient objects.
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```bash
The Patient model.
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```bash
They are inheritting a lot of their code from ActiveRecord.
```

What does typing `rails console` in a directory that houses a rails app do for
us?

```bash
We can interact with our rails app from the command line.
```

What does typing `rails db` in a directory that houses a rails app do for us?

```bash
Open the DB for us to interact with directly from the command line.
```

What is the specific name for the type of string our data will be coming back
from the server in?

```bash
JSON
```
