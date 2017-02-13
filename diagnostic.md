# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
API="${API_ORIGIN:-http://localhost:4741}"
URL_PATH="/books/${ID}"
curl "${API}${URL_PATH}" \
  --include \
  --request GET

echo

```

In what file does the above code go?

```md
scripts/books/show.sh
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
bundle exec rake runs the version of rake named in the gem file which solves dependencies
db:migrate updates a schema by adding, removing, or updating tables, columns, or entries```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
scaffold is a full set (model, database migration, controller, views, and test suite)
controller is just setting up the controller
```

What is the job of the `serializer`?

```md
describe which attributes and relationships should be serialized
```

What do we expect the command `Patient.all` to return?

```md
it will return a list of all patients in the database
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
models/patient.rb
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
model access the database based on information from the controller```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
it accesses the psql client from the command line
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
it invokes the dbconsole
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
JSON
```
