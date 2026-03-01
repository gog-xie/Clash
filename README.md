<h1 align="center"> ✈️基于mihomo内核代理程序<br>⠀<br>订阅配置说明</h1>

---

<p align="center"><b>🚴‍♀️本项目基于Aethersailor大佬的OpenClash配置文件，根据个人上网习惯及机场特性微改🚴‍♀️</b></p>
<p align="center"><b>🐜持续漏网之鱼🐟的维护补录，定制个人需求，如个别内网设备指定域名代理，其余直连的特殊需求🐜</b></p>
<p align="center"><b>😂规则模板可拓展至Windows Clash Verge、ASUS MerlinClash、OpenWrt Nikki、OpenClash等mihomo内核程序使用😂</b></p>

---

- ## 1 前言
#### &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;曾用Openwrt旁路由科学上网，旁路由存在诸多问题，且使用多有不便。家庭网络简单好用即可，改为仅一台华硕硬路由满足家庭上网需求，安装了Merlinclash科学上网，而在Merlinclash中不易配置分流规则，沿用了Openclash的配置文件，效果接近无感！至于广告拦截，在终端安装例如AdGuard插件效果远远好于OpenClash的效果，故可以在硬路由或终端上安装相关插件。
#### &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;本项目主要是相关订阅模板的下载，各代理程序的设置请自行查阅相关教程，如OpenClash的设置建议参照 [Aethersailor](https://github.com/Aethersailor/Custom_OpenClash_Rules/wiki/OpenClash-%E8%AE%BE%E7%BD%AE%E6%96%B9%E6%A1%88)大佬的设置方案🥊。

***

- ## 2 OpenClash订阅模板

- ### 2.1 Yaml模板（推荐）

#### &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;采用Subconverter订阅时有小毛病出现，用yaml配置文件导入可减少小问题，而且可配置较为美观的Zashboard控制面板。下载yaml文件后只需输入机场名称和机场订阅地址后导入OpenClash即可。

#### [2.1.1 Fallback地区故转模板](https://github.com/gog-xie/Clash/blob/main/yaml/OpenClash_FallBack.yaml)

```
https://github.com/gog-xie/Clash/blob/main/yaml/OpenClash_FallBack.yaml
```

#### [2.1.2 url-test地区自动模板](https://github.com/gog-xie/Clash/blob/main/yaml/OpenClash_Simple.yaml)

```
https://github.com/gog-xie/Clash/blob/main/yaml/OpenClash_Simple.yaml
```


- ### 2.2 Sub订阅转换ini链接
#### [2.2.1 Custom_Clash订阅链接](https://raw.githubusercontent.com/gog-xie/clash/refs/heads/main/CF/Custom_Clash.ini)

```
https://raw.githubusercontent.com/gog-xie/clash/refs/heads/main/CF/Custom_Clash.ini
```

```
https://testingcf.jsdelivr.net/gh/gog-xie/clash@main/CF/Custom_Clash.ini
```

#### [2.2.2 Custom_Clash_Simple订阅链接](https://raw.githubusercontent.com/gog-xie/clash/refs/heads/main/CF/Custom_Clash_Simple.ini)

```
https://raw.githubusercontent.com/gog-xie/clash/refs/heads/main/CF/Custom_Clash_Simple.ini
```

```
https://testingcf.jsdelivr.net/gh/gog-xie/clash@main/CF/Custom_Clash_Simple.ini
```

#### [2.2.3 Custom_Clash_FallBack订阅链接](https://raw.githubusercontent.com/gog-xie/clash/refs/heads/main/CF/Custom_Clash_FallBack.ini)

```
https://raw.githubusercontent.com/gog-xie/clash/refs/heads/main/CF/Custom_Clash_FallBack.ini
```

```
https://testingcf.jsdelivr.net/gh/gog-xie/clash@main/CF/Custom_Clash_FallBack.ini
```

-  ## 3 其他系统yaml模板
>   #### 若主路由为华硕硬路由，配置MerlinClash订阅规则完全可借鉴OpenClash的订阅模板，可直接导入模板使用或稍加改动即可。
>  * 在OpenClash配置订阅中的规则集选择“启用”，避免yaml文件太大影响速度，再到配置管理中下载yaml配置文件导入Merlinclash中可直接使用。目前Merlinclash中GoeIP数据库数量为0，官方解释为“mmdb等格式的geo文件无法统计数量”，但GoeSite和GoeIP数据正常调用，使用效果不受影响。同理，也可导入Windows Clash Verge中使用，导入Nikki时注意需带相关设置参数。这里推荐使用以下yaml文件，仅需修改yaml文件中的机场地址和名称即可：


