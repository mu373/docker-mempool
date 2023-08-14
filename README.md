# docker-mempool

Run mempool on Docker using `bitcoind` on a separate container.
- `docker-compose.yml` is forked from [mempool/mempool](https://github.com/mempool/mempool/blob/master/docker/docker-compose.yml).
- Original documentation for the Docker configurations are available [here](https://github.com/mempool/mempool/tree/master/docker).
- For running `bitcoind` on Docker, you can use [mu373/docker-bitcoind](https://github.com/mu373/docker-bitcoind).



## Setup
Setup environment variables
```sh
cp .api.sample.env .api.env
vim .api.env # Edit the configuration to fit your needs
```

Start the container
```sh
# Make sure to start bitcoind container *before* starting this mempool container
docker compose up -d
```
Your Mempool instance should be running at [http://localhost:8181](http://localhost:8181).