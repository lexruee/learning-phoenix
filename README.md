# Learning Phoenix

## Creating a new Project

```
mix phx.new PATH [--module MODULE] [--app APP]
```

To get more details how to use the command just run `mix phx.new`.

Once you created a project, then run the following commands to setup the project:

  * Install dependencies with `mix deps.get`
  * Create and migrate your database with `mix ecto.setup`
  * Install Node.js dependencies with `cd assets && npm install`
  * Start Phoenix endpoint with `mix phx.server`
  * Start Phoenix endpoint in the iex console with `iex -S mix phx.server`

Now you can visit [`localhost:4000`](http://localhost:4000) from your browser.

Ready to run in production? Please [check our deployment guides](https://hexdocs.pm/phoenix/deployment.html).


## Online Resources

 * [Phoenix Getting Started Guide](https://hexdocs.pm/phoenix/up_and_running.html)
 * [Phoenix Documentation](https://hexdocs.pm/phoenix/overview.html)
 * [Phoenix Project Website](https://phoenixframework.org/)

## Book Resources

 * [Programming Phoenix](https://pragprog.com/book/phoenix/programming-phoenix)
