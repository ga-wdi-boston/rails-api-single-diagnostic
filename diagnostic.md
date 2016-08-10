# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What is the purpose of a backend?

```bash
One of the purpose of backend is to store data that can be accessed, manipulated and deleted. To be able to do that we would need front end to interact with backend.
```

Which layer in the MVC pattern is used by the controller to fetch data?

```bash
Route takes request and gives it to controller
```

Which layer in the MVC pattern communicates with the model?

```bash
Controller receives the request from route and fires up a method that is needed for that request. Then it sends it to model where bussines logic happens.

So, answer is controller layer.
```

Why don't we use views in our interpretation of the MVC pattern?

```bash
Because it takes time to render the page for each change. Instead we are collecting all changes and we send it all toghether back to the user.
```

What does C.R.U.D stand for?

```bash
Create, read, update, delete
```

In which part of the MVC pattern can we find C.R.U.D actions?

```bash
Requests are in route part.

Methods(actions) that are needed are in Controller part. It receives request from route, and we store those requests in our controller.
```
List at least 5 standard actions that C.R.U.D corresponds to?

```bash
index, show, create, update, destroy
```

A user action fires a `GET` request for `person/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list)

```bash
Route receives request. Request would look like this:   get '/person/:id', to: 'people#show'. For this request we need to fire method show. Controller will hold that method. So, that request is now in controller part.  Controller fires up the method that needs a model to work on with that method. Model is created. Model needs data to be able to operate on it. Data is created in rails console. newPerson = Person.create(some person). Then it goes back to the controller, and controller send it back to the route that is user on the front end.
```

What is the command to start an instance of a rails server?

```bash
// your response here
```

What are the commands to drop, create, migrate and seed a database? (4 bullet
points)

```bash
rake db:drop
rake db:create
rake db:migrate
rake db:seed

I think this is all done with rake db:nuke_pave.
```

What is the command to scaffold a pet with a name and an age?

```bash
rails g scaffold pet name:string age:integer
```

List two advantages of using serializers? (2 bullet points)

```bash
1. It protects your data.
2. To make your JSON look good.

```
