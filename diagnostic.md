# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```bash
def index
    @books = books.all

    render json: @books
  end

  def show
    render json: book.find(params[:id])
  end
```

In what file does the above code go?

```bash
In the books controller.
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```bash
It migrates the changes being made to the DB.  I like to compare it to performing
a commit.
```

What do we call the string rendered from our server?

```bash
// your response here
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```bash
`rails g scaffold things` generates a quick template of your application
"rails g controller things" generates the controller and the views.
```

What is the job of the `serializer`?

```bash
The serializer is a way for rails to interpret and convert the data stored in a DB
columns.
```

What do we expect the command `Patient.all` to return?

```bash
All patients in a DB
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```bash
In the patients_controller.rb
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```bash
It inherits much of what it does from ActiveRecord
```

What does typing `rails console` in a directory that houses a rails app do for
us?

```bash
It allows us to run rails commands in an easy to use interface.
```

What does typing `rails db` in a directory that houses a rails app do for us?

```bash
It puts us into psql.
```

What is the specific name for the type of string our data will be coming back
from the server in?

```bash
JSON
```
