# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
before_action :set_patient, only: [:show]
def show
    render json: @patient
end

def set_patient
    @patient = Patient.find(params[:id])
end
private :set_patient

def show
  @patient = Patient.find(params[:id])

  render json: @patient
end
```

In what file does the above code go?

```md
In the `app/controllers/books_controller.rb`.
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
The command `bundle exec rake db:migrate` creates a path for the developer to
experiment and change their code.
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
Creating a scaffold creates the controller, the model, and the serializer,
and it inputs the controller with the CRUD actions. Using the latter command
just creates the controller, but we have to put in the CRUD actions manually.
```

What is the job of the `serializer`?

```md
The `serializer`'s job is to
```

What do we expect the command `Patient.all` to return?

```md
The command `Patient.all` is supposed to return all of the patients that we
have in our database.
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
The constant `Patient` is actually defined in the `ApplicationController`;
The `PatientsController` inherits from it.
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
The `model` files contain so little because they are validating what should
be shown in the database; they also show the relationship between two databases.
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do
for us?

```md
Typing `bin/rails console` will open up pry.
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
Typing `bin/rails db` would open up Postgres.
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
It will come back in JSON format.
```
