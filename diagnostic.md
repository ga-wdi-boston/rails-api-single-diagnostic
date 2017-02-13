# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```rb
get '/books/4' or to: 'books#4'
```

In what file does the above code go?

```md
routes.rb
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```md
It trasfers a copy of the previous version of the database, or from the production version. So that you can make and test new changes without affecting production, or at least the working copy.
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```md
The scaffold commands sets up a basic rails template for the things database, where as the controller command sets up just the controller page from the database things.
```

What is the job of the `serializer`?

```md
This creates and adds the index that items in the data base will be listed by.
```

What do we expect the command `Patient.all` to return?

```md
A list of all the things that are contained under the class Patient.
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```md
It is defined in the patient create file.
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```md
Model just proecesses commands and data based on the command given. It however doesn't contain the data, and is just responding the controler.
```

What does typing `bin/rails dbconsole` in a directory that houses a rails app do for
us?

```md
It allows use to interact with the database that we're working on inside the console.
```

What does typing `rails db` in a directory that houses a rails app do for us?

```md
Not sure what that specific command does, however from what I can interperate it acts like db new or db migrate. Meaning it starts a new path or database. The other option is it would start the migration process to build a new working area.
```

What is the specific name for the type of string our data will be coming back
from the server in?

```md
I would assume its either json or xml? That is just from what I can tell, but I am not sure at all.
```
