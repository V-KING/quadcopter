# gitbook插入视频
使用embed手机不兼容，所以使用iframe


* 方法1

```
<iframe id="video" width="510" height="498" src="http://player.youku.com/embed/XODA2NDM4OTI0"  frameborder="0" allowfullscreen="allowfullscreen"></iframe>

<script>
window.onload=window.onresize=Init;           
function Init(){            
	document.getElementsByTagName("iframe").video.width=""+document.getElementById("section-").clientWidth*0.9+"";
	document.getElementsByTagName("iframe").video.height=""+document.getElementById("section-").clientWidth*9/16+"";
}
</script>
```

<iframe id="video" width="510" height="498" src="http://player.youku.com/embed/XODA2NDM4OTI0"  frameborder="0" allowfullscreen="allowfullscreen"></iframe>

<script>
window.onload=window.onresize=Init;           
var iframePaddingleft = 15;
function Init(){            
	document.getElementsByTagName("iframe").video.width=""+document.getElementById("section-").clientWidth-iframePaddingleft*2+"";
	document.getElementsByTagName("iframe").video.height=""+document.getElementById("section-").clientWidth*9/16+"";
}
</script>

