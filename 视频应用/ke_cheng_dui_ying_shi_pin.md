# gitbook插入视频


* 方法三

```
<iframe id="video" src="http://player.youku.com/embed/XODA2NDM4OTI0" width="510" height="498" frameborder="0" allowfullscreen="allowfullscreen"></iframe>

<script>
window.onload=window.onresize=Init;           
function Init(){            
	document.getElementById("section-").width=""+document.body.clientWidth*0.8+"";             
	document.getElementById("section-").height=""+document.body.clientWidth*0.45+"";
}
</script>

document.getElementsByTagName("iframe").video.width
```

<iframe id="video" width="510" height="498" src="http://player.youku.com/embed/XODA2NDM4OTI0"  frameborder="0" allowfullscreen="allowfullscreen"></iframe>

<script>
window.onresize=Init;           
function Init(){            
	document.getElementsByTagName("iframe").video.width=""+document.getElementById("section-").clientWidth+"";
	document.getElementsByTagName("iframe").video.width=""+document.getElementById("section-").clientWidth*9/16+"";
}
</script>




* 方法一：

```
<iframe height=498 width=510 src="http://player.youku.com/embed/XNjcyMDU4Njg0" frameborder=0 allowfullscreen></iframe>
```


* 方法二：

```
    <embed src="http://player.youku.com/player.php/sid/XNzQxMjU2ODI0/v.swf" allowFullScreen="true" quality="high" width="480" height="400" align="middle" allowScriptAccess="always" type="application/x-shockwave-flash"></embed>
```


