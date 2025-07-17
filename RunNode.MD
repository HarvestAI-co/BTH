Recommended go version:
` 1.20 - 1.21.3 `


First step:
```shell 
make all
```

and then init genesis data:
```shell
./build/bin/geth --datadir ./data init genesis.json
```


Run the node sync:
```shell
./build/bin/geth --datadir ./data --config ./data/config.toml --cache 8192 --syncmode "full" --gcmode=archive -ipcdisable console
```
