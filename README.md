<div align="center">
<img src="./docs/logo.png" width=200 />

# ww_resources
# 鸣潮资源库

<p align="center">
  <a href="https://qm.qq.com/q/DVb9aGPmaQ">
    <img src="https://img.shields.io/badge/QQ%E7%BE%A4-743103809-orange">
  </a>
</p>
</div>



本仓库收集整理与 鸣潮/Wuthering Waves 相关的资源文件；

以及为 **早柚核心GsCore**插件[WutheringWavesUID](https://github.com/tyql688/WutheringWavesUID) 插件提供的第三方素材资源。



## 📁 资源目录结构

| 介绍                                                         | 文件夹           |
| ------------------------------------------------------------ | ---------------- |
| [WutheringWavesUID](https://github.com/tyql688/WutheringWavesUID) /ww帮助菜单顶图 | banner_bg        |
| [WutheringWavesUID](https://github.com/tyql688/WutheringWavesUID)/ww角色面板图片 | custom_role_pile |



## ✨ 使用方法

   - 将素材放入插件指定的资源目录

   - 参考插件文档配置资源路径

     

### 🖼 banner_bg  ww帮助菜单顶图

> [!NOTE]
>
> 路径：/gsuid_core/gsuid_core/plugins/WutheringWavesUID/WutheringWavesUID/wutheringwaves_help/texture2d/banner_bg.jpg

将本项目下载后，挑选 ww_resources/banner_bg 里面一张喜欢的图片 ，重命名为 banner_bg.jpg复制到 /gsuid_core/gsuid_core/plugins/WutheringWavesUID/WutheringWavesUID/wutheringwaves_help/texture2d/banner_bg.jpg 替换原文件即可。

#### 🖼参考图

![ww帮助](./docs/ww_help.jpg)



### 🖼 custom_role_pile ww角色面板图片

> [!NOTE]
>
> 路径 ：gsuid_core/data/WutheringWavesUID/custom_role_pile
>

将本项目下载后，手动将ww_resources/custom_role_pile复制到 gsuid_core/data/WutheringWavesUID/custom_role_pile/ 目录下即可。

#### 🖼参考图
面板参考图"ww散华面板":

![ww散华面板](./docs/ww_panel.jpeg)

#### Debian Linux 使用教程

> [!NOTE]
>
> 我的WutheringWavesUID存放角色面板图片的路径是 "/opt/picture/ww_resources/custom_role_pile/ "
>
> 仅提供参考，需按照实际位置进行修改



(1) 通过APT包管理器安装两个软件包`rsync` 和 `git`。

```bash
apt install -y rsync git
```


(2) 将GitHub仓库 anyliew/ww_resources 克隆到本地目录 /opt/picture/ww_resources/ ;如果目标目录不存在，git会自动创建

```bash
git clone https://github.com/anyliew/ww_resources /opt/picture/ww_resources/
```


(3) 将源目录 /opt/picture/ww_resources/custom_role_pile/ 的内容同步到目标目录 /opt/gsuid_core/data/WutheringWavesUID/custom_role_pile/。

```bash
rsync -av --delete --progress /opt/picture/ww_resources/custom_role_pile/ /opt/gsuid_core/data/WutheringWavesUID/custom_role_pile/
```

#### 1panel定时更新

自动化脚本，用于定期更新

```bash
cd /opt/picture/ww_resources/ && git pull
rsync -av --delete --progress /opt/picture/ww_resources/custom_role_pile/ /opt/gsuid_core/data/WutheringWavesUID/custom_role_pile/
```
![1panel计划任务](./docs/1panel_scheduled_task.png)


#### 📝 游戏角色名称与id对应表

> custom_role_pile
>
> 参考 WutheringWavesUID/utils/map/detail_json/char

|    名称     | id   |
| :---------: | ---- |
|    散华     | 1102 |
|    白芷     | 1103 |
|    凌阳     | 1104 |
|    折枝     | 1105 |
|    釉瑚     | 1106 |
|   珂莱塔    | 1107 |
|    炽霞     | 1202 |
|    安可     | 1203 |
|   莫特斐    | 1204 |
|    长离     | 1205 |
|   布兰特    | 1206 |
|    露帕     | 1207 |
|   卡卡罗    | 1301 |
|    吟霖     | 1302 |
|    渊武     | 1303 |
|    今汐     | 1304 |
|   相里要    | 1305 |
|    秧秧     | 1402 |
|    秋水     | 1403 |
|    忌炎     | 1404 |
|    鉴心     | 1405 |
| 漂泊者·气动 | 1406 |
|    夏空     | 1407 |
| 漂泊者·气动 | 1408 |
|  卡提希娅   | 1409 |
| 漂泊者·衍射 | 1501 |
| 漂泊者·衍射 | 1502 |
|   维里奈    | 1503 |
|    灯灯     | 1504 |
|   守岸人    | 1505 |
|    菲比     | 1506 |
|    赞妮     | 1507 |
|    桃祈     | 1601 |
|    丹瑾     | 1602 |
|     椿      | 1603 |
| 漂泊者·湮灭 | 1604 |
| 漂泊者·湮灭 | 1605 |
|   洛可可    | 1606 |
|  坎特蕾拉   | 1607 |



## 📌 注意事项

禁止将本仓库资源用于任何商业用途



## 📌声明

本仓库的表情素材等均来自网络，如有侵权请联系作者删除，如有侵权内容，请通过 Issues 联系删除！

