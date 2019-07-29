# Learning Phoenix

## Installation on Arch Linux

### Version manager

First, install the version manager `asdf-vm`:

```bash
yay -S asdf-vm
```

### Elixir

``` 
asdf plugin-add elixir
asdf plugin install elixir 1.9.0
asdf global elixir 1.9.0
```

Check:

``` 
elixir --version
mix --version
```


### Node.js

``` 
asdf plugin-add nodejs
asdf plugin install nodejs 12.2.0
asdf global nodejs 12.2.0
```

Check:

``` 
node --version
```


### Postgres

``` 
yay -S postgresql
sudo -iu postgres
initdb -D /var/lib/postgres/data
exit
```

Check:

``` 
psql --version
```

### Phoenix
``` 
mix local.hex
mix archive.install hex phx_new 1.4.8
```


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

## mix phx 

The main command to use is `mix` in combination `phx` tasks. 

To get a list of available phx tasks run `mix help | grep -i phx`.

Examples: 

```
mix local.phx          # Updates the Phoenix project generator locally
mix phx                # Prints Phoenix help information
mix phx.digest         # Digests and compresses static files
mix phx.digest.clean   # Removes old versions of static assets.
mix phx.gen.cert       # Generates a self-signed certificate for HTTPS testing
mix phx.gen.channel    # Generates a Phoenix channel
mix phx.gen.context    # Generates a context with functions around an Ecto schema
mix phx.gen.embedded   # Generates an embedded Ecto schema file
mix phx.gen.html       # Generates controller, views, and context for an HTML resource
mix phx.gen.json       # Generates controller, views, and context for a JSON resource
mix phx.gen.presence   # Generates a Presence tracker
mix phx.gen.schema     # Generates an Ecto schema and migration file
mix phx.gen.secret     # Generates a secret
mix phx.new            # Creates a new Phoenix application
mix phx.new.ecto       # Creates a new Ecto project within an umbrella project
mix phx.new.web        # Creates a new Phoenix web project within an umbrella project
mix phx.routes         # Prints all routes
mix phx.server         # Starts applications and their servers
```

For more details see the [Phoenix Mix Documentation](https://hexdocs.pm/phoenix/phoenix_mix_tasks.html).

## Basic Examples
 
 * [Hello World App](https://github.com/lexruee/phx-hello)
 * [Todo App](https://github.com/lexruee/phx-todo)
 * [Blog App](https://github.com/lexruee/phx-blog)
 * [Login App](https://github.com/lexruee/phx-login)


## Online Resources

 * [Phoenix Getting Started Guide](https://hexdocs.pm/phoenix/up_and_running.html)
 * [Phoenix Documentation](https://hexdocs.pm/phoenix/overview.html)
 * [Phoenix Project Website](https://phoenixframework.org/)

## Book Resources

 * [Programming Phoenix](https://pragprog.com/book/phoenix/programming-phoenix)
