# dd-signal

监控多个B站主播的直播状态，并发送开播、下播提醒消息的Telegram Bot。

>  这个机器人可以帮助早已把Telegram作为日常摸鱼工具的你dd一堆vtubers，解决B站客户端自带开播提醒基本没法用的问题。

我搭建的公开机器人：[@dd_signal_bot](https://t.me/dd_signal_bot)

## 特性

- 同时监控多个B站主播的直播状态
- 通过Telegram Bot原生方式添加、删除监控列表的。

## 部署

以在Linux上安装为例。

1.通过[@BotFather](https://t.me/BotFather)申请机器人，并记录`Telegram Bot API Token`。

2.安装Node.js和npm。[教程](https://nodejs.org/en/download/package-manager/)。

3.拉取本项目，并安装依赖。

```bash
git clone https://github.com/juzeon/dd-signal.git
cd dd-signal/
npm install
```

4.运行程序。

```bash
node ./index.js --token "您的Telegram Bot API Token"
```

您可以设定更多参数：

```bash
--interval <IntervalBySec> - 可选，每次访问B站API间隔的秒数，默认为5
--token <TelegramBotToken> - 必选，Telegram Bot Token
--proxy <HTTPProxy> - 可选，以 http:// 开头的代理
```

## 演示

帮助：

![](https://img11.360buyimg.com/ddimg/jfs/t1/159010/22/8547/76071/60371d58E0a373bfe/6e757d351feacaa2.png)

添加：

![](https://img12.360buyimg.com/ddimg/jfs/t1/166397/24/8126/160428/60366d3fE3f90e563/7b038365b7d299ac.png)

删除：

![](https://img10.360buyimg.com/ddimg/jfs/t1/150438/16/21013/58240/60371cf1Eb86ef6a5/41daf2bf461380df.png)

列表：

![](https://img10.360buyimg.com/ddimg/jfs/t1/168344/38/7845/126065/60366ef9E316cec24/954bb30110188d63.png)

开播、下播提醒：

![](https://img10.360buyimg.com/ddimg/jfs/t1/170050/11/7723/15309/60366fabE9e17d285/c4852b6b8c534c7d.png)