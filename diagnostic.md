# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
curl --include --request GET http://localhost:4741/books/4

API="${API_ORIGIN:-http://localhost:4741/books/4}"
URL_PATH="/examples"
curl "${API}${URL_PATH}" \
  --include \
  --request GET \
  --header "Authorization: Token token=$TOKEN"

```

In what file does the above code go?

```md
This code would go in the scripts folder.  An example file in that folder may be "get-ingredient.sh"
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
It executes the rake script specific to your gemfile.  The command db:migrate runs migrations that have yet to run.

```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
"Rails g scaffold things" creates a full set of model, database migration for the model, controller, and views.  "Rails g controller things" specifically creates a new controller called things.
```

What is the job of the `serializer`?

```md
A serializer describe which attributes and relationships should be serialized.  They are used for rendering JSON responses.
```

What do we expect the command `Patient.all` to return?

```md
// Nothing on its own, but it refers to all instances of patient.
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
In the patient model.
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
// your response here
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
It determines which database you're using and allows you to interface with its command line.
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
// your response here
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
// your response here
```
