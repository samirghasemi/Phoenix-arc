# Test
how to run this project:
To start your Phoenix server:

  * Install dependencies with `mix deps.get`
  * Create and migrate your database with `mix ecto.setup`
  * Install Node.js dependencies with `npm install` inside the `assets` directory
  * Start Phoenix endpoint with `mix phx.server`

Now you can visit [`localhost:4000`](http://localhost:4000) from your browser.

Ready to run in production? Please [check our deployment guides](https://hexdocs.pm/phoenix/deployment.html).




# Arc 
## arc for Phoenix
arc is library to implement upload file in Phoenix

Make project and wait for install dependency:
```sh
mix phx.new test
```
go to project folder and config your database in config/dev.exs
```
# ...
config :test, Test.Repo,
  username: "postgres",
  password: "1234",
  database: "test3_dev",
  hostname: "localhost",
# ...
```

And create your database:

```sh
mix ecto.create
```

Create user model:
```sh
mix phx.gen.html Accounts User users avatar:string username:string
```

migrate your new model in database:
```sh
mix ecto.migrate
```
