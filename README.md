<img src="https://user-images.githubusercontent.com/633843/32198822-e59a0fc4-be1d-11e7-9b92-03ce17ba05ba.png" alt="screenshot"/>

#### fork自 jpillora/cloud-torrent

**Cloud torrent** 是Go（golang）编写的一个自托管的远程torrent客户端。您可以远程启动，将其作为服务器本地磁盘上的文件集下载，然后通过HTTP进行检索或流式传输。

### 特性

* 单文件
* 跨平台
* 提供种子搜索
* Real-time updates
* 移动端友好
* 快速 [content server](http://golang.org/pkg/net/http/#ServeContent)


### 安装

**Binaries**

你可已从release下载二进制的binaries

查看 [最新release](https://github.com/weihuagu/cloud-torrent/releases/latest) 或者通过以下命令行下载安装

```
sudo curl https://i.jpillora.com/WeihuaGu/cloud-torrent! | sudo bash
```

*Tip*: [开机自启动 `cloud-torrent` 教程](https://github.com/jpillora/cloud-torrent/wiki/Auto-Run-on-Reboot)



**从源代码安装**

*[Go](https://golang.org/dl/) is required to install from source*

``` sh
$ go get -v github.com/weihuagu/cloud-torrent
```


### 用法

```
$ cloud-torrent --help

  Usage: cloud-torrent [options]

  Options:
  --title, -t        Title of this instance (default Cloud Torrent, env TITLE)
  --port, -p         Listening port (default 3000, env PORT)
  --host, -h         Listening interface (default all)
  --auth, -a         Optional basic auth in form 'user:password' (env AUTH)
  --config-path, -c  Configuration file path (default cloud-torrent.json)
  --key-path, -k     TLS Key file path
  --cert-path, -r    TLS Certicate file path
  --log, -l          Enable request logging
  --open, -o         Open now with your default browser
  --help
  --version, -v

  Version:
    0.X.Y

  用法示例:
  1.执行 cloud-torrent --port 7000 --config-path cloud-torrent.json --title "Cloud Torrent" --log 
  2.在浏览器打来http://localhost:7000

    

```


#### 捐赠原作者

If you'd like to buy me a coffee or more, you can donate via [PayPal](https://www.paypal.com/cgi-bin/webscr?cmd=_xclick&business=dev%40jpillora%2ecom&lc=AU&item_name=Open%20Source%20Donation&button_subtype=services&currency_code=USD&bn=PP%2dBuyNowBF%3abtn_buynowCC_LG%2egif%3aNonHosted) or BitCoin `1AxEWoz121JSC3rV8e9MkaN9GAc5Jxvs4`.

### Notes

This project is the rewrite of the original [Node version](https://github.com/jpillora/node-torrent-cloud).

![overview](https://docs.google.com/drawings/d/1ekyeGiehwQRyi6YfFA4_tQaaEpUaS8qihwJ-s3FT_VU/pub?w=606&h=305)

Credits to @anacrolix for https://github.com/anacrolix/torrent

Copyright (c) 2017 Jaime Pillora
