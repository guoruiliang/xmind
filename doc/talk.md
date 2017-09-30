
## 升级OTA

``` 
\\10.200.1.11\Share\ApplicationDev\Kyle.Yu\sau40t1-ota_20170912_1505205988_158.zip
新的ota 包，需手动更新
测试Alexa 语言功能
1. 手动升级OTA 包
2. 获取到token，将token手动写入到屏幕上有两个小孔的设备
3. alexa 功能现在只能使用standalone 模式测试，需要使用那个有两个小孔的设置测试
手动更新OTA
1. C:\Users\kyle.yu>adb push C:\Users\kyle.yu\Desktop\ota.zip /cache/recovery/
2. C:\Users\kyle.yu>adb shell sync
3. C:\Users\kyle.yu>adb shell "echo \"--update_package=/cache/recovery/ota.zip\"  /cache/recovery/command"
4. C:\Users\kyle.yu>adb reboot recovery
```



## ayla.conf

this is for production sever with new model name
but we still need the server side chnage
OK, you may try for gateway binding
push it to /cache/conf/ayla.conf
remember to save your old config file
then do a factory reset
in order to use new config file

/data/gateway/access_token
mv /data/gateway/access_token_tmp

## gateway not bind

data/gatway 删除data3 data4