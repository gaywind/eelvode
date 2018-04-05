# EeLvode


## Requirements
1. `elixir >= 1.4.2`
2. `phoenix >= 1.3.0-rc.1`
3. `postgresql >= 9.6`
4. `node >= 7.2.0`
5. `yarn >= 0.17.9`

## Install
1. `mix deps.get`
2. `mix ecto.create && mix ecto.migrate`
3. `yarn install`

## Develop
1. `cd ~/eelvode && mix phx.server`


## Docker 
```bash
docker-compose up -d eelvode
docker-compose run eelvode mix ecto.create
docker-compose run eelvode mix ecto.migrate
docker-compose run eelvode mix run apps/priv/repo/seeds.exs
docker-compose restart eelvode
```

