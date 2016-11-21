# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```bash
localhost:XXXX/books/4
Also, via curl request
```

In what file does the above code go?

```txt
Not sure what is being looked for here. It could be in a a script file so the curl request could be run from the command line. It could also be the routes file that is like Ruby's air traffic controller.
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```txt
This function is like pushing to whatever changes we have made to our code to GitHub. This updates our rails API with the most recent chages made.
```

What do we call the string rendered from our server?

```bash
JSON
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```txt
Scaffold just creates predeterimined files that Ruby assumes you will need (model, controller, database, etc.) where as generating a controller allows for more fine tune precision as to what is being created.
```

What is the job of the `serializer`?

```txt
The serializer acts as a filter for what our rails server will allow to be seen. If we have a column called 'secretstuff' and we don't add it to our serializer it will not be seen.
```

What do we expect the command `Patient.all` to return?

```txt
A list of all the Patients in the database
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```bash
In the database
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```bash
They inherit information from Rails. Basically because rails is awesome.
```

What does typing `rails console` in a directory that houses a rails app do for
us?

```bash
It enables us to view and manipulate our database via Ruby
```

What does typing `rails db` in a directory that houses a rails app do for us?

```bash
Puts us into PSQL
```

What is the specific name for the type of string our data will be coming back
from the server in?

```bash
JSON
```
