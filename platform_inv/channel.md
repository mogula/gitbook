# 渠道管理

## 1. 库表
```
tb_ordercenter_channel
```

配置渠道的基本信息，渠道编码、渠道名称、渠道类型。渠道编码在表中是orderchannel字段，链接中的sou是orderchannel的32进制表示形式。可以用mysql的进制转换函数得到。
```
select conv(orderchannel, 10, 32) as sou from tb_ordercenter_channel
```
