## 使用教程

安装依赖

```bash
sudo apt update
sudo apt install git -y
sudo snap install docker 
```

下载相关软件

```bash
git clone https://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@github.com/flyzstu/service.git
```

### hysteria 配置单端口

```bash
iptables -t nat -A PREROUTING -i eth0 -p udp --dport 20000:50000 -j DNAT --to-destination :5566
```

