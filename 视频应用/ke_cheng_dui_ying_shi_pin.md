# gitbook插入视频


* 方法三

```
<divstyle="text-align: center;">
<embedid="movie"src="http://player.youku.com/player.php/sid/XMjg4NzkzMjQ4/v.swf"allowfullscreen="true"quality="high"width="90%"align="middle"allowscriptaccess="always"type="application/x-shockwave-flash"/>
</div>
<scripttype="text/javascript">document.getElementById("movie").style.height=document.getElementById("movie").scrollWidth*0.8+"px"</script>


```


<iframe height=498 width=510 src="http://player.youku.com/embed/XMTI4MjU5OTA3Mg==" frameborder=0 allowfullscreen></iframe>


<script type="text/javascript">
window.onload = window.onresize = function () {
    resizeIframe();
}
var resizeIframe=function(){
    var bodyw=document.body.clientWidth;
    for(var ilength=0;ilength<=document.getElementsByTagName("iframe").length;ilength++){

        document.getElementsByTagName("iframe")[ilength].height = bodyw*9/16;//设定高度

    }
}
</script>



* 方法一：

```
<iframe height=498 width=510 src="http://player.youku.com/embed/XNjcyMDU4Njg0" frameborder=0 allowfullscreen></iframe>
```

<iframe height=498 width=510 src="http://player.youku.com/embed/XNjcyMDU4Njg0" frameborder=0 allowfullscreen></iframe>

* 方法二：

```
    <embed src="http://player.youku.com/player.php/sid/XNzQxMjU2ODI0/v.swf" allowFullScreen="true" quality="high" width="480" height="400" align="middle" allowScriptAccess="always" type="application/x-shockwave-flash"></embed>
```

<embed src="http://player.youku.com/player.php/sid/XNzQxMjU2ODI0/v.swf" allowFullScreen="true" quality="high" width="480" height="400" align="middle" allowScriptAccess="always" type="application/x-shockwave-flash"></embed>