#### [3.1.1 ClashVerge_FallBack模板](https://github.com/gog-xie/Clash/blob/main/yaml/ClashVerge_FallBack.yaml)

```
https://github.com/gog-xie/Clash/blob/main/yaml/ClashVerge_FallBack.yaml
```

#### [3.1.2 MerlinClash_FallBack模板](https://github.com/gog-xie/Clash/blob/main/yaml/MerlinClash_FallBack.yaml)

```
https://github.com/gog-xie/Clash/blob/main/yaml/MerlinClash_FallBack.yaml
```

#### [3.1.3 MerlinClash_Simple模板](https://github.com/gog-xie/Clash/blob/main/yaml/MerlinClash_Simple.yaml)

```
https://github.com/gog-xie/Clash/blob/main/yaml/MerlinClash_Simple.yaml
```

#### [3.1.4 Nikki_FallBack模板（推荐）](https://github.com/gog-xie/Clash/blob/main/yaml/Nikki_FallBack.yaml)

```
https://github.com/gog-xie/Clash/blob/main/yaml/Nikki_FallBack.yaml
```

<p align="center"> <b>MerlinClash GeoIP数量显示为0 </b></p>
<div align="center"> <img src="https://github.com/gog-xie/Clash/blob/main/pic/clash/merlinclash%E5%86%85%E7%BD%AE%E8%A7%84%E5%88%99%E8%B0%83%E7%94%A8.png" width="360" heiht="190"></div>

-  ## 4 特殊需求
>  * 在OpenClash、Nikki或MerlinClash系统中，常常有部分设备不需要科学代理，旁路由比较好设置，只需让需要代理设备的网关指向旁路由，不需代理的默认指向主路由即可；但也有设备仅少量代理需求，其余不走科学代理，或openclash安装在主路由情况下部分设备不走科学代理。特别是前者比较特殊，既要少量代理，又要大部分直连，比如白群仅docker镜像库、Emby海报刮削需要科学代理，其余全部绕过内核走直连的情况（主要是群晖按普通规则代理后，经常性的产生不必要的代理流量，实际上是不需要的），可以利用规则先后顺序正则匹配的特点来实现部分代理其他不代理，按先后顺序匹配指令，如果没有匹配上，再去匹配下一项规则。根据这一特点，先将这类设备IP 与MAC地址绑定，再让不需代理的设备IP匹配走直连，其次让部分需要代理的设备IP 匹配Proxy规则，最后让部分需要代理的设备IP匹配走直连。把这三项放规则集的最前端即可，例如以下规则：内网设备192.168.50.88走直连，设备192.168.50.98的部分域名（My_Proxy）走代理，其余走直连。

```
rules:
- SRC-IP-CIDR,192.168.50.88/32,DIRECT
- RULE-SET,My_Proxy,手动选择
- SRC-IP-CIDR,192.168.50.98/32,DIRECT
......
```
>  * 如果只有有少量的代理需求，可直接写域名或IP规则匹配：
```
rules:
- SRC-IP-CIDR,192.168.50.88/32,DIRECT
- DOMAIN-SUFFIX,themoviedb.org，国外媒体
- DOMAIN-SUFFIX,tmdb.org，国外媒体
- DOMAIN-SUFFIX,hub.docker.com，github
- SRC-IP-CIDR,192.168.50.98/32,DIRECT
......
```

                     
***

---
<p align="center"> <b>手机端Zashboard控制面板效果 </b></p>
<div align="center"> <img src="https://github.com/gog-xie/Clash/blob/main/pic/clash/zashboard3.png?raw=true" width="360" heiht="190"></div>

---

<p align="center"> <b>电脑端Zashboard控制面板局部效果 </b></p>
<div align="center"> <img src="https://github.com/gog-xie/Clash/blob/main/pic/clash/zashboard1.png?raw=true" width="720" heiht="380"></div>

---

<p align="center"> <b>电脑端Zashboard控制面板分流策略组 </b></p>
<div align="center"> <img src="https://github.com/gog-xie/Clash/blob/main/pic/clash/zashboard2.png?raw=true" width="720" heiht="380"></div>

---

<p align="center"> <b>电脑端Zashboard控制面板连接列表 </b></p>
<div align="center"> <img src="https://github.com/gog-xie/Clash/blob/main/pic/clash/zashboard4.png" width="1080" heiht="760"></div>

---
