<!DOCTYPE html>
<html lang="sq">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Surprizë ❤️</title>

<style>
body{
    margin:0;
    height:100vh;
    display:flex;
    justify-content:center;
    align-items:center;
    background:linear-gradient(135deg,#ff8fb1,#ffd6e7);
    font-family:Arial,sans-serif;
    text-align:center;
}

.box{
    background:white;
    padding:30px;
    border-radius:20px;
    box-shadow:0 0 20px #ff8fb1;
}

h1{
    color:#ff4f81;
}

button{
    padding:15px 30px;
    margin:10px;
    border:none;
    border-radius:30px;
    font-size:20px;
    cursor:pointer;
}

.yes{
    background:#ff4f81;
    color:white;
}

.no{
    background:#ddd;
}

img{
    width:250px;
    border-radius:20px;
    display:none;
}
</style>

</head>

<body>

<div class="box">
<h1>A e do Elushi Alessin? ❤️</h1>

<button class="yes" onclick="yes()">PO ❤️</button>
<button class="no" onclick="no()">JO 😢</button>

<br>
<img id="photo" src="foto.jpg">

<p id="msg"></p>
</div>


<script>
let size=20;

function no(){
    size-=3;
    document.querySelector(".no").style.fontSize=size+"px";
    if(size<=5){
        document.querySelector(".no").style.display="none";
    }
}

function yes(){
    document.getElementById("photo").style.display="block";
    document.getElementById("msg").innerHTML="E dija që do thoshe PO ❤️🥰";
}
</script>

</body>
</html>
