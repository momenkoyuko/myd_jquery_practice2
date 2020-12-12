<!doctype html>
<html>
<head>
<meta charset="UTF-8">
<title>無題ドキュメント</title>
</head>
<style>
	#ex{
		width: 300px;
		height: 300px;
		border: solid 1px red;
	}
</style>


<body>
<div id="ex">
</div>	
<button id="show">show</button>
<button id="hide">hide</button>
	
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
	
<script>
	let t = 0
	$("#hide").on("click",function(){
		$("#ex").hide(2000);
	});
	$("#show").on("click",function(){
		$("#ex").show(2000);
		t++;
		$("#ex").html(t);
		$("#ex").css("border",t+"px solid red");
		
	});
	
</script>
	
	
	
</body>
</html>
