`CDN`的全称是content delivery network，内容分发网络。将各种缓存服务器分部到用户访问较为频繁的地区或者网络中，在用户访问网站时，利用全局负载技术将用户的访问指向最近工作正常的缓存服务器上

它的核心点有两个，一个是`缓存`，一个是`回源`。

这两个概念都非常好理解。对标到上面描述的过程，“缓存”就是说我们把资源 copy 一份到 CDN 服务器上这个过程，“回源”就是说 CDN 发现自己没有这个资源（一般是缓存的数据过期了），转头向根服务器（或者它的上层服务器）去要这个资源的过程。