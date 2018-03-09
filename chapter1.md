# java取得arduino的rxtx資訊

# Ｍac 環境下

* ### [Arduino官網介紹](http://playground.arduino.cc/Interfacing/Java)
* 需要先下載rxtx的lib

* mac設定環境
* 增加rxtx lib需要用到而mac沒有的資料夾

#### 1.下載資源：GitHub   [https://git.oschina.net/myaniu/RXTX](https://git.oschina.net/myaniu/RXTX)

#### 2.將RXTXcomm.jar 和 librxtxSerial.jnilib複製到/Library/Java/Extensions目錄下， 並給存取權

```
sudo cp RXTXcomm.jar /Library/Java/Extensions/
sudo cp librxtxSerial.jnilib /Library/Java/Extensions/
sudo chmod -R 755 /Library/Java/Extensions
```

#### 3.網路上查的

The RXTX library requires access to the`/var/lock`directory, but it does not exists on a Mac!!!

So you only need to create it properly:

```
sudo mkdir /var/lock
sudo chmod go+rwx /var/lock
```

#### 4.把Arduino官網的java範例修改 PORT\_NAMES 跟 DATA\_RATE （鮑率）

mac 上的 com port 的PORT\_NAMES 可以去/dev/裡面找

```
ls /dev/tty.usb*
```



