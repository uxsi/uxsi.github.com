---
layout: default
---

<style>
	.demo_area{}
	.demo_area p{letter-spacing:12px;}
	.demo_box{display:inline-block;width:100px;height:100px;background-color:#F1F1F1;text-align:center;letter-spacing:normal;}
	.demo_box.red{background-color:#F7C6C7;}
	.demo_box.blue{background-color:#C7DEF8;}
</style>
<div class="demo_area">
	<p><span class="demo_box">default box</span><span class="demo_box red">red box</span><span class="demo_box blue">blue box</span></p>
</div>

```css
.demo_box{... background-color:#F1F1F1; ...}
.red{bcakground-color:#F7C6C7;}
.blue{bcakground-color:#C7DEF8;}
```
<style>
	.demo_box{background-color:#F1F1F1;}
</style>
<div class="demo_area">
	<p><span class="demo_box">default box</span><span class="demo_box red">red box</span><span class="demo_box blue">blue box</span></p>
</div>

所以