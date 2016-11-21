# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```bash
curl GET http://localhost:3000/books/4
```

In what file does the above code go?

```bash
Routes file. ```

In your own words, what does the command `bundle exec rake db:migrate` do?

```bash
That command migrates the changes made to the database schema. It essentially creates a new version of the database with the updates modificaitons.
```

What do we call the string rendered from our server?

```bash
Not sure about this one.
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```bash
Scaffolding will generate the model, controller, view, and routes used in 'things'. Rails g controller will only generate the controller assocaited with the things, not the other components. ```

What is the job of the `serializer`?

```bash
The serializer determines what data is viewable when manipultaing a database. ```

What do we expect the command `Patient.all` to return?

```bash
A list of all the patients.```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```bash
Its defined in the model. ```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```bash
Because they're mostly being told what to do by the controller.
```

What does typing `rails console` in a directory that houses a rails app do for
us?

```bash
Typing 'rails console' allows us to interact with the Rails application from the command line.  ```

What does typing `rails db` in a directory that houses a rails app do for us?

```bash
It inserts us into the database we're currently working on. ```

What is the specific name for the type of string our data will be coming back
from the server in?

```bash
No sure about this one. ```
