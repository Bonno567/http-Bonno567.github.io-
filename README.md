
<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Chúc mừng 8/3</title>

<style>
body{
background: linear-gradient(#ffd6e7,#ffeef5);
text-align:center;
font-family:sans-serif;
padding-top:50px;
}

h1{
color:#ff4d88;
font-size:40px;
}

p{
font-size:20px;
}

img{
width:220px;
border-radius:15px;
margin-top:20px;
}

button{
margin-top:30px;
padding:12px 25px;
font-size:18px;
background:#ff4d88;
color:white;
border:none;
border-radius:10px;
cursor:pointer;
}

.heart{
position:fixed;
bottom:-10px;
font-size:20px;
animation: float 5s linear infinite;
}

@keyframes float{
0%{transform:translateY(0)}
100%{transform:translateY(-100vh)}
}
</style>
</head>

<body>

<h1>Chúc mừng 8/3 🌸</h1>

<img src="https://i.imgur.com/9XnKQ9H.jpg">

<p>Chúc bạn có một ngày thật vui vẻ</p>
<p>và luôn cười nhiều như bây giờ ✨</p>

<button onclick="alert('Chúc bạn 8/3 vui vẻ nha! 🌸')">
Bấm vào đây 🎁
</button>

<script>
setInterval(()=>{
let heart=document.createElement("div");
heart.className="heart";
heart.innerHTML="❤️";
heart.style.left=Math.random()*100+"vw";
heart.style.fontSize=(15+Math.random()*20)+"px";
document.body.appendChild(heart);

setTimeout(()=>{heart.remove()},5000);
},500);
</script>

</body>
</html>
