Jian，遵循黑白调、简洁风、高性能、以纯写作为主而诞生的一款Ghost主题；

计划写这种风格的主题已经好长时间了（其实也就一个多月），由于强迫症的原因，一直是写到百分之？的时候就删掉重写；

因为原来万网的虚拟主机快到期了，又恰巧碰到阿里云的免费产品试用6个月的活动，赶紧去申请资格，但是很遗憾，我居然不符合条件，原因是以前买过一次ECS;赶紧把我姐的支付宝账号借来开启阿里云，花了九块钱买了个啥产品我也忘了，获得了免费6个月的ECS试用资格；6个月过后就要省吃俭用续费喽！！！

换上ECS后呢，赶紧把原来的Typecho换成我等待已久的Ghost，因为半年前接触的Ghost，因为没有闲钱买阿里云ECS，又不甘心辛苦备案的域名绑到外国VPS上，所以就在用虚拟主机支持的PHP；

以前写过一个Ghost主题[White-Block](https://github.com/Weic96/Whie-Block) ,还是刚接触前端不久写的，现在看起来太囧了；

#### 预览图

**首页**

![](http://dl.weic96.cn/website/1/bb/7bb998d16557653269117060c7208.png)
**菜单栏展开后的首页**

![](http://dl.weic96.cn/website/1/f8/1f8ac4a3b93fc3f9faf329e16b7d2.png)
**文章页**

![](http://dl.weic96.cn/website/5/a1/aa76bd55ea1b96a9deee519a7f874.png)


#### 功能和特色

* 黑白色调为主；
* 炫酷的侧边滑动菜单栏设计；
* 响应式设计,这年头的网站没有响应式简直就是难(la)受(ji),无论是你桌子上摆的、包包里放的还是裤衩里装的统统可以适配;
* 高大少的Pjax技术；
* 代码高亮，专为程序猿准备；
* 不丰富的社交按钮，只有4个；
* 支持嵌入第三方评论，优先支持多说；
* Alpha版本，更多功能和优化请期待，谢谢！


#### 所含开源项目
- jQuery
- jQuery.pjax.js
- highlight.pack.js
- waves.min.js
- FontAwesome


#### 使用注意
本主题提供免费使用，但是不能魔改和修改底部版权信息，转载请注明项目主页；请务必遵守，这是对作者最起码的尊重；

本主题同时也提供收费版，其实就是卖个版权，收费版可以魔改和去除页面底部的版权信息；如需要购买请看下面；


#### 下载与购买

请[点击我](https://github.com/weic96/Jian)前往Github项目地址下载，可以的话来一个star可好？

收费版只需22元，如需购买请QQ联系或电子邮件联系我，购买后我会将你的域名留在本页面；

* QQ : 1104365773
* E-mail : [i@weic96.cn](mailto:i@weic96.cn)

#### 更新日志
* 2017.01.10 发布Alpha 0.12;
* 2017.01.11 发布Alpha 0.2;

#### 食用方法

#####安装
到Github或OSC@Git下载主题后在网页后台直接上传或使用FTP上传到你的Ghost目录下的==content/themes==目录里，然后解压；

上传后你还需要在你的Ghost网页后台更换主题；

###### 修改侧边栏里的微博、Github、邮箱地址
打开本主题的==partials==目录里的==navigation.hbs==文件，根据注释修改href属性；

    <div class="page-nav-icon">
            {{!-- 微博 --}}
            <a href="" class="fa fa-weibo"></a>
            {{!-- Github --}}
            <a href="" class="fa fa-github"</a>
            {{!-- 邮箱 --}}
            <a href="" class="fa fa-envelope"></a>
            {{!-- RSS --}}
            <a href="{{@blog.url}}/rss" class="fa fa-rss"></a>
    </div>

###### 嵌入第三方评论代码
获得第三方评论代码后，这里以多说为例，打开本主题==partials==目录里的==comments.hbs==文件，将第三方评论代码追击到最底部；（向下面这样）

    <a href="javascript:;" class="post-page-comments-title">评论</a>
    <!-- 下面是第三方评论代码 -->

    <div class="post-page-comments">
            <div class="ds-thread" data-thread-key="{{title}}" data-title="{{title}}" data-url="{{url}}"></div>
	        <script type="text/javascript">
	              var duoshuoQuery = {short_name:"xxx"};
		          (function() {
		               var ds = document.createElement('script');
		               ds.type = 'text/javascript';ds.async = true;
		               ds.src = (document.location.protocol == 'https:' ? 'https:' : 'http:') + '//static.duoshuo.com/embed.js';
		               ds.charset = 'UTF-8';
		               (document.getElementsByTagName('head')[0]
		|| document.getElementsByTagName('body')[0]).appendChild(ds);
		})();
	        </script>
     </div>

###### 侧边栏（导航菜单栏）
导航栏里的导航链接是Ghost后台设置的Navigation，所以直接在后台添加链接即可；

头像是用的blog@logo，你只需上传blog@logo就行了；

###### 标签云页面
首先需要看一篇文章[《为Ghost博客增加标签云》](https://weic96.cn/ghost-cloud-tags/) ，然后新建一个独立页面，这个独立页面的URL为==tags== ；

###### 友情链接页面
新建一个独立页面，这个独立页面的URL为==links== ；
