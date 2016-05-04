<!--# animation-delay--->
<!--css3  animation-delay负值应用-->
<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <title>animation-delay负值 弹性效果</title>
  <style type="text/css">
  *{padding:0;margin:0;}
  .box{width: 600px;margin:100px auto;}
  .box a{float:left;display:block;width:10px;height:100px;background:green;margin-left:10px;transform: scaleY(0.3);animation: zoomIn 1.2s ease infinite}
  /*.box a:nth-child(1){
    -webkit-animation-delay:-1s;
  }*/
  <!--跳跃时间段-->
  .box a:nth-child(2){
    -webkit-animation-delay:-1.1s;
  }
  .box a:nth-child(3){
    -webkit-animation-delay:-1.0s;
  }
  .box a:nth-child(4){
    -webkit-animation-delay:-0.9s;
  }
  .box a:nth-child(5){
    -webkit-animation-delay:-0.8s;
  }
  @-webkit-keyframes zoomIn{
  <!--实现跳跃式效果-->
   0%,40%,100%{
        -webkit-transform:scaleY(.4);
      }
      20%{
        -webkit-transform:scaleY(1);
  }
  </style>
</head>
<body>
<div class="box">
	<a href="#" class="one"></a>
	<a href="#" class="two"></a>
	<a href="#" class="three"></a>
	<a href="#" class="four"></a>
	<a href="#" class="five"></a>
</div>
</body>
</html>
