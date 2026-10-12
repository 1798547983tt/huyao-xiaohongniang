# 狐妖小红娘 · 资源仓库

存放《狐妖小红娘》SillyTavern 角色卡相关的资源。

## 目录

| 位置 | 内容 |
|---|---|
| `art/` | 状态栏背景图：苦情巨树 |
| `music/` | 配乐：人间白首、梦回还、若当来世（点「开始建档」后由状态栏播放） |
| `video/` | 开局页选篇视频（9 篇，重新封装过：索引在文件头、去掉了音轨） |
| `poster/` | 选篇视频的封面帧 `<篇>.jpg` 与选篇卡缩略图 `<篇>-thumb.jpg` |
| `keyart/` | 开局页动态插画（11 篇）：原图 `<篇>.webp`、深度图 `<篇>-depth.webp`、缩略图 `<篇>-thumb.webp` |

开局页的素材地址锁定在某一次提交（`@提交号`），不跟 `@main`：替换这些文件后，要在卡里的「狐妖开局」脚本改用新的提交号，旧卡仍读旧文件。

## art：状态栏背景图

| 文件 | 用于 |
|---|---|
| `kuqing-night.webp` / `.png` | 深色主题「夜·红线苦情树」 |
| `kuqing-day.webp` / `.png` | 浅色主题「涂山琉璃·狐火」 |
| `kuqing-manga.webp` / `.png` | 漫画主题「漫画·手绘分镜」 |

尺寸都是 1536 × 1024。`.png` 是原图；`.webp` 是压缩后的版本（每张约 250–380KB），状态栏优先读取它。

状态栏默认从这个仓库读图（经 jsDelivr 国内镜像）：

```text
https://testingcf.jsdelivr.net/gh/1798547983tt/huyao-xiaohongniang@main/art
```

更换图片：用同名文件覆盖并推送。jsDelivr 对 `@main` 有缓存，推送后可以逐个打开下面的地址刷新（把文件名换成实际改动的那张）：

```text
https://purge.jsdelivr.net/gh/1798547983tt/huyao-xiaohongniang@main/art/kuqing-night.webp
```
