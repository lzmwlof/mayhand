<?php
    header('Content-type: image/jpeg');
	$width = 400;
	$hieght = 600;
	$im = imagecreatetruecolor($width,$hieght);
	$bjcolor = imagecolorallocate($im,255,255,200);
    imagefilledrectangle($im,0,0,$width,$hieght,$bjcolor);		
	$text = '有人问我：分手了那么久还
	记得你的前任吗？
	怎么说呢？记得显得太花心，
	不记得显得太薄情，其实我觉得，
	那个人就好比我走路的时候
	撞上了一个电线杆，很痛，
	以后走路我都会记住绕着
	电线杆走，可能很久以后，
	我都不记得当时撞得
	有多痛了，可是，那个电线杆，
	永远都在。';
	$stercolor = imagecolorallocate($im,rand(0,255),rand(0,255),rand(0,255));
	$x = 40;
	$y = 160;
	$font = 'HaTian-JingZhi.ttf';
	imagettftext($im,16,0,$x,$y,$stercolor,$font,$text);
	imagejpeg($im);
	
	

?>
