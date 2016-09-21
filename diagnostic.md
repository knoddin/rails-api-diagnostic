# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.

What is the purpose of a backend?

```bash
The purpose of a backend is to allow for data storage and separate communication between
a client and a server. We do not necessarily want other viewers/users to see the communication
that other users are having with the server.
```

Which layer in the MVC pattern is used by the controller to fetch data?

```bash
The model fetches data upon command from the controller.
```

Which layer in the MVC pattern communicates with the model?

```bash
The controller.
```

Why don't we use views in our interpretation of the MVC pattern?

```bash
Our interpretation of view is just the browser...
```

What does C.R.U.D stand for?

```bash
CREATE, READ, UPDATE, DELETE
```

In which part of the MVC pattern can we find C.R.U.D actions?

```bash
Controller contains all the methods.
```

List at least 5 standard actions that C.R.U.D corresponds to?

```bash
create, index, show, update, destroy
```

A user action fires a `GET` request for `/persons/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list)

```bash
1. client talks to server to ask for the person with ID 1 but server doesnt have it
2. server connects with router
3. router connects with the controller, which fires all the methods it has in store for the get request
4. the methods within the controller fire to the model
5. the model, if the messages are correct, retrieves data in database
6. the model passes back to controller
7. controller passes info to router and then to server
8. server sends information back to the client
```

What is the command to generate a new rails-api app?

```bash
rails-api new
```

What is the command to start an instance of a rails server?

```bash
bundle exec rails-api
```

What are the commands to drop, create and migrate a database? (3 bullet points)

```bash
bundle exec rake db: drop
bundle exec rake db: create
bundle exec rake db: migrate
```

What is the command to scaffold a pet with a name and age attributes (hint:
Also think of the data types for each attribute)?

```bash
bundle exec rails-api g scaffold pet name:string age:integer 
```
