

### 编译

```b
docker build -f Dockerfile-spr-tnn-miner -t spr-tnn-miner:latest .

docker build -f Dockerfile-spr-tnn-node -t spr-tnn-node:latest .

```



```bash
# spr节点
docker run -itd --name spectred-node  --restart=always  -p 18111:18111 -p 18110:18110 -v ~/.rusty-spectre:/root/.rusty-spectre spr-rust-node:v.0.3.6
# spr 网桥
docker run -itd --name spectrebridge -p 5555:5555 -p 2114:2114 -e server=0.0.0.0:18110 spr-tnn-node:latest
# spr 锄头
docker run  -itd --name spr \
	-e w=spectre:xxxxxxxxxx \
	-e t=1 -e name=02 -e s= xxx.xxx.xxx.xxx \
	-e p=5555 spr-tnn-miner:latest
```



