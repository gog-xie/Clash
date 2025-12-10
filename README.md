<h1 align="center"> ✈️Openclash<br>⠀<br>配置说明</h1>

---

<p align="center"><b>🚴‍♀️本项目基于Aethersailor大佬配置文件根据个人上网习惯及机场特性微改🚴‍♀️</b></p>
<p align="center"><b>🐜持续漏网之鱼🐟的维护补录🐜</b></p>
<p align="center"><b>😂规则模板可拓展至Windows Clash Verge、MerlinClash等系统使用😂</b></p>

---

#### 曾用Openwrt旁路由科学上网，旁路由存在诸多问题，且使用多有不便。家庭网络简单好用即可，改为仅一台华硕硬路由满足家庭上网需求，安装了Merlinclash科学上网，而在Merlinclash中不易配置分流规则，沿用了Openclash的配置文件，效果接近无感！至于广告拦截，在终端安装例如AdGuard插件效果远远好于OpenClash的效果，故可以在硬路由或终端上安装相关插件。

***


- ## 相关订阅模板地址

- ### Yaml模板（推荐）

#### 采用Fallback模式，用Subconverter订阅有时出现小毛病，尽可能用yaml配置文件导入，zashboard控制面板还相对美观。下载yaml文件后只需输入机场名称和机场订阅地址后导入OpenClash即可。

#### [OpenClash-Fallback模板地址：](https://github.com/gog-xie/clash/blob/main/CF/yaml/GOG_Clash_FallBack.yaml)

```
https://github.com/gog-xie/clash/blob/main/CF/yaml/GOG_Clash_FallBack.yaml
```

#### [OpenClash-模板地址：](https://github.com/gog-xie/clash/blob/main/CF/yaml/GOG_Clash_FallBack.yaml)

```
https://github.com/gog-xie/clash/blob/main/CF/yaml/GOG_Clash_FallBack.yaml
```


- ### Custom_Clash.in
#### [Github地址：](https://raw.githubusercontent.com/gog-xie/clash/refs/heads/main/CF/Custom_Clash.ini)

```
https://raw.githubusercontent.com/gog-xie/clash/refs/heads/main/CF/Custom_Clash.ini
```

#### [直连地址：](https://testingcf.jsdelivr.net/gh/gog-xie/clash@main/CF/Custom_Clash.ini)

```
https://testingcf.jsdelivr.net/gh/gog-xie/clash@main/CF/Custom_Clash.ini
```

- ### Custom_Clash_Simple.ini
#### [Github地址：](https://raw.githubusercontent.com/gog-xie/clash/refs/heads/main/CF/Custom_Clash_Simple.ini)

```
https://raw.githubusercontent.com/gog-xie/clash/refs/heads/main/CF/Custom_Clash_Simple.ini
```

#### [直连地址：](https://testingcf.jsdelivr.net/gh/gog-xie/clash@main/CF/Custom_Clash_Simple.ini)

```
https://testingcf.jsdelivr.net/gh/gog-xie/clash@main/CF/Custom_Clash_Simple.ini
```

- ### Custom_Clash_FallBack.ini
#### [Github地址：](https://raw.githubusercontent.com/gog-xie/clash/refs/heads/main/CF/Custom_Clash_FallBack.ini)

```
https://raw.githubusercontent.com/gog-xie/clash/refs/heads/main/CF/Custom_Clash_FallBack.ini
```

#### [直连地址：](https://testingcf.jsdelivr.net/gh/gog-xie/clash@main/CF/Custom_Clash_FallBack.ini)

```
https://testingcf.jsdelivr.net/gh/gog-xie/clash@main/CF/Custom_Clash_FallBack.ini
```

-  ## 其他系统订阅模板配置
>   #### 若主路由为华硕硬路由，配置MerlinClash订阅规则完全可借鉴OpenClash的订阅模板，可直接导入模板使用或稍加改动即可。
>  * 在OpenClash配置订阅中的规则集选择“启用”，避免yaml文件太大影响速度，再到配置管理中下载yaml配置文件导入Merlinclash中可直接使用。目前Merlinclash中GoeIP数据库数量为0，官方解释为“mmdb等格式的geo文件无法统计数量”，但GoeSite和GoeIP数据正常调用，使用效果不受影响。同理，也可导入Windows Clash Verge中使用。但这里推荐使用以下yaml文件，仅需修改yaml文件中的机场地址即可：


#### [ClashVerge模板地址：](https://github.com/gog-xie/clash/blob/main/CF/yaml/ClashVerge.yaml)

```
https://github.com/gog-xie/clash/blob/main/CF/yaml/ClashVerge.yaml
```

#### [MerlinClash模板地址：](https://github.com/gog-xie/clash/blob/main/CF/yaml/MerlinClash.yaml)

```
https://github.com/gog-xie/clash/blob/main/CF/yaml/MerlinClash.yaml
```
<p align="center"> <b>MerlinClash GeoIP数量显示为0 </b></p>
<div align="center"> <img src="https://github.com/gog-xie/Clash/blob/main/pic/clash/merlinclash%E5%86%85%E7%BD%AE%E8%A7%84%E5%88%99%E8%B0%83%E7%94%A8.png" width="360" heiht="190"></div>


-  ## 特殊需求
>  * 在OpenClash或MerlinClash中，常常有部分设备不需要科学代理，旁路由比较好设置，只需让需要代理设备的网关指向旁路由，不需代理的默认指向主路由即可；但也有设备仅少量代理需求，其余不走科学代理，或openclash安装在主路由情况下部分设备不走科学代理。特别是前者比较特殊，既要少量代理，又要大部分直连，比如白群仅docker镜像库、Emby海报刮削需要科学代理，其余全部绕过内核走直连的情况（主要是群晖按普通规则代理后，经常性的产生github流量，实际上是不需要的），可以利用规则先后顺序正则匹配的特点来实现部分代理其他不代理，按先后顺序匹配指令，如果没有匹配上，再去匹配下一项规则。根据这一特点，先将这类设备IP 与MAC地址绑定，再让不需代理的设备IP匹配走直连，其次让部分需要代理的设备IP 匹配Proxy规则，最后让部分需要代理的设备IP匹配走直连。把这三项放规则集的最前端即可，例如以下规则：内网设备192.168.50.88走直连，设备192.168.50.8的部分域名（My_Proxy）走代理，其余走直连。

```
rules:
- SRC-IP-CIDR,192.168.50.88/32,DIRECT
- RULE-SET,My_Proxy,手动选择
- SRC-IP-CIDR,192.168.50.8/32,DIRECT
......
```
>  * 如果只有有少量的代理需求，可直接写域名或IP规则匹配：
```
rules:
- SRC-IP-CIDR,192.168.50.88/32,DIRECT
- DOMAIN-SUFFIX,themoviedb.org，国外媒体
- DOMAIN-SUFFIX,tmdb.org，国外媒体
- DOMAIN-SUFFIX,hub.docker.com，github
- SRC-IP-CIDR,192.168.50.8/32,DIRECT
......
```

                     
***

