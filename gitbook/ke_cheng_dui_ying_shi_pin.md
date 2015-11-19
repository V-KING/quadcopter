# gitbook插入视频
使用embed手机不兼容，所以使用iframe


* 方法1

```
<iframe id="video" onload="Init()" src="http://player.youku.com/embed/XODg5NjE3ODcy"  frameborder="0" allowfullscreen="allowfullscreen"></iframe>

<script>
window.onload=window.onresize=window.load=Init;var iframePaddingleft = 15;           
function Init(){            
    document.getElementsByTagName("iframe").video.width=""+document.getElementById("section-").clientWidth-iframePaddingleft*2+"";
    document.getElementsByTagName("iframe").video.height=""+document.getElementById("section-").clientWidth*9/16+"";
}
</script>
```

<iframe id="video" onload="Init()" src="http://player.youku.com/embed/XODg5NjE3ODcy"  frameborder="0" allowfullscreen="allowfullscreen"></iframe>

<script>
window.onload=window.onresize=window.load=Init;var iframePaddingleft = 15;           
function Init(){            
    document.getElementsByTagName("iframe").video.width=""+document.getElementById("section-").clientWidth-iframePaddingleft*2+"";
    document.getElementsByTagName("iframe").video.height=""+document.getElementById("section-").clientWidth*9/16+"";
}
</script>

