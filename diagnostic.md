# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
resources :books, only: [:index, :show]
resources :books, except: [:new, :edit]
```

In what file does the above code go?

```md
config/routes.rb
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
`bundle exec` will execute a script from the current bundle. `rake db:migrate` will run a migrate task in the `db` space.
Reference: http://stackoverflow.com/questions/6588674/what-does-bundle-exec-rake-mean
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
These commands will generate different things. The scaffold command will generate a model file, a migration file, test routes, a test controller, and several files in the views directory. The controller command will generate a controller with all of the RESTful actions (new, create, update, edit, destroy, index, show).
```

What is the job of the `serializer`?

```md
Serializers describe which attributes and relationships should be serialized. By using a serializer, ActiveRecord objects will be placed into the desired response format (JSON).
```

What do we expect the command `Patient.all` to return?

```md
`Patient.all` should return an index of all the patients listed in the directory.
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
`Patient` is a class, which is defined in the models folder. The file is located in app/models/patient.rb.
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
Each of the classes in our models are inheriting from ApplicationRecord. ApplicationRecord inherits from ActiveRecord::Base. A lot of the functionality we see is coming from ActiveRecord::Base.
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
`bin/rails dbconsole` figures out which database you're using. It will also drop you into the appropriate command line interface.
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
`rails db` does the same thing as `bin/rails dbconsole`.
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
Our data will be coming back from the server in the form of a response body.
```
