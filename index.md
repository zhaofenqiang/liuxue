---
title: Welcome!
layout: template
filename: index
--- 
<br>
<h1 align="center"> <strike> Netflix and Chill </strike> <br> Netflix, HBO, Hulu, Youtube, Disney+, Apple TV, Amazon Prime Video... and Chill </h1>

<p align="center">
  <img src="https://raw.githubusercontent.com/imcrisanto/mms-142/main/streaming-scrolling.gif" />
   <br>
  <em> Source: The Wall Street Journal </em>
</p>

Presented on this site is a report on Video Streaming Services by Group D. Be informed of the roots of this technology; how and why it rose to popularity among the audience; how it runs as a business; its impact to the television, DVD, and traditional film industries; and ultimately, the future awaiting this technology based on the current trends and data.

*** 

<h3 align="center"> <i> "Most entrepreneurial ideas will sound crazy, stupid, and uneconomic, <br> and then they'll turn out to be right." </i> <br> <h4 align="center"> - Reed Hastings, CEO of Netflix </h4>  </h3> 

*** 

<div align="center">
<script type="text/javascript" align="center">
//Specify the slider's width (in pixels)
var sliderwidth="730px"
//Specify the slider's height
var sliderheight="180px"
//Specify the slider's slide speed (larger is faster 1-10)
var slidespeed=2
//configure background color:
slidebgcolor="#FFFFFF"

//Specify the slider's images
var leftrightslide=new Array()
var finalslide=''
leftrightslide[0]='<a href="https://imcrisanto.github.io/mms142-groupd-2020/history"><img src="https://i.imgur.com/aQK5fWh.png" border=1 alt="History"></a>'
leftrightslide[1]='<a href="https://imcrisanto.github.io/mms142-groupd-2020/business"><img src="https://i.imgur.com/OnNCTXr.png.png" border=1 alt="Business"></a>'
leftrightslide[2]='<a href="https://imcrisanto.github.io/mms142-groupd-2020/popularity"><img src="https://i.imgur.com/1499QRZ.png" border=1 alt="Popularity"></a>'
leftrightslide[3]='<a href="https://imcrisanto.github.io/mms142-groupd-2020/impact"><img src="https://i.imgur.com/Htp5jhs.png" border=1 alt="Impact"></a>'
leftrightslide[4]='<a href="https://imcrisanto.github.io/mms142-groupd-2020/future"><img src="https://i.imgur.com/7ZcoFz9.png" border=1 alt="Future"></a>'
//Specify gap between each image (use HTML):
var imagegap=" "

//Specify pixels gap between each slideshow rotation (use integer):
var slideshowgap=5

////NO NEED TO EDIT BELOW THIS LINE////////////

var copyspeed=slidespeed
leftrightslide='<nobr>'+leftrightslide.join(imagegap)+'</nobr>'
var iedom=document.all||document.getElementById
if (iedom)
document.write('<span id="temp" style="visibility:hidden;position:absolute;top:-100px;left:-9000px">'+leftrightslide+'</span>')
var actualwidth=''
var cross_slide, ns_slide

function fillup(){
if (iedom){
cross_slide=document.getElementById? document.getElementById("test2") : document.all.test2
cross_slide2=document.getElementById? document.getElementById("test3") : document.all.test3
cross_slide.innerHTML=cross_slide2.innerHTML=leftrightslide
actualwidth=document.all? cross_slide.offsetWidth : document.getElementById("temp").offsetWidth
cross_slide2.style.left=actualwidth+slideshowgap+"px"
}
else if (document.layers){
ns_slide=document.ns_slidemenu.document.ns_slidemenu2
ns_slide2=document.ns_slidemenu.document.ns_slidemenu3
ns_slide.document.write(leftrightslide)
ns_slide.document.close()
actualwidth=ns_slide.document.width
ns_slide2.left=actualwidth+slideshowgap
ns_slide2.document.write(leftrightslide)
ns_slide2.document.close()
}
lefttime=setInterval("slideleft()",30)
}
window.onload=fillup

function slideleft(){
if (iedom){
if (parseInt(cross_slide.style.left)>(actualwidth*(-1)+8))
cross_slide.style.left=parseInt(cross_slide.style.left)-copyspeed+"px"
else
cross_slide.style.left=parseInt(cross_slide2.style.left)+actualwidth+slideshowgap+"px"

if (parseInt(cross_slide2.style.left)>(actualwidth*(-1)+8))
cross_slide2.style.left=parseInt(cross_slide2.style.left)-copyspeed+"px"
else
cross_slide2.style.left=parseInt(cross_slide.style.left)+actualwidth+slideshowgap+"px"

}
else if (document.layers){
if (ns_slide.left>(actualwidth*(-1)+8))
ns_slide.left-=copyspeed
else
ns_slide.left=ns_slide2.left+actualwidth+slideshowgap

if (ns_slide2.left>(actualwidth*(-1)+8))
ns_slide2.left-=copyspeed
else
ns_slide2.left=ns_slide.left+actualwidth+slideshowgap
}
}


if (iedom||document.layers){
with (document){
document.write('<table border="0" cellspacing="0" cellpadding="0"><td>')
if (iedom){
write('<div style="position:relative;width:'+sliderwidth+';height:'+sliderheight+';overflow:hidden">')
write('<div style="position:absolute;width:'+sliderwidth+';height:'+sliderheight+';background-color:'+slidebgcolor+'" onMouseover="copyspeed=0" onMouseout="copyspeed=slidespeed">')
write('<div id="test2" style="position:absolute;left:0px;top:0px"></div>')
write('<div id="test3" style="position:absolute;left:-1000px;top:0px"></div>')
write('</div></div>')
}
else if (document.layers){
write('<ilayer width='+sliderwidth+' height='+sliderheight+' name="ns_slidemenu" bgColor='+slidebgcolor+'>')
write('<layer name="ns_slidemenu2" left=0 top=0 onMouseover="copyspeed=0" onMouseout="copyspeed=slidespeed"></layer>')
write('<layer name="ns_slidemenu3" left=0 top=0 onMouseover="copyspeed=0" onMouseout="copyspeed=slidespeed"></layer>')
write('</ilayer>')
}
document.write('</td></table>')
}
}
</script> 
</div>
