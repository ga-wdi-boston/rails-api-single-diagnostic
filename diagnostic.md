# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What are two ways of telling rails where to route a GET request to '/books/4'?

```bash
Using use Ruby''s Net::HTTP class:

require 'net/http'

url = URI.parse('localhost:4741/books/4')
req = Net::HTTP::Get.new(url.to_s)
res = Net::HTTP.start(url.host, url.port) {|http|
  http.request(req)
}
puts res.body

get '/books/:id', to: 'books#show'

```

In what file does the above code go?

```bash
routes.rb
```

In your own words, what does the command `bundle exec rake db:migrate` do?

```bash
It creates migrations and acts somewhat as the equivalent of commits on git hub.
 So similar to version contorl.
```

What do we call the string rendered from our server?

```bash
JSON
```

What is the difference between `rails g scaffold things` and
`rails g controller things`?

```bash
`rails g scaffold things` - this generates a scaffold which tells rails how the
application database may be used. Rails then uses this specification together
with its templates to genereate the that the app uses on the database.

`rails g controller things` - generates a controller for 'things'.
```

What is the job of the `serializer`?

```bash
// your response here
```

What do we expect the command `Patient.all` to return?

```bash
Patient.all would return a table of all patients.
```

We use the constant `Patient` in the `PatientsController`, but where is it
actually defined?

```bash
its defined in the model
```

Why do our `model` files appear to be lacking so much code, when they're doing
so much for us?

```bash
The model files define a class for each data set in addition defining other
characteristics.
```

What does typing `rails console` in a directory that houses a rails app do for
us?

```bash
opens a console where we can perform operations on that MVC and build and
troubleshoot.
```

What does typing `rails db` in a directory that houses a rails app do for us?

```bash
// your response here
```

What is the specific name for the type of string our data will be coming back
from the server in?

```bash
JSON
```
