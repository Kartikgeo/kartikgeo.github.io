<!DOCTYPE html>
<html>
<head>
	<title>7 Different Colors</title>
</head>
<body>
<script type="text/javascript">
var colors = new Array("blue", "yellow", "red", "green", "orange","cyan","indigo");
var i=0;
function changeColor()
{
	 document.body.style.backgroundColor = colors[i];
     i++;
     if(i>colors.length)
     {
     	i=0;
     }
 	 window.setTimeout("changeColor()",2000);	
}
function disp_mesg_status()
{
	window.status="All Seven Colors Displayed";
}
</script>
<form>
<input type="button" name=btn_color value="changecolors" onmouseover="changeColor()">
<input type="button" name="btn_mesg" value="Display Message" onclick="disp_mesg_status()">
</form>
</body>
</html>
