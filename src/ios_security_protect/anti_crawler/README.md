# 反爬

iOS防护中，还有一部分的手段叫做：`反爬`

* `反爬`
  * 目的：
    * 防止别人的爬虫爬取你的app的数据
    * 防止别人能用抓包工具抓包你的app，看到明文的数据
  * 手段
    * https
      * `SSL pinning`=`certificate pinning`=`证书绑定`
      * `证书校验`
