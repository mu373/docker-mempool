# docker-mempool

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
