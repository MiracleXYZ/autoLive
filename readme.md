# autoLive

一个将YouTube内容转播到bilibili的小工具，原作者的使用说明在[这里](https://www.bilibili.com/read/cv1122933/)。

我将原脚本进行了一些修改，使之适应自动推流。（PS：同时加上了`-re`参数，好像并不影响播放还会更加顺滑，可能效果因直播而异，可以在`config.ini`中进行调整。）

## 用法

按照文章安装完环境之后，在`cookies.txt`中输入你的`cookies`，在`config.ini`中调整直播信息。

用`screen`进行自动推流：

```
screen -dmS rebroadcast python3 youtube.py
```

退出直播：

```
screen -X -S rebroadcast quit
```

## TO-DO

1. 提高连接稳定性
2. 增加自动重连机制
3. 局部打码/显示B站评论

