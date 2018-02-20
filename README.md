<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>

.hero {
    background-color: salmon;
    background-image: url("https://raw.githubusercontent.com/xela3287/My-Resume/master/12931264_1140210139322976_6155531305991804464_n.jpg");
    background-position: center;
    background-size: cover;
    color: #fff;
    height: 200vh;
    overflow: hidden;
}

.textimage {
	position: relative;
	widht: 300px;
	height: 350px;
	top: -50px;
	left: -50px;
	
}
ul {
    list-style-type: none;
    font-family: "Arial";
    margin: 0;
    padding: 0;
    overflow: hidden;
    background-color: #333;
}

li {
    float: left;
}

li a {
    font-family: "Arial";
    display: block;
    color: white;
    text-align: center;
    padding: 14px 16px;
    text-decoration: none;
}

li a:hover {
    background-color: #111;
}
.mySlides {display:none;
	bonder:solid;
	position: relative;
	widht: 500px;
	height: 300px;
	top: -250px;
	right: -740px;}

.text-block {
    position: absolute;
    bottom: 20px;
    right: 20px;
    background-color: black;
    color: white;
    padding-left: 20px;
    padding-right: 20px;
}
.asidestyle{
background-color: #000000;
position: relative;
height:500px;
width: 500px;
right: -500px;
top:-500px;

 opacity: 0.5;
 filter: alpha(opacity=50);
}

</style>
</head>


<body onload="startTime()">
<ul>
  <li><a class="active" href="#home">Home</a></li>
  <li><a href="#News">MySelf</a></li>
  <li><a href="#contact">Contact</a></li>
  <li><a href="#About"></a></li>
  
</ul>
<div class="hero">
<img class="textimage" src="https://raw.githubusercontent.com/xela3287/My-Resume/master/LIFE%20c%26g.png"/>
 <div >


<img class="textimage" src="My-Resume/LIFE c&g.png">



</div> 
 


<aside class="asidestyle">


<div class="text-block">
    <h4>Nature</h4>
    
</div>

</aside>
<div class="slidePos" style="max-width:500px">

</ul>
  <img class="mySlides" src="https://juegosrev.com/wp-content/uploads/2017/06/Wallpapers-One-Piece-Luffy-Gallery-85-Plus-PIC-WPW3010576.jpg" style="width:100%">
  <img class="mySlides" src="http://otakukart.com/animeblog/wp-content/uploads/2017/08/Monkey-d-luffy-gear-4-Full-HD.jpg" style="width:100%">
  <img class="mySlides" src="http://www.onepiecepodcast.com/wp-content/uploads/2014/01/one-piece-film-z.jpg" style="width:100%">
</div>	

</div>


<script>
var myIndex = 0;
carousel();

function carousel() {
    var i;
    var x = document.getElementsByClassName("mySlides");
    for (i = 0; i < x.length; i++) {
       x[i].style.display = "none";  
    }
    myIndex++;
    if (myIndex > x.length) {myIndex = 1}    
    x[myIndex-1].style.display = "block";  
    setTimeout(carousel, 2000); // Change image every 2 seconds
}
function startTime() {
    var today = new Date();
    var h = today.getHours();
    var m = today.getMinutes();
    var s = today.getSeconds();
    m = checkTime(m);
    s = checkTime(s);
    document.getElementById('txt').innerHTML =
    h + ":" + m + ":" + s;
    var t = setTimeout(startTime, 500);
}
function checkTime(i) {
    if (i < 10) {i = "0" + i};  // add zero in front of numbers < 10
    return i;
}
</script>
</body>
</html> 
