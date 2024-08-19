# spr 所有信息

官方网站：[Spectre Network: Fast, Private, Decentralized Blockchain (spectre-network.org)](https://spectre-network.org/)

web钱包（推荐）：[Spectre Wallet (spectre-network.org)](https://wallet.spectre-network.org/)

手机钱包: [Release v0.3.15 · spectre-project/spectre-mobile (github.com)](https://github.com/spectre-project/spectre-mobile/releases)  温馨提示：手机钱包下载下来，不要使用vpn否则钱包不会同步

资源管理器：https://explorer.spectre-network.org/

github: [Spectre (github.com)](https://github.com/spectre-project)

twitter: https://twitter.com/SpectreNetwrk

收益计算器: https://spectre-network.org/#miningrewardcalculator

## 节点

### Windows节点

选择节点文件夹运行cmd脚本：

* 第一步下载仓库: https://gitee.com/muaimingjun/spectre-spr-information
* 第二步下载节点文件(可以选择覆盖掉节点data目录下面的数据文件)：https://spectre-network.org/downloads/legacy/datadir-rust.zip
* 第三步 进入node文件夹，选择节点运行脚本
* 第四步选择网桥 运行脚本

### linux 节点

*  安装docker 和 docker compose 这里推荐 使用1panel

  [在线安装 - 1Panel 文档](https://1panel.cn/docs/installation/online_installation/)

* 下载 docker comose 文件

* [docker comose](./dockers/docker-compose-bridge.yml)

* 然后复制到 1panal 容器编排里面设置容器名称即可

编排好之后呢容器全部关闭

关闭之后去下载节点文件: 

https://spectre-network.org/downloads/legacy/datadir-rust.zip

解压到节点对应目录，1panel 详情里面有挂在路径，解压到哪里面就可以了



## 挖矿

这里推荐使用tnn锄头，因为算力确实增加很多

- 锄头：[Release v0.4.0-dev · spectre-spr/spectre-spr-information (github.com)](https://github.com/spectre-spr/spectre-spr-information/releases/tag/v0.4.0-dev)
  =======
- 锄头：[spr-tnn-开发者2.5%](https://gitee.com/muaimingjun/spectre-spr-information/releases/tag/v0.4.0-dev)

```bash
  tnn-miner* --spectre --daemon-address node-ip  --port  5555 --wallet spectre:qxxxxxxxxxg --threads 10 --worker-name 矿工名称
```
#### tnn锄头算力

![本地路径](img/F18BE05112CD3183E527B50D6C2CCBE3.png)


- 锄头：[spr-官方-社区税 1%](https://github.com/spectre-project/spectre-miner/releases/tag/v0.3.16)

```bash
  
./spectre-miner-v0.3.16-linux-gnu-amd64 --mining-address  spectre:xxxxxxx  -s x.x.x.x -p xxxx

```
#### 官方锄头算力
![本地路径](img/4A9F4A66B14A1561F5AB9C3D45633C97.png)

  

### docker  运行 挖矿程序 支持 (x86_64 /  arm64)

```bash
docker run -itd --name spr  --restart=always   -e w=spectre:xxxxxxxxxxxxxxxxxxxxxxxx  -e s=192.168.2.3 -e p=5555 -e t=30 -e name=02 itgpt/tnn-miner:latest
```



注意文件里面要更改自己的网桥ip端口号还有自己的钱包地址，根据自己机器实际情况更改线程数量，和自己矿机名称。**

## 交易所

注册交易所

* 如果您没有注册 nonkyc 请使用我的推荐链接非常感谢您 ： https://nonkyc.io?ref=664caf26103e9be1dd7b5320
* 如果您没有注册 xeggex 请使用我的推荐链接非常感谢您：https://xeggex.com?ref=65f6b77cabe5789e24b76aff
* 交易所:  [xeggex](https://xeggex.com/market/SPR_USDT)
* 交易所币地址： [Trade SPR with USDT : NonKYCcryptocurrency exchange](https://nonkyc.io/market/SPR_USDT)
* 交易所： [Exbitron](https://exbitron.com/trade?market=SPR-USDT)






# ♥️ 支持项目\(Support\)

<p>如果 <b>spectre-spr-information</b> 对您有帮助，请考虑为它点个 <b>Star</b> ⭐，感谢您的支持！</p>
<table>
<thead>
<tr>
<th align="center">qq群 747579702 </th>
<th align="center">钱包</th>
</tr>
</thead>
<tbody><tr>
<td align="center"><img src="./img/qq.jpg" alt="qq群 747579702" height="324" width="250"></td>

<td align="center"><img src="./img/dashang.png" alt="钱包" height="400" width="480"></td>
</tr>
</tbody>
</table>
<p>如果您愿意，可以考虑提供资助 <b>spectre:qqsxlp2hpnpdzs3ur0sdjv6x479ywj92a0gfu6vlwahetz3n3mz2u8j3fwgwd</b> 提供额外的支持！</p>

