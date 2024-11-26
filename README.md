<html>
	<head>
		<meta charset="utf-8">
		<title></title>
		<script type="text/javascript">
			function question1(){
				alert("There is nothing in this option");
			}
			function tip(){
				alert("You already located at this page");
			}
			function warning(){
				alert("Click the picture, not the word!");
			}
			function last(){
				var obj1 = document.getElementById("num1");
				var obj2 = document.getElementById("num2");
				var obj3 = document.getElementById("num3");
				if(obj1.className=="img1"&&obj2.className=="img2"&&obj3.className=="img3"){
					obj1.className="img2";
					obj2.className="img3";
					obj3.className="img1";
					return;
				}
				if(obj1.className=="img2"&&obj2.className=="img3"&&obj3.className=="img1"){
					obj1.className="img3";
					obj2.className="img1";
					obj3.className="img2";
					return;
				}
				if(obj1.className=="img3"&&obj2.className=="img1"&&obj3.className=="img2"){
					obj1.className="img1";
					obj2.className="img2";
					obj3.className="img3";
					return;
				}
			}
			function next(e){
				var obj1 = document.getElementById("num1");
				var obj2 = document.getElementById("num2");
				var obj3 = document.getElementById("num3");
				if(obj1.className=="img1"&&obj2.className=="img2"&&obj3.className=="img3"){
					obj1.className="img3";
					obj2.className="img1";
					obj3.className="img2";
					return;
				}
				if(obj1.className=="img2"&&obj2.className=="img3"&&obj3.className=="img1"){
					obj1.className="img1";
					obj2.className="img2";
					obj3.className="img3";
					return;
				}
				if(obj1.className=="img3"&&obj2.className=="img1"&&obj3.className=="img2"){
					obj1.className="img2";
					obj2.className="img3";
					obj3.className="img1";
					return;
				}
			}
		</script>
		<style type="text/css">
			body{
				background-image:url("Backgroundimage.jpg");
				background-repeat:no-repeat;
				background-size:cover;
				background-color: dimgray;
				margin: 0px;
				padding: 0px;
			}
			ul{
					list-style-type:none;
			 		margin:0px auto;
			    	padding:0px;
			    	display:flex;
					justify-content:center;
					background-color:black;
			}
			li{
				 	width:15%;
			    	line-height:50px;
			    	text-align:center;
			    	background-size:100% 100%;
					color: aliceblue;
			}
			.txt1{
				color: gold;
				font-size: 30px;
				font-family: 华文行楷;
				border-right: 1px solid lightgoldenrodyellow;
			}
			.img1{
				width: 75%;
				height: 85%;
				display: flex;
				position: absolute;
				left: 12.5%;
				z-index: 3;
			}
			.page1{
				height: 150px;
				width: 40px;
				display: flex;
				position: absolute;
				left: 12.5%;
				top: 290px;
				align-items: center;
				justify-content: center;
				font-size: 20px;
				background-color: rgba(255,255,255,0.0);
				border-radius: 25px;
				color: grey;
				z-index: 5;
			}
			.page2{
				height: 150px;
				width: 40px;
				display: flex;
				position: absolute;
				right: 12.5%;
				top: 290px;
				align-items: center;
				justify-content: center;
				font-size: 20px;
				background-color: rgba(255,255,255,0.0);
				border-radius: 25px;
				color: grey;
				z-index: 5;
			}
			.img2{
				width: 75%;
				height: 85%;
				display: flex;
				position: absolute;
				left: 12.5%;
				z-index: 2;
			}
			.img3{
				width: 75%;
				height: 85%;
				display: flex;
				position: absolute;
				left: 12.5%;
				z-index: 1;
			}
			.imgl{
				width: 20%;
				height: 85%;
				display: flex;
				position: absolute;
				left: -2%;
			}
			.imgr{
				width: 20%;
				height: 85%;
				display: flex;
				position: absolute;
				right: -2%;
			}
			div{
				font-size: 25px;
				color: aliceblue;
				font-family: 华文行楷;
			}
			.div1{
				height: 10%;
				width: 20%;
				display: flex;
				position: absolute;
				right: 10%;
				z-index: 5;
			}
		</style>
	</head>
	<body>
		<ul>
			<li id="first" class="txt1" onclick="location.href='https://ys.mihoyo.com'">言er</li>
			<li onclick="location.href='https://beiming720.github.io/web2/'">首页</li>
		    <li onclick="location.href='https://beiming720.github.io/web2/web2-1/index1.html'">魂类游戏</li>
			<li onclick="tip()">类魂游戏</li>
			<li onclick="location.href='https://store.steampowered.com/'">其他</li>
		</ul>
		<img src="BlackMythWukong.jpg" class="img1" id="num1" onclick="location.href='https://heishenhua.com/'"/>
		<button type="button" class="page1" onclick="last(this)">◁</button>
		<button type="button" class="page2" onclick="next(this)">▷</button>
		<img src="HollowKnight.jpg" class="img2" id="num2" onclick="location.href='https://store.steampowered.com/app/367520/Hollow_Knight/'"/>
		<img src="Salt and Sanctuary.jpg" class="img3" id="num3" onclick="location.href='https://ska-studios.com/games/salt-and-sanctuary/'"/>
		<img src="BlackMythWukong-Yangjian.jpg" class="imgl"/>
		<img src="BlackMyth Wukong.jpg" class="imgr"/>
		<div class="div1" onclick="warning()">点击图片可查看详情</div>
	</body>
</html>
