# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```bash
1. curl GET localhost/books/4
2. show.books[:4]
```

In what file does the above code go?

```bash
1 in scripts
2 in the controler
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```bash
It runs all the migrations in the order in which they were created and helps to set up the way in which your db is structured
```

What do we call the string rendered from our server?

```bash
json
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```bash
rails scafold builds the entire controler, model and all the actions where as g controler just builds the controler
```

What is the job of the `serializer`?

```bash
It acts as a filter for the content returned from the server
```

What do we expect the command `Patient.all` to return?

```bash
A list of all patients (the index) rendered in json
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```bash
In the patient model
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```bash
They inherit a whole ton of methods from ActiveRecord which isn''t all writen out in the file.
```

What does typing `rails console` in a directory that houses a rails app do for
us?

```bash
It provides an active environment in which to test and manipulate the server processes
```

What does typing `rails db` in a directory that houses a rails app do for us?

```bash
Opens psql in the current rails project dc and allows us to interact with it
```

What is the specific name for the type of string our data will be coming back
from the server in?

```bash
json
```
