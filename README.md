# Chirp

This is the 1.6.11 version of https://www.youtube.com/watch?v=MZvmYaFkNJI

To start your Phoenix server:

  * Install dependencies with `mix deps.get`
  * Create and migrate your database with `mix ecto.setup`
  * Start Phoenix endpoint with `mix phx.server` or inside IEx with `iex -S mix phx.server`

Now you can visit [`localhost:4000`](http://localhost:4000) from your browser.

Ready to run in production? Please [check our deployment guides](https://hexdocs.pm/phoenix/deployment.html).

## Learn more

  * Official website: https://www.phoenixframework.org/
  * Guides: https://hexdocs.pm/phoenix/overview.html
  * Docs: https://hexdocs.pm/phoenix
  * Forum: https://elixirforum.com/c/phoenix-forum
  * Source: https://github.com/phoenixframework/phoenix

## What to do to make it work
  * added docker-compose.yml for a postgres database
  * mix phx.gen.live Timeline Post posts username body likes_count:integer reposts_count:integer
  * add resulting the routes in router.ex
  * mix phx.server, localhost:4000
  * there will be a button to create the database and after that also to run the migrations if you haven't done it
  * changed lib/chirp_web/live/post_live/index.html.heex
  * ceated lib/chirp_web/live/post_live/form_component.html.heex
  * add broadcast in lib/chirp/timeline.ex and call it in insert and update
  * handle the subscribe in lib/chirp_web/live/post_live/index.ex
  
  
