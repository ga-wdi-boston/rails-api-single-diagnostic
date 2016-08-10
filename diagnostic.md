# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What is the purpose of a backend?

```bash
To store data and to send that data to the client upon requests.
```

Which layer in the MVC pattern is used by the controller to fetch data?

```bash
the model
```

Which layer in the MVC pattern communicates with the model?

```bash
the database
```

Why don't we use views in our interpretation of the MVC pattern?

```bash
Because we have the controller skip that step by sending JSON back to the client;
it is more efficient that way.
```

What does C.R.U.D stand for?

```bash
Create Read Update Destroy
```

In which part of the MVC pattern can we find C.R.U.D actions?

```bash
the controller
```
List at least 5 standard actions that C.R.U.D corresponds to?

```bash
Create - Create
Read - index, show
Update - Patch
Destroy - Delete
```

A user action fires a `GET` request for `person/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list)

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

What is the command to start an instance of a rails server?

```bash
rails s
```

What are the commands to drop, create, migrate and seed a database? (3 bullet
points)

```bash
<ul>
  <li>bundle exec rake rails db:drop</li>
  <li>bundle exec rake db:create</li>
  <li>bundle exec rake g migration</li>
  <li>bundle exec rake db:seed</li>
</ul>
```

What is the command to scaffold a pet with a name and an age?

```bash
rails g scaffold Pet name:string age:integer
```

List two advantages of using serializers? (2 bullet points)

```bash
<ul>
 <li>You can hide attributes that are unneccssary for users to see.</li>
</ul>
```
