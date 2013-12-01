<style type="text/css">
</style>
<div class="demo_area">
	<p><span class="demo_box">default box</span><span class="demo_box red">red box</span><span class="demo_box blue">blue box</span></p>
</div>

针对上面效果的解决方案，一般是对demo_box进行抽象，然后派生出red和blue等其它box，再结合代码效率什么的，得出的所谓最有效率的方案：

	.demo_box{... background-color:#F1F1F1; ...}
	.red{bcakground-color:#F7C6C7;}
	.blue{bcakground-color:#C7DEF8;}

但是，最高效的方案却不一定是最安全的，如果把`.demobox`从第一行移至第三行，结果将变成：

<style>
	.demo_box{background-color:#F1F1F1;}
</style>
<div class="demo_area">
	<p><span class="demo_box">default box</span><span class="demo_box red">red box</span><span class="demo_box blue">blue box</span></p>
</div>

没想到最高效的代码竟然如此脆弱。所以有时候不要太纠结，差不多了就行了。