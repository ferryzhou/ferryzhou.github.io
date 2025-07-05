---
title: "microbit web bluetooth connect"
date: 2024-06-21
---

<p>昨天各种试都不work</p>
<p>要气死了</p>
<p>今天下班回来继续</p>
<p>一下子成功了</p>
<p>记一下几个关键地方免得回头又搞半天</p>
<p>第一从makecode下载代码的时候不按pair button，直接下载文件，拖到microbit drive里</p>
<p>第二把microbit插上电，不急着按ab和resetbutton去启动bluetooth连接，不用</p>
<p>第三点击webapp connect，就直接连接成功了！</p>
<p>后来下载自己的makecode js到microbit还是不行</p>
<p>code完全一样也不行！</p>
<p>弄了半天，发现是因为别人样本<a href="https://makecode.microbit.org/_C06XuChrjRvs">makecode</a>的一个设置不一样！</p>
<p>首先弄成js模式</p>
<p>然后左边explorer展开</p>
<p>里面有一个文件pxt.json</p>
<p>里面"JustWorks pairing (default): Pairing is automatic once the pairing is initiated."是off的</p>
<p>但是如果自己加bluetooth extension,那个选项是on的!</p>
<p>而且点不动!</p>
<p>只能点击"Edit Settings as text"</p>
<p>然后把里面一段设置copy过来</p>
<div>
<blockquote>
<div>    "yotta": {</div>
<div>        "config": {</div>
<div>            "microbit-dal": {</div>
<div>                "bluetooth": {</div>
<div>                    "open": 1,</div>
<div>                    "pairing_mode": 0,</div>
<div>                    "whitelist": 0</div>
<div>                }</div>
<div>            }</div>
<div>        }</div>
<div>    }</div>
<div> </div>
</blockquote>
</div>

<!-- wp:paragraph -->
<p>然后保存下载就可以了</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>这样在webapp里连接bluetooth的时候这个device就可以显示出来,pair就可以了</p>
<!-- /wp:paragraph -->
