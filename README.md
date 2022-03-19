## ✨  BabyProxy ✨  · ETH Pool Charge Commission、Mining Pool Redirect，One key build private mining pool

![minerProxy.PNGZz](https://bcn.135editor.com/files/users/1169/11697638/202203/Og7B9gZC_M93k.jpg "参数说明.jpg" )

- ✔ New resource code move here， Old repo was deleted：rgerd/babyProxy
- ⚡ Use for Mining Pool Proxy、Redirect、Pool Charge Commission

### Linux Server Deploy Guide

1、Prepare your Linux Server(you can use google cloud server)
- Recommend Server：Centos 7.x 
- Region：US、HK、UN、ASIA

2、RUN command one by one：

#### 👆 Step 1：Config your server ENV, Run command below 1 by 1：

- Just: ctrl + c && ctrl + v

```nashorn js
echo "root soft nofile 102400" >>/etc/security/limits.conf
echo "root hard nofile 102400" >>/etc/security/limits.conf
echo "DefaultLimitNOFILE=102400" >>/etc/systemd/system.conf
echo "DefaultLimitNPROC=102400" >>/etc/systemd/system.conf
echo "DefaultLimitNOFILE=102400" >>/etc/systemd/user.conf
echo "DefaultLimitNPROC=102400" >>/etc/systemd/user.conf

```

### ✌Step 2：Clone github resource Code
```bash
# Clone code to your server
git clone https://github.com/babyProxy/babyProxy.git
# go in 
cd babyProxy
# Grant program execution permission
chmod +x babyProxy
```
At this point, the code + server is ready, and you can start mining happily.

### 👌Step 3：Enable babyProxy mining pool forwarding
- The template has been prepared for everyone in advance, just replace it with your own wallet address
- Parameter Description

![参数说明.png](https://bcn.135editor.com/files/users/1169/11697638/202203/6jLBrL4c_JgJv.png "参数说明.jpg" )

- F2pool：f2pool-6688.sh
- Poolin：poolin-1883.sh
- Ethermine： ethermine-14444.sh

❗ Execute the following commands as needed:
```bash
nohup f2pool-6688.sh &
nohup poolin-1883.sh &
nohup ethermine-14444.sh &
```

### Special attention items

❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗

- Please remember to open the corresponding port for the mining pool forwarding service, such as etherming.org open 4444, 5555, Biyin open 1883, etc.
- Operate the security group in the server cloud service provider console, release the corresponding port(If you don't know how to do this, just Google it)

❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗❗

#### Last Step
- 💬 If you have any questions, please email directly
- 📫 Email：588@usd.dog
- 😄 Donate:
    - BTC：34URScr9mwe6SJUNDRx71iGCDjjt74aYhi
    - ETH：0x4d2755c4FFFF163a7637acd1388D547B894157B2
    - Gitcoin：0x4d2755c4FFFF163a7637acd1388D547B894157B2

