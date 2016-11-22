# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```bash
To store data and to send that data to the client upon requests.
```

In what file does the above code go?

```bash
the model
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```bash
the database
```

What do we call the string rendered from our server?

```bash
Because we have the controller skip that step by sending JSON back to the client;
it is more efficient that way.
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```bash
Create Read Update Destroy
```

What is the job of the `serializer`?

```bash
the controller
```

What do we expect the command `Patient.all` to return?

```bash
Create - Create
Read - index, show
Update - Patch
Destroy - Delete
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```bash
<ol>
  <li>The GET request gets sent to the router.</li>
  <li>The router takes the GET request and the given URL and matches it to the
  correct controller action.</li>
  <li>That controller action communicates to the appropriate model which houses the
  business logic</li>
  <li>The model communicates with the database and the databse returns the data back to the model.</li>
  <li>The model gives that data to the controller and the controller turns the data into JSON and sends it to the client.</li>
</ol>
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```bash
rails s
```

What does typing `rails console` in a directory that houses a rails app do for
us?

```bash
<ul>
  <li>bundle exec rake rails db:drop</li>
  <li>bundle exec rake db:create</li>
  <li>bundle exec rake g migration</li>
  <li>bundle exec rake db:seed</li>
</ul>
```

What does typing `rails db` in a directory that houses a rails app do for us?

```bash
rails g scaffold Pet name:string age:integer
```

What is the specific name for the type of string our data will be coming back
from the server in?

```bash
<ul>
 <li>You can hide attributes that are unneccssary for users to see.</li>
</ul>
```
