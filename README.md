- 👋 Hi, I’m @Kumutha0519
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
Kumutha0519/Kumutha0519 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
<p>Coding 

session.html

<html>

<head>

<script>

function clickCounter() {

 if (typeof(Storage) !== "undefined") {

 if (sessionStorage.clickcount) {

 sessionStorage.clickcount = Number(sessionStorage.clickcount)+1;

 } else {

 sessionStorage.clickcount = 1;

 }

 document.getElementById("result").innerHTML = "You have clicked the button " +

sessionStorage.clickcount + " time(s).";

 } else {

 document.getElementById("result").innerHTML = "Sorry, your browser does not support web

storage...";

 }

}

</script>

</head>

<body>

<p><button onclick="clickCounter()" type="button">Click me!</button></p>

<div id="result"></div>

<p>Click the button to see the counter increase.</p>

<p>Close the browser tab (or window), and try again, and the counter is reset.</p>

</body>

</html>

dragdrop.html

<html>

<head>

<style>

#div1, #div2 {

 float: left;

 width: 100px;

 height: 100px;

 margin: 10px;

 padding: 10px;

 border: 1px solid black;

}

</style>

<script>

function allowDrop(ev) {

 ev.preventDefault();

}

function drag(ev) {

 ev.dataTransfer.setData("text", ev.target.id);

}

function drop(ev) {

 ev.preventDefault();

 var data = ev.dataTransfer.getData("text");

 ev.target.appendChild(document.getElementById(data));

}

</script>

</head>

<body>

<h2>Drag and Drop</h2>

<p>Drag the image back and forth between the two div elements.</p>

<div id="div1" ondrop="drop(event)" ondragover="allowDrop(event)">

 <img src="smiley.gif" draggable="true" ondragstart="drag(event)" id="drag1" width="88"

height="88">

</div>

<div id="div2" ondrop="drop(event)" ondragover="allowDrop(event)"></div>

</body>

</html>

rosebud.html

<html>

<head>

<title>Untitled Document</title>

</head>

<body>

<canvas id="myCanvas" width="500" height="500" style="border-color:#63F;

 border-style:solid">

 </canvas>

 <script>

var c = document.getElementById("myCanvas");

var ctx = c.getContext('2d');

function draw_rose()

{

ctx.fillStyle = "green";

ctx.fillRect(218,240,5,150);

ctx.fillStyle = "red";

ctx.strokeStyle = "white";

ctx.arc(220,190,50,0,2*Math.PI);

ctx.fill();

ctx.scale(2,1);

ctx.fillRect(85,110,50,80);

ctx.beginPath();

ctx.arc(100,100,20,0,2*Math.PI);

ctx.fill();

ctx.stroke();

ctx.closePath();

ctx.beginPath();

ctx.arc(120,110,20,0,2*Math.PI);

ctx.fill();

ctx.stroke();

ctx.closePath();

ctx.fillStyle = "green";

ctx.beginPath();

ctx.arc(90,250,20,0,2*Math.PI);

ctx.fill();ctx.stroke();

ctx.closePath();

ctx.beginPath();

ctx.arc(130,250,20,0,2*Math.PI);

ctx.fill();

ctx.stroke();

ctx.closePath();

}

draw_rose();

</script>

</body>

</html>

ocation.html

<html>

<head>

<title>Untitled Document</title>

<script type="text/javascript">

function showPosition(position)

{

document.write("Latitude : "+position.coords.latitude);

document.write("Longitude : "+position.coords.longitude);

}

function getLocation()

{

if(navigator.geolocation)

{

navigator.geolocation.getCurrentPosition(showPosition);

}

else

{

document.write("Browser not supported");

}
Coding 

session.html

<html>

<head>

<script>

function clickCounter() {

 if (typeof(Storage) !== "undefined") {

 if (sessionStorage.clickcount) {

 sessionStorage.clickcount = Number(sessionStorage.clickcount)+1;

 } else {

 sessionStorage.clickcount = 1;

 }

 document.getElementById("result").innerHTML = "You have clicked the button " +

sessionStorage.clickcount + " time(s).";

 } else {

 document.getElementById("result").innerHTML = "Sorry, your browser does not support web

storage...";

 }

}

</script>

</head>

<body>

<p><button onclick="clickCounter()" type="button">Click me!</button></p>

<div id="result"></div>

<p>Click the button to see the counter increase.</p>

<p>Close the browser tab (or window), and try again, and the counter is reset.</p>

</body>

</html>

dragdrop.html

<html>

<head>

<style>

#div1, #div2 {

 float: left;

 width: 100px;

 height: 100px;

 margin: 10px;

 padding: 10px;

 border: 1px solid black;

}

</style>

<script>

function allowDrop(ev) {

 ev.preventDefault();

}

function drag(ev) {

 ev.dataTransfer.setData("text", ev.target.id);

}

function drop(ev) {

 ev.preventDefault();

 var data = ev.dataTransfer.getData("text");

 ev.target.appendChild(document.getElementById(data));

}

</script>

</head>

<body>

<h2>Drag and Drop</h2>

<p>Drag the image back and forth between the two div elements.</p>

<div id="div1" ondrop="drop(event)" ondragover="allowDrop(event)">

 <img src="smiley.gif" draggable="true" ondragstart="drag(event)" id="drag1" width="88"

height="88">

</div>

<div id="div2" ondrop="drop(event)" ondragover="allowDrop(event)"></div>

</body>

</html>

rosebud.html

<html>

<head>

<title>Untitled Document</title>

</head>

