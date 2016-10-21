# docker-datomic-pro
Docker composed Datomic Pro DB, Datomic Console, Datomic REST endpoint based on ideas from [pointslope/docker-datomic-example](https://github.com/pointslope/docker-datomic-example).

# Steps

0. Check out this repo and cd into docker-datomic-pro folder
1. Get a Datomic Pro Starter Edition license at [my.datomic.com](https://my.datomic.com)
2. Set shell environment variables MY_DATOMIC_USER, MY_DATOMIC_DOWNLOAD_KEY, DATOMIC_VERSION, DATOMIC_LICENSE_KEY
3. Run "docker-compose up"
4. Datomic should now be running. See the consol for output related to host/ports: Datomic DB: datomic:dev://datomicdb:4334/, REST end point: [localhost:8001](localhost:8001), Console end point: [localhost:9000](localhost:9000)
