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
font-family:'Poppins',sans-serif;
}

body{
height:100vh;
display:flex;
justify-content:center;
align-items:center;
background:linear-gradient(135deg,#ffd6e7,#ffc2da,#ffeaf4);
overflow:hidden;
}

.card{
width:90%;
max-width:420px;
background:rgba(255,255,255,.35);
backdrop-filter:blur(12px);
padding:35px;
border-radius:30px;
text-align:center;
box-shadow:0 15px 35px rgba(255,105,180,.3);
animation:fade 1.5s;
}

h1{
font-family:'Pacifico',cursive;
font-size:45px;
color:#ff4d88;
}

h2{
margin:10px 0;
color:#ff6b9a;
}

p{
margin-top:20px;
line-height:1.8;
color:#555;
}

button{
margin-top:25px;
padding:14px 30px;
background:#ff4d88;
color:white;
border:none;
border-radius:50px;
font-size:16px;
cursor:pointer;
transition:.3s;
}

button:hover{
transform:scale(1.08);
}

#popup{
position:fixed;
top:0;
left:0;
width:100%;
height:100%;
background:rgba(0,0,0,.45);
display:none;
justify-content:center;
align-items:center;
}

.box{
background:white;
padding:30px;
border-radius:25px;
width:85%;
max-width:350px;
text-align:center;
animation:fade .5s;
}

.box h2{
color:#ff4d88;
}

.box p{
margin-top:15px;
}

.heart{
position:absolute;
animation:fall linear forwards;
}

@keyframes fall{
0%{
transform:translateY(-100px);
opacity:0;
}
20%{
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
transform:translateY(30px);
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

<h1>🎂 Happy Birthday</h1>

<h2>Princess nyaa akuu 🩷</h2>

<p>

Selamat ulang tahun yaaa kesayangan nyaa akuuu! 😍🌸💕🥳💋💖

Semoga di usia yang baruu inii kamuu selalu sehat, bahagia, panjang umur, dan semua doa serta impian kamuu satu per satu menjadi kenyataan yaaa🫶.

Tiamaacii yaaa sayanggg udaaa hadir dan buatt hidup akuuu lebih berwarna🥰🫶. harapan akuu kedepannya semoga akuu bisaa terus dampingi kamuu disetiap ulang tahun kamuu🥺🫶

Tetap jadi perempuan yang baik, manis, lucu, dan selalu tersenyum yang akuu kenal yaaa sayanggg. 🥰🤍

Akuu bakalan selalu doa in yang terbaik buatt kamuu.😍🫶

Alapyuuuu kesayangan nyaa akuu.😍💖

</p>

<button onclick="bukaHadiah()">
🎁 Buka Hadiah
</button>

</div>

<div id="popup">

<div class="box">

<h2>💌 Pesan Spesial</h2>

<p>

Kalau suatu saatt nantii kamuu bertanya apaa hadiah terbaik yang pernaa akuu miliki...

Jawabannya tetap samaa.

<b>Kamuu sayanggg.</b> 🥺❤️

Terima kasih sudaa menjadi bagian terindah dalam hidup nyaa akuuu.🫶

Happy Birthday, Princess-ku.

I Love You Forever Sayangg💋🥰😍💖💕

</p>

<button onclick="tutup()">

💕 Peluk Virtual

</button>

</div>

</div>

<script>

function bukaHadiah(){

document.getElementById("popup").style.display="flex";

}

function tutup(){

document.getElementById("popup").style.display="none";

}

setInterval(()=>{

let heart=document.createElement("div");

heart.className="heart";

heart.innerHTML=["💖","💕","🌸","🩷","💗"][Math.floor(Math.random()*5)];

heart.style.left=Math.random()*100+"vw";

heart.style.fontSize=(18+Math.random()*20)+"px";

heart.style.animationDuration=(5+Math.random()*4)+"s";

document.body.appendChild(heart);

setTimeout(()=>{

heart.remove();

},9000);

},250);

</script>

</body>
</html>
