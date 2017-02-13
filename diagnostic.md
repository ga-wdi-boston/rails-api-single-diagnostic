# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
// Not very clear about the question.. If asking how do I create a route for the show get request then it is config/routes.rb: get '/books/' to: 'books#index' if it is to respond to the request then I enter the action in the controller
def show
    @book = Book.find(params[:id])
    render json: @book
  end
```

In what file does the above code go?

```md
// in the controller
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
//  Bundle exec is a command used to execute the ordered instructions specified in a script. And rake db: migrate is to update the database to the latest version.

```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
// Rails g scaffold generates views, models, and controllers each with relevant actions in one operation for things. Rails g controller things will create a file called things_controller.rb which will respond to requests for the resource called Things.Requests like get, post, patch, delete.
```

What is the job of the `serializer`?

```md
// The serializer customizes json output.
```

What do we expect the command `Patient.all` to return?

```md
// It is a get request structured in the controller and it will show all the patients.
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
// it is defined in the model as Class Patient.
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
// Because the model is inheriting actions and attributes from the library Active Controller and this library has default structured actions for creating, saving data.
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
// It opens the database console for the cdirectory that houses the rails app.
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
// It does the same? as above in bin/rails db console?
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
// json
```
