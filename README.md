<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Gaming Web</title>

<style>

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:Arial, sans-serif;
}

body{
    background-image:url("https://img.goodfon.com/wallpaper/nbig/8/1d/digital-art-artwork-illustration-car-bmw.webp");
    background-size:cover;
    background-position:center;
    background-repeat:no-repeat;
    background-attachment:fixed;
    min-height:100vh;
    overflow-x:hidden;
    transition:0.5s;
}

/* DARK MODE */

.dark{
    background:#111;
    color:white;
}

/* NAVBAR */

nav{
    width:100%;
    padding:20px;
    display:flex;
    justify-content:space-between;
    align-items:center;
    background:rgba(0,0,0,0.5);
    backdrop-filter:blur(10px);
    position:sticky;
    top:0;
    z-index:1000;
}

.logo{
    color:#00eeff;
    font-size:30px;
    font-weight:bold;
    text-shadow:0 0 10px #00eeff;
}

nav ul{
    display:flex;
    list-style:none;
}

nav ul li{
    margin:0 15px;
}

nav ul li a{
    color:white;
    text-decoration:none;
    font-size:18px;
    transition:0.3s;
}

nav ul li a:hover{
    color:#00eeff;
    text-shadow:0 0 10px #00eeff;
}

/* BUTTON */

.mode-btn{
    padding:10px 20px;
    border:none;
    border-radius:10px;
    background:#00eeff;
    cursor:pointer;
    font-weight:bold;
}

/* GLASS EFFECT */

.container{
    width:90%;
    max-width:500px;
    margin:50px auto;
    padding:30px;
    border-radius:25px;
    background:rgba(255,255,255,0.1);
    backdrop-filter:blur(10px);
    box-shadow:0 0 20px rgba(0,0,0,0.5);
}

/* TITLE */

h1{
    color:white;
    margin-bottom:20px;
    text-shadow:0 0 10px cyan;
}

/* NEON BUTTONS */

.btn{
    display:block;
    margin:15px 0;
    padding:15px;
    text-align:center;
    border-radius:15px;
    text-decoration:none;
    color:white;
    background:rgba(0,0,0,0.5);
    border:2px solid #00eeff;
    transition:0.3s;
    box-shadow:0 0 10px #00eeff;
}

.btn:hover{
    background:#00eeff;
    color:black;
    transform:scale(1.05);
    box-shadow:0 0 30px #00eeff;
}

/* ANIMATION */

@keyframes move{
    0%{
        background-position:0 0;
    }
    100%{
        background-position:100% 100%;
    }
}

body{
    animation:move 20s linear infinite;
}

/* LOADING SCREEN */

#loader{
    position:fixed;
    width:100%;
    height:100vh;
    background:black;
    display:flex;
    justify-content:center;
    align-items:center;
    color:#00eeff;
    font-size:40px;
    z-index:9999;
}

/* RESPONSIVE */

@media(max-width:768px){

    nav{
        flex-direction:column;
    }

    nav ul{
        margin-top:10px;
    }

    nav ul li{
        margin:10px;
    }

    .container{
        width:95%;
    }

}

</style>
</head>

<body>

<div id="loader">
    LOADING...
</div>

<nav>

<div class="logo">GAMING</div>

<ul>
    <li><a href="#">Home</a></li>
    <li><a href="#">Games</a></li>
    <li><a href="#">Telegram</a></li>
</ul>

<button class="mode-btn" onclick="darkMode()">
🌙 Mode
</button>

</nav>

<div class="container">

<h1>🎮 O'yinlar</h1>

<a href="html.html" class="btn">Mini O'yin</a>

<a href="2 game.html" class="btn">Mini Horror</a>

<a href="2d game.html" class="btn">Mini Action</a>

<h1>🌐 Web Sahifa</h1>

<a href="mening web saxifam.html" class="btn">
Mening Sahifam
</a>

<h1>📩 Telegram</h1>

<a href="https://t.me/Azizradoy1" class="btn">
Azizga yozish
</a>

<a href="https://t.me/Nurikqwertyyy" class="btn">
Nursultonga yozish
</a>

<a href="https://t.me/ZBB2011" class="btn">
Bexruzga yozish
</a>

<h1>🧮 Kalkulyator</h1>

<a href="./calculator.html" class="btn">
Kalkulyator
</a>

</div>

<script>

/* DARK MODE */

function darkMode(){
    document.body.classList.toggle("dark");
}

/* LOADING */

window.addEventListener("load", function(){

    document.getElementById("loader").style.display="none";

});

</script>

</body>
</html>
