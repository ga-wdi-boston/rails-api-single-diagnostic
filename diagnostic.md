# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```bash
the back end is our database. it stores and serves data as needed
```

In what file does the above code go?

```bash
model
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```bash
controller
```

What do we call the string rendered from our server?

```bash
views is an outdated concept in MVC
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```bash
Create, Read (show & index), Update, Destroy
```

What is the job of the `serializer`?

```bash
the model is what carries out the CRUD actions
```

What do we expect the command `Patient.all` to return?

```bash
GET INDEX, GET SHOW, POST, PATCH, DESTROY
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```bash
1. the route connects to the controller
2. the controller then send the req to the model
3. the model the database to get person if id 1
4. the model then brings that info back to the controller
5. the controller sends that data directly to the client
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```bash
rails s
```

What does typing `rails console` in a directory that houses a rails app do for
us?

```bash
im pretty sure db:nuke_pave does all of those things
drop -  rake db:drop
create - rake db:create
migrate - rake db:migrate
seed - rake db:seed
```

What does typing `rails db` in a directory that houses a rails app do for us?

```bash
rails g scaffold pet name:string age:date
```

What is the specific name for the type of string our data will be coming back
from the server in?

```bash
serializers allow us to hide data. it also allows us to show date with correct authorization. e.g. if someone was an admin on a site thay would have access to information the public may not
```
