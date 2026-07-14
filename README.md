<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Happy Birthday Princess 💖</title>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&family=Pacifico&display=swap" rel="stylesheet">

<style>
*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:Poppins,sans-serif;
}

body{
background:linear-gradient(135deg,#ffd6e7,#ffc0cb,#ffe4ef);
overflow:hidden;
display:flex;
justify-content:center;
align-items:center;
height:100vh;
}

.card{
background:rgba(255,255,255,.4);
backdrop-filter:blur(10px);
padding:30px;
border-radius:30px;
text-align:center;
width:90%;
max-width:400px;
box-shadow:0 10px 30px rgba(255,105,180,.3);
animation:fade 1.5s;
}

img{
width:180px;
height:180px;
border-radius:50%;
object-fit:cover;
border:6px solid white;
box-shadow:0 5px 20px rgba(255,105,180,.4);
margin-bottom:20px;
}

h1{
font-family:Pacifico;
color:#ff4f93;
font-size:42px;
}

p{
margin-top:15px;
line-height:1.8;
color:#555;
}

button{
margin-top:20px;
padding:12px 30px;
border:none;
background:#ff4f93;
color:white;
border-radius:50px;
font-size:16px;
cursor:pointer;
transition:.3s;
}

button:hover{
transform:scale(1.08);
}

.heart{
position:absolute;
font-size:25px;
animation:fall linear forwards;
}

@keyframes fall{
0%{
transform:translateY(-100px);
opacity:0;
}
10%{
opacity:1;
}
100%{
transform:translateY(110vh);
opacity:0;
}
}

@keyframes fade{
from{
opacity:0;
transform:translateY(40px);
}
to{
opacity:1;
transform:translateY(0);
}
}
</style>
</head>

<body>

<div class="card">

<img src="foto.jpg" alt="Princess">

<h1>Happy Birthday 💖</h1>

<h2>Princess nya akuu 🥰</h2>

<p>
Selamat ulang tahun yaa sayangku 🤍🌸<br><br>

Semoga selalu sehat, bahagia, panjang umur,
dan semua impianmu tercapai.

Terima kasih sudah hadir di hidupku dan
menjadi alasan aku tersenyum setiap hari.

Aku sayang kamu lebih dari yang bisa
aku ungkapkan dengan kata-kata. 💕

Love You Forever ❤️
</p>

<button onclick="surprise()">
Klik Hadiahnya 🎁
</button>

</div>

<script>

function surprise(){

alert("💖 Selamat Ulang Tahun Princess-ku! 💖\n\nSemoga kita selalu bersama yaa. Aku sayang kamu selamanya ❤️");

}

setInterval(()=>{

let h=document.createElement("div");

h.className="heart";

h.innerHTML=["💖","💕","🌸","💗"][Math.floor(Math.random()*4)];

h.style.left=Math.random()*100+"vw";

h.style.fontSize=(20+Math.random()*20)+"px";

h.style.animationDuration=(5+Math.random()*4)+"s";

document.body.appendChild(h);

setTimeout(()=>{
h.remove();
},9000);

},250);

</script>

</body>
</html>
