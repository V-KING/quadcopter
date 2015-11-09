# gitbook插入视频


* 方法三

```
<iframe id="video" src="http://player.youku.com/embed/XODA2NDM4OTI0" width="510" height="498" frameborder="0" allowfullscreen="allowfullscreen"></iframe>

<script>
window.onload=window.onresize=Init;           
function Init(){            
	document.getElementById("video").width=""+document.body.clientWidth*0.8+"";             
	document.getElementById("video").height=""+document.body.clientWidth*0.45+"";
}
</script>
```

<iframe id="video" src="http://player.youku.com/embed/XODA2NDM4OTI0" width="510" height="498" frameborder="0" allowfullscreen="allowfullscreen"></iframe>

<script>
window.onload=window.onresize=Init;           
function Init(){            
	document.getElementById("video").width=""+document.body.clientWidth*0.8+"";             
	document.getElementById("video").height=""+document.body.clientWidth*0.45+"";
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