<body>

<canvas id="myCanvas" width="500" height="500" style="border-color:#63F;

 border-style:solid">

 </canvas>

 <script>

var c = document.getElementById("myCanvas");

var ctx = c.getContext('2d');

function draw_rose()

{

ctx.fillStyle = "green";

ctx.fillRect(218,240,5,150);

ctx.fillStyle = "red";

ctx.strokeStyle = "white";

ctx.arc(220,190,50,0,2*Math.PI);

ctx.fill();

ctx.scale(2,1);

ctx.fillRect(85,110,50,80);

ctx.beginPath();

ctx.arc(100,100,20,0,2*Math.PI);

ctx.fill();

ctx.stroke();

ctx.closePath();

ctx.beginPath();

ctx.arc(120,110,20,0,2*Math.PI);

ctx.fill();

ctx.stroke();

ctx.closePath();

ctx.fillStyle = "green";

ctx.beginPath();

ctx.arc(90,250,20,0,2*Math.PI);

ctx.fill();ctx.stroke();

ctx.closePath();

ctx.beginPath();

ctx.arc(130,250,20,0,2*Math.PI);

ctx.fill();

ctx.stroke();

ctx.closePath();

}

draw_rose();

</script>

</body>

</html>

ocation.html

<html>

<head>

<title>Untitled Document</title>

<script type="text/javascript">

function showPosition(position)

{

document.write("Latitude : "+position.coords.latitude);

document.write("Longitude : "+position.coords.longitude);

}

function getLocation()

{

if(navigator.geolocation)

{

navigator.geolocation.getCurrentPosition(showPosition);

}

else

{

document.write("Browser not supported");

}

}

</script>

</head>

<body>

 <button type="button" onClick="getLocation()">Get Location</button>

</body>

</html>
Coding 

session.html

<html>

<head>

<script>

function clickCounter() {

 if (typeof(Storage) !== "undefined") {

 if (sessionStorage.clickcount) {

 sessionStorage.clickcount = Number(sessionStorage.clickcount)+1;

 } else {

 sessionStorage.clickcount = 1;

 }

 document.getElementById("result").innerHTML = "You have clicked the button " +

sessionStorage.clickcount + " time(s).";

 } else {

 document.getElementById("result").innerHTML = "Sorry, your browser does not support web

storage...";

 }

}

</script>

</head>

<body>

<p><button onclick="clickCounter()" type="button">Click me!</button></p>

<div id="result"></div>

<p>Click the button to see the counter increase.</p>

<p>Close the browser tab (or window), and try again, and the counter is reset.</p>

</body>

</html>

dragdrop.html

<html>

<head>

<style>

#div1, #div2 {

 float: left;

 width: 100px;

 height: 100px;

 margin: 10px;

 padding: 10px;

 border: 1px solid black;

}

</style>

<script>

function allowDrop(ev) {

 ev.preventDefault();

}

function drag(ev) {

 ev.dataTransfer.setData("text", ev.target.id);

}

function drop(ev) {

 ev.preventDefault();

 var data = ev.dataTransfer.getData("text");

 ev.target.appendChild(document.getElementById(data));

}

</script>

</head>

<body>

<h2>Drag and Drop</h2>

<p>Drag the image back and forth between the two div elements.</p>

<div id="div1" ondrop="drop(event)" ondragover="allowDrop(event)">

 <img src="smiley.gif" draggable="true" ondragstart="drag(event)" id="drag1" width="88"

height="88">

</div>

<div id="div2" ondrop="drop(event)" ondragover="allowDrop(event)"></div>

</body>

</html>

rosebud.html

<html>

<head>

<title>Untitled Document</title>

</head>

<body>

<canvas id="myCanvas" width="500" height="500" style="border-color:#63F;

 border-style:solid">

 </canvas>

 <script>

var c = document.getElementById("myCanvas");

var ctx = c.getContext('2d');

function draw_rose()

{

ctx.fillStyle = "green";

ctx.fillRect(218,240,5,150);

ctx.fillStyle = "red";

ctx.strokeStyle = "white";

ctx.arc(220,190,50,0,2*Math.PI);

ctx.fill();

ctx.scale(2,1);

ctx.fillRect(85,110,50,80);

ctx.beginPath();

ctx.arc(100,100,20,0,2*Math.PI);

ctx.fill();

ctx.stroke();

ctx.closePath();

ctx.beginPath();

ctx.arc(120,110,20,0,2*Math.PI);

ctx.fill();

ctx.stroke();

ctx.closePath();

ctx.fillStyle = "green";

ctx.beginPath();

ctx.arc(90,250,20,0,2*Math.PI);

ctx.fill();ctx.stroke();

ctx.closePath();

ctx.beginPath();

ctx.arc(130,250,20,0,2*Math.PI);

ctx.fill();

ctx.stroke();

ctx.closePath();

}

draw_rose();

</script>

</body>

</html>

ocation.html

<html>

<head>

<title>Untitled Document</title>

<script type="text/javascript">

function showPosition(position)

{

document.write("Latitude : "+position.coords.latitude);

document.write("Longitude : "+position.coords.longitude);

}

function getLocation()

{

if(navigator.geolocation)

{

navigator.geolocation.getCurrentPosition(showPosition);

}

else

{

document.write("Browser not supported");

}

}

</script>

</head>

<body>

 <button type="button" onClick="getLocation()">Get Location</button>

</body>

</html>

}

</script>

</head>

<body>

 <button type="button" onClick="getLocation()">Get Location</button>

</body>

</html>
</p>
