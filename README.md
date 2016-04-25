# geekitpro
self web


link : http://geekitpro.github.io/geekitpro


绑定自己的域名

有一个功能其实很重要，就是绑定自己的域名。想想如果有天 github 网站被依法和谐了，那怎么办？如果一开始就是用自己的域名，那就简单了，直接换一台服务器就好了。

绑定域名的具体的操作步骤在这里 。

DNS 设置的方式并不唯一，但也是大同小异，下面演示一下我自己的操作过程。我的 gitbeijing.com 这个域名是在 godaddy.com 上买的。 首先在 godaddy.com 上，让 gitbeijing.com 使用 digitalocean 的 domain server : ns1.digitalocean.com 。

下一步，到 digitalocean 网站上，添加 A Record 指向 192.30.252.153 和 192.30.252.154



到 happypeter/gitbeijing项目的 gh-pages 分支，创建 CNAME 文件，里面的内容为

gitbeijing.com
这样操作结束，当然还要稍微等几个小时给 DNS 扩散。晚上做完上面的操作，第二天早上访问 http://gitbeijing.com 已经可以访问到我的网站了，如果访问 http://www.gitbeijing.com 则可以跳转到 http://gitbeijing.com ，效果完美。

