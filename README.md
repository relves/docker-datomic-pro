# docker-datomic-pro
Docker composed Datomic Pro DB, Datomic Console, Datomic REST endpoint inspired by [pointslope/docker-datomic-example](https://github.com/pointslope/docker-datomic-example).

# Steps

0. Check out this repo and cd into docker-datomic-pro folder
1. Get a Datomic Pro Starter Edition license at [my.datomic.com](https://my.datomic.com)
2. Set shell environment variables MY_DATOMIC_USER, MY_DATOMIC_DOWNLOAD_KEY, DATOMIC_VERSION, DATOMIC_LICENSE_KEY
3. Run "docker-compose up"
4. Everything should now be running. Datomic DB: datomic:dev://localhost:4334/, REST end point: [localhost:8001](http://localhost:8001), Console end point: [localhost:9000](http://localhost:9000/browse)

# Caveat emptor
As is, this is intended as a Datomic development environment configuration, not for production use.
