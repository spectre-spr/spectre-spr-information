### 下载 termux

选择适合的机器下载termux ：https://github.com/termux/termux-app/releases/tag/v0.118.1

安装上去之后打开 执行下面命令

```bash
apt update
apt upgrade -y
apt install -y git proot proot-distro wget curl
proot-distro install ubuntu  # 安装ubuntu系统
proot-distro login ubuntu   # 登录ubuntu系统
```



在ubuntu 里面执行下面命令

```bash
apt update
apt install -y wget  
```

下载并运行挖矿程序: 记得更改自己钱包

```bash
wget https://gitee.com/muaimingjun/spectre-spr-information/releases/download/v0.3.6/Tnn-miner-arm64-phone   # 下载锄头

chmod +x Tnn-miner*  # 添加可执行权限
./Tnn-miner-arm64-phone --spectre --daemon-address xxx.xxx.xxx.xxx  --port  5555 --wallet spectre:xxxxxxxxxxxxxxxxxxxxxxxxxg --threads 8

```



