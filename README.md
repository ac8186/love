<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
<meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
<title>专属</title>

<style type="text/css">
@font-face {
	font-family: digit;
	src: url('digital-7_mono.ttf') format("truetype");
}
</style>

<link rel="shortcut icon" type="image/x-icon" href="pig.ico" />
<link href="css/default.css" type="text/css" rel="stylesheet">
<script type="text/javascript" src="js/jquery.js"></script>
<script type="text/javascript" src="js/garden.js"></script>
<script type="text/javascript" src="js/functions.js"></script>

</head>

<body>

<div id="mainDiv">
	<div id="content">
		<div id="code">

			<span class="space"/><span class="comments">Youth fades day by day,</span><br />
			  一个白日带走了一点青春，<br />
			<span class="space"/><span class="comments">Though what we had in my memory can not be erased,</span><br />	
			  日子虽不能毁坏我印象里你所给我的光阴，<br />			
			<span class="space"/><span class="comments">Still it makes me different gradually.</span><br />	
			却慢慢的使我不同了。<br />			
			<span class="space"/><span class="comments">Life is too thin,</span><br />	
			生命是太脆薄的一种东西，<br />			
			<span class="space"/><span class="comments">which withers more than a flower against the days,</span><br />	
			并不比一株花更经得住年月风雨，<br />			
            <span class="space"/><span class="comments">With an eye for nature,</span><br />
			用对自然倾心的眼，<br />
			<span class="space"/><span class="comments">Look at our lives.</span><br />
			反观人生，<br />
			<span class="space"/><span class="comments">I can’t help but feel cherished of passion,</span><br />
			使我不能不觉得热情的可珍，<br />
			<span class="space"/><span class="comments">On the same person and same thing,</span><br />
			在同一人事上，<br />
			<span class="space"/><span class="comments">Coincidence just happens once.</span><br />
			第二次的凑巧是不会有的。<br />
			<span class="space"/><span class="comments">I have only seen the full moon once in my life.</span><br />
			我生平只看过一回满月。<br />			
			<span class="space"/><span class="comments">And I comforted myself,</span><br />	
			我也安慰自己过，<br />	
			<span class="space"/><span class="comments">I told myself,</span><br />	
			我说：<br />				
			<span class="space"/><span class="comments">I have crossed bridges in many places,</span><br />	
			我行过许多地方的桥，<br />				
			<span class="space"/><span class="comments">I have seen clouds for many times,</span><br />	
			看过许多次数的云，<br />				
			<span class="space"/><span class="comments">I have drunk wine of many kinds,</span><br />	
			喝过许多种类的酒，<br />				
			<span class="space"/><span class="comments">But only loved one girl who was in her best age.</span><br />	
			却只爱过一个正当最好年龄的人。<br />				
			
			<span class="space"/><span class="comments">---------------------------------------------</span><br />
			<span class="keyword">Mr</span> ZHANG ＆ <span class="keyword">Mrs</span> MA From 2016-3-31<br />
		</div>
		<div id="loveHeart">
			<canvas id="garden"></canvas>
			<div id="words">
				<div id="messages">
					亲爱的，这是我们相爱在一起的时光。
					<div id="elapseClock"></div>
				</div>
				<div id="loveu">
					爱你直到永永远远。<br/>
					<div class="signature">- 张先生</div>
				</div>
			</div>
		</div>
	</div>
</div>

<script type="text/javascript">
var offsetX = $("#loveHeart").width() / 2;
var offsetY = $("#loveHeart").height() / 2 - 55;
var together = new Date("2016-03-31 19:00:00");
// together.setFullYear(2017,11,25);
// together.setHours(10);
// together.setMinutes(0);
// together.setSeconds(0);
// together.setMilliseconds(0);

if (!document.createElement('canvas').getContext) {
	var msg = document.createElement("div");
	msg.id = "errorMsg";
	msg.innerHTML = "Your browser doesn't support HTML5!<br/>Recommend use Chrome 14+/IE 9+/Firefox 7+/Safari 4+"; 
	document.body.appendChild(msg);
	$("#code").css("display", "none")
	$("#copyright").css("position", "absolute");
	$("#copyright").css("bottom", "10px");
	document.execCommand("stop");
} else {
	setTimeout(function () {
		startHeartAnimation();
	}, 5000);

	//传递给后端初始时间
	timeElapse(together);
	
	setInterval(function () {
		timeElapse(together);
	}, 500);

	adjustCodePosition();
	$("#code").typewriter();
}
</script>
</div>
</body>
</html>
