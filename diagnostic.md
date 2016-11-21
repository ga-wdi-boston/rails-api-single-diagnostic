# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```bash
(notes are still on other computer :( ...))

def show
   render json: @books
 end
```

In what file does the above code go?

```bash
controller
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```bash
appends data to the json model
```

What do we call the string rendered from our server?

```bash
json
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```bash
Generating the scafold gives you everything you need - model, data migration, controller, views, and a test suite.
```

What is the job of the `serializer`?

```bash
To show or hide data attributes to the user
```

What do we expect the command `Patient.all` to return?

```bash
...all of the patients? (in your data base)
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```bash
in your data or .csv file.
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```bash
models are broken down individually be seperation of concerns. Also the controller is where all the heavy lifting happens.
```

What does typing `rails console` in a directory that houses a rails app do for
us?

```bash
its a repl that allows us to test data relations.
```

What does typing `rails db` in a directory that houses a rails app do for us?

```bash
The same as rails console. It figures out what database you are using and put you into what ever repl you would need.
```

What is the specific name for the type of string our data will be coming back
from the server in?

```bash
json
```
