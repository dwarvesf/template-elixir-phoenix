# <%= name %>
> <%= description %>

## Setup your project before run
Update content in `config/dev.exs` and `config/test.exs`

```Elixir
# Configure your database
config :<%=name%>, <%=name%>.Repo,
  adapter: Ecto.Adapters.Postgres,
  username: System.get_env("POSTGRES_USER") || "postgres",
  password: System.get_env("POSTGRES_PASSWORD") || "postgres",
  hostname: System.get_env("POSTGRES_HOST") || "localhost",
  database: "<%=name%>_(dev|test)",
  pool_size: 10
```

## How to run your project
```
make run
```

## How to test your project
```
make test
```
## License

MIT &copy; [Dwarves Team](github.com/dwarvesf)
