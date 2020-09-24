# 渠道链接
为了管理渠道链接，链接需要包含2个关键信息活动编码与渠道编码。

## 1. 库表
```
tb_ordercenter_fes_chan 活动与渠道关联的表
tb_channel_url 活动链接表，保存短网址
```

## 2. 结构
渠道链接中包含有活动编码（fes）与渠道编码（sou），如下：
```
http://localhost:8080/orderchannel/baidu/index.html?fes=9on&sou=33
```

fes 是活动表中fescod字段32进制的表示，sou 是渠道表中orderchannel字段32进制的表示。
  
mysql 可以通过conv函数进行进制转换。
select conv(fescod, 10, 32) from tb_ordercenter_festival
select conv(orderchannel, 10, 32) from tb_ordercenter_channel
