# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```bash
you could use a routes file for ruby with an entry "get /books/4"
alternatively you could use an SQL request along the lines of "SELECT * FROM books WHERE id IN 4"
```

In what file does the above code go?

```bash
the ruby code goes in a routes.rb file, while the SQL could go in something like 060_get_book_id_4.sql
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```bash
it executes a migration file which often runs a series of sql files to perform table setup and other such actions
```

What do we call the string rendered from our server?

```bash
a return? render json "somestings"?
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```bash.
a scaffold sets up starter code for a generic rails component while a controller sets up the requesite files specifically designed for a rails controller
```

What is the job of the `serializer`?

```bash
A serializer prevents a get request from returning all content except that which is specified as being permissable.
```

What do we expect the command `Patient.all` to return?

```bash
I would expect it might return a list of all instances of the class patient, assuming such a function exists within the patient class
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```bash
It is defined in the PatientsModel file
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```bash
much of that code, especifically variables associated with the model, are defined in a related file.
```

What does typing `rails console` in a directory that houses a rails app do for
us?

```bash
It gives us the ability to execute code directly inside the rails server.
```

What does typing `rails db` in a directory that houses a rails app do for us?

```bash
It gives direct access to our active rails database and the information stored with it.
```

What is the specific name for the type of string our data will be coming back
from the server in?

```bash
A json object?
```
