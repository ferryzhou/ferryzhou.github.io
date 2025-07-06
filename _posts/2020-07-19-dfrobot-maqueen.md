---
title: "Dfrobot maqueen"
date: 2020-07-19
---

<!-- wp:image {"id":7605,"sizeSlug":"large"} -->
<figure class="wp-block-image size-large"><img src="https://ferryzhou.wordpress.com/wp-content/uploads/2020/07/img_20200719_105051-1.jpg" alt="" class="wp-image-7605" /></figure>
<!-- /wp:image -->

<!-- wp:paragraph -->
<p>很便宜，才三十块</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>之前买过microbit，兼容</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>机器人不大，但是五脏俱全</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>有轮子，有range sensor，有line tracing，扬声器</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>再加上microbit本身的蓝牙，六宫格的LED，控制芯片</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>直接把microbit板子插在机器人主板上就算集成了，非常方便，不用连任何线</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>不过开始写程序费了些劲</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>用的Mac电脑</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>无论是下载的mind+本地应用程序还是网页程序都不work</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>之前用过microbit网站上编过程序，其实很简单，写完下载一个hex文件copy到microbit盘就行了。用一根micro USB线连接microbit和电脑。microbit就成了一个小U盘。</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>所以其实只要写完程序，能编译成hex就行</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>可以官方提供的编程环境怎么也找不到hex输出方式</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>连接microbit也不行。寻找device manager和serial port，感觉都是Windows上的东西。也没有Mac的教程。</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>而microbit网站的问题是没看到怎么支持macqueen</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>后来注意到mind+需要先选择一个模块，比如maqueen，然后就出现了几个maqueen的指令。</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>于是又上microbit make code网站，看看能不能加extension</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>很快找到了，点击advanced，添加extensions</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>但是页面里没有dfrobot</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>搜也搜不到</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>把mind+里面的code copy到microbit make code网页显示编译问题</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>回头又搜dfrobot microbit extension</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>搜到一些东西，但是不知道怎么使用，只有GitHub项目</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>后来又搜了一些又读文档</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>官方文档说只要是支持的extension，就可以load进来</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>而github那个项目是支持的！</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>我注意到GitHub项目名含有mcqueen</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>就在add extension的页面搜了一下maqueen</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>真出来了！</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>这样就可以进行maqueen编程了！</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>关键是可以下载安装到microbit里面去</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>快速试了一个简单的转动一个轮子</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>下载，copy，拔线，把microbit插到maqueen，打开开关</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>机器人真的开始转动了！</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>我们都兴奋的不得了</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>今天上午又尝试了更多东西</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>半个小时，就迭代了好几个版本</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>从最开始的双轮向前行走</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>到第六版检测到障碍就显示障碍距离，后退转弯发声</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>这样一个完整的避障机器人就成功了</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>code也非常简单，不到十行，毛毛和豆豆都能懂</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>真不错</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>豆豆问，加强版机器人什么时候到呀？</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>我说，你们先把简化版的玩好，玩熟了我们就买强化版的</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>强化版的还支持视觉，视觉模块五十块，还有物体识别功能</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>真没想到现在的机器人能这么便宜，模块化，而且易于操作和编程，连小朋友都可以。</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>前不久看了一个文章，science的，视频里kuka机器人代替科研人员做实验，效率比人高很多倍，还找到了更好的试剂</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>感觉机器人这一波不远了</p>
<!-- /wp:paragraph -->

<!-- wp:image {"id":7604,"sizeSlug":"large"} -->
<figure class="wp-block-image size-large"><img src="https://ferryzhou.wordpress.com/wp-content/uploads/2020/07/img_20200719_110016.jpg" alt="" class="wp-image-7604" /></figure>
<!-- /wp:image -->
