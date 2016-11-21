# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```bash
- the router
- using a curl request
```

In what file does the above code go?

```bash
scripts/get-books.sh
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```bash
it executes the rake script with thw command migrate in the current bundle
```

What do we call the string rendered from our server?

```bash
curl
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```bash

```

What is the job of the `serializer`?

```bash
The serializer decides which of the attributes will be shown to users in the
database.
```

What do we expect the command `Patient.all` to return?

```bash
retuens all the patients and their attributes in the database.
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```bash
Patient is defined in the ruby class
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```bash

```

What does typing `rails console` in a directory that houses a rails app do for
us?

```bash
runs pry
```

What does typing `rails db` in a directory that houses a rails app do for us?

```bash
enables us to use psql, the command-line interface to PostgreSQL.
```

What is the specific name for the type of string our data will be coming back
from the server in?

```bash
json
```
