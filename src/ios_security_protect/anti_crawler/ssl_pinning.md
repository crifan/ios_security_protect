# SSL证书绑定

* 背景
  * iOS的app，多数和服务器端通信，也是基于常见`HTTP`/`HTTPS`协议。
  * 而iOS逆向中往往会，用抓包工具，比如`Charles`去抓包分析你的网络请求。
    * 其中因为抓包可以直接看到明文数据而多数已不用`HTTP`了。
    * 而改用加密的`HTTPS`，而抓包`HTTPS`，一般来说无法直接看到明文数据，只能看到加密后的乱码。
    * 但是采用了根证书信任等手段，往往也可以抓包到`HTTPS`的明文。
    * 而最新的手段一般是：采用`证书绑定`=`SSL pinning`，app内部会对于SSL的证书和本地的证书做绑定和校验，使得抓包工具比如Charles的证书，无法通过验证，从而导致无法抓包到`HTTPS`的明文。
* 而iOS防护的话，不希望被抓包，被看到HTTPS的明文，所以往往也会去采用：`证书绑定`=`SSL pinning`
  * 而证书绑定中，更高级和更严格一点的手段是：`本地证书校验`？

## 如何绕过证书绑定

详见：

[绕过证书绑定 · 移动端逆向：绕过抓包限制](https://book.crifan.org/books/mobile_re_capture_bypass_limit/website/bypass_pinning/)
