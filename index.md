## 欢迎来到我的网页，我是沭辙。
<html>
	<head>
		<meta charset="utf-8">
		<title></title>
		<style type="text/css">
		#box{width: 100px; margin: 25px; background-color: #6495ed; position: absolute; border: 3px dashed blue;}
		</style>
		<script src="jquery-3.6.0.js"></script>
	</head>
	<body>
		<input type="button" class="button" value="执行动画"/>
		<input type="button" id="stop" value="停"/>
		<div id="box">RIA应用开发</div>
	</body>
	<script type="text/jscript">
	$('.button').click(function(){
		/*$('#box').animate({
			width:'300px',
			height:'200px',
			opacity:0.5,
			fontSize:'50px'
			});*/
			
		/*$('#box').animate({
			left:'300px',
			top:'200px'},'slow');*/
			
		/*$('#box').animate({
			left:'+=100px'},'slow');*/
			
		$('#box').animate({width:'300px'})
			     .animate({height:'200px'})
				 .animate({opacity:0.5})
				 .animate({fontSize:'50px'});
				 
		$("#stop").click(function(){
			//$("#box").stop();
			$("#box").stop(true,false/*true*/);
		});	 
	});
	</script>
</html>

