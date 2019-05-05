# AircraftRegistry

**TODO: Add description**

#### Build aircraft registry DB
```bash
cd app/aircraft_registry/docker
docker build -t aircraft-registry-db -f Dockerfile.db .
```

#### Run aircraft registry DB
`docker run -p 5432:5432 --rm aircraft-registry-db`

#### Run a pgadmin server
`docker run --rm -p 80:80 -e "PGADMIN_DEFAULT_PASSWORD=password" -e "PGADMIN_DEFAULT_EMAIL=admin" dpage/pgadmin4`

## Installation

If [available in Hex](https://hex.pm/docs/publish), the package can be installed
by adding `aircraft_registry` to your list of dependencies in `mix.exs`:

```elixir
def deps do
  [
    {:aircraft_registry, "~> 0.1.0"}
  ]
end
```

Documentation can be generated with [ExDoc](https://github.com/elixir-lang/ex_doc)
and published on [HexDocs](https://hexdocs.pm). Once published, the docs can
be found at [https://hexdocs.pm/aircraft_registry](https://hexdocs.pm/aircraft_registry).
