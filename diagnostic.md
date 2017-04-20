# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
resources :books, only: [:show]
books#show

or did you want the curl request code?
```

In what file does the above code go?

```md
routes.rb
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
It defines how the database should organize the hash data (model) into the database.
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
I think it's the admin rights, but not positive.
Or does scaffold create the model for the things and the controller is created automatically while
the rails g controller things only makes a controller file of things?
```

What is the job of the `serializer`?

```md
Adapts data into json format?  need clarification on this.
```

What do we expect the command `Patient.all` to return?

```md
list of all instances of object Patient

use this in @patients = Patient.all to assign the instances of object Patient to a variable we
can use for applying method render and other methods as well
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
models/patient.rb
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
Rails has builtins that do that work for us
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
brings up a console for the database  - we can use SQL commands
$rails console opens up pry>
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
dumps the db into SQL environment
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
// your response here
```
