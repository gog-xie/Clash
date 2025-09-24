<h1 align="center"> ✈️Openclash<br>⠀<br>配置说明</h1>

---

<p align="center"><b>🚴‍♀️本项目基于Aethersailor大佬配置文件根据个人上网习惯及机场特性微改🚴‍♀️</b></p>
<p align="center"><b>🐜持续漏网之鱼🐟的维护补录🐜</b></p>
<p align="center"><b>😂规则模板可拓展至Windows Clash Verge、MerlinClash等系统使用😂</b></p>
<p align="center"><b>🙏🙏🙏 感谢Aethersailor大佬 🙏🙏🙏</b></p>

---

#### 曾用Openwrt旁路由科学上网，旁路由国内测速相对直连测速带宽打了个2折，且使用多有不便。其实家庭网络简单好用即可，改为仅一台华硕硬路由满足家庭上网需求，安装了Merlinclash科学上网，而在Merlinclash中不易配置分流规则，沿用了Openclash的配置文件，效果接近无感！至于广告拦截，可以在硬路由或终端上安装相关插件。

***

- ## Aethersailor大佬教程
#### [教程链接：](https://github.com/Aethersailor/Custom_OpenClash_Rules/wiki/OpenClash-设置方案)
```
https://github.com/Aethersailor/Custom_OpenClash_Rules/wiki/OpenClash-设置方案
```
- ## 自用订阅模板地址

- ### Custom_Clash.in
#### [Github地址：](https://raw.githubusercontent.com/gog-xie/clash/refs/heads/main/CF/Custom_Clash.ini)

```
https://raw.githubusercontent.com/gog-xie/clash/refs/heads/main/CF/Custom_Clash.ini
```

#### [直连地址：](https://testingcf.jsdelivr.net/gh/gog-xie/clash@main/CF/Custom_Clash.ini)

```
https://testingcf.jsdelivr.net/gh/gog-xie/clash@main/CF/Custom_Clash.ini
```

- ### Custom_Clash_Full.in
#### [Github地址：](https://raw.githubusercontent.com/gog-xie/clash/refs/heads/main/CF/Custom_Clash_Full.ini)

```
https://raw.githubusercontent.com/gog-xie/clash/refs/heads/main/CF/Custom_Clash_Full.ini
```

#### [直连地址：](https://testingcf.jsdelivr.net/gh/gog-xie/clash@main/CF/Custom_Clash_Full.ini)

```
https://testingcf.jsdelivr.net/gh/gog-xie/clash@main/CF/Custom_Clash_Full.ini
```

- ### Custom_Clash_Smart.in
#### [Github地址：](https://raw.githubusercontent.com/gog-xie/clash/refs/heads/main/CF/Custom_Clash_Smart.ini)

```
https://raw.githubusercontent.com/gog-xie/clash/refs/heads/main/CF/Custom_Clash_Smart.ini
```

#### [直连地址：](https://testingcf.jsdelivr.net/gh/gog-xie/clash@main/CF/Custom_Clash_Smart.ini)

```
https://testingcf.jsdelivr.net/gh/gog-xie/clash@main/CF/Custom_Clash_Smart.ini
```


-  ## 其他系统订阅模板配置
> *  主路由为华硕硬路由，配置MerlinClash订阅规则完全可借鉴OpenClash的订阅模板，可直接导入模板使用或稍加改动即可。
> *  分两种情况，在Openclash配置订阅里，使用规则集选“禁用”时，openclash中配置好的yaml文件可直接下载导入Clash Verge或Merlinclash中使用。如果使用规则集选“启用”时，Openclash的yaml配置订阅文件需稍加修改，需要将OpenClash中的yaml配置文件中rules的RULE-SET改为具体的规则数据（参照Aethersailor大佬及本项目rule的Custom_Direct_Classical.yaml及My_Direct.yaml等文件）及策略组（尽可能不要改变规则的先后顺序），并删除rule-providers相关数据后，可直接导入Windows Clash Verge、华硕路由器Merlinclash等系统的订阅规则文件，目前Merlinclash中GoeIP数据库数量为0，官方解释为“mmdb等格式的geo文件无法统计数量”，但GoeSite和GoeIP数据正常调用，使用效果不受影响。
<p align="center"> <b>是否启用规则集 </b></p>
<div align="center"> <img src="https://github.com/gog-xie/clash/blob/main/pic/clash/%E8%A7%84%E5%88%99%E9%9B%86.png" width="720" heiht="380"></div>


<p align="center"> <b>替换RULE-SET规则集 </b></p>
<div align="center"> <img src="https://github.com/gog-xie/clash/blob/main/pic/clash/RULE-SET.png" width="720" heiht="380"></div>



<p align="center"> <b>删除rule-providers规则集连接</b></p>
<div align="center"> <img src="https://github.com/gog-xie/clash/blob/main/pic/clash/rule-providers.png" width="720" heiht="380"></div>


                     
***

