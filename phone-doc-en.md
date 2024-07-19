###  Download termux

download Termux: <https://github.com/termux/termux-app/releases/tag/v0.118.1>

After installation, open Termux and execute the following commands:

```bash
apt update
apt upgrade -y
apt install -y git proot proot-distro wget curl
proot-distro install ubuntu  # Install Ubuntu system
proot-distro login ubuntu   # Log in to the Ubuntu system

```

Execute the following command within Ubuntu:

```ba
apt update
apt install -y wget  
```

Download and run the mining program: Remember to change your own wallet address

```bash
wget https://gitee.com/muaimingjun/spectre-spr-information/releases/download/v0.3.6/Tnn-miner-arm64-phone   # Download the miner

chmod +x Tnn-miner*  # Add executable permissions
./Tnn-miner-arm64-phone --spectre --daemon-address xxx.xxx.xxx.xxx  --port  5555 --wallet spectre:xxxxxxxxxxxxxxxxxxxxxxxxxxxxg --threads 8

```

