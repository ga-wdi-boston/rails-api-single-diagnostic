# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```bash
specify your route with to:/books/4 in routes
or write a CRUD request specifically into terminal using CURL request
```

In what file does the above code go?

```bash
routes.rb

```

In your own words, what does the command `bundle exec rake db:migrate` do?

```bash
It brings the current table data into the table that was just created

```

What do we call the string rendered from our server?

```bash
The error message?  I guess.  The 'do next to make this thing work' message?

```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```bash
scaffold will set up an entire API for you, with routes, controllers, etc.  Controller will just set up the Controller for you.
```

What is the job of the `serializer`?

```bash
To filter out things that you don't want seen.

```

What do we expect the command `Patient.all` to return?

```bash
All of the patients.

```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```bash
Hmm, so the parameters of the Patient are defined in controller, but the Class is actually
declared in the Model, so...both?  I guess really it's defined in the table, because the columns associated
with the patient are what define it.

```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```bash
because they inherit from activerecord.  Which is still confusing.
```

What does typing `rails console` in a directory that houses a rails app do for
us?

```bash
brings us into our rails app
```

What does typing `rails db` in a directory that houses a rails app do for us?

```bash
shows us all of our available databases
```

What is the specific name for the type of string our data will be coming back
from the server in?

```bash
JSON, but only because we specify render JSON?
```
