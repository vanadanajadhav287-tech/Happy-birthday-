# Happy-birthday-🎂✨
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Happy Birthday ❤️</title>

<style>
body{
    margin:0;
    padding:0;
    font-family: 'Poppins', sans-serif;
    background: linear-gradient(135deg, #ff9a9e, #fad0c4);
    overflow-x:hidden;
    text-align:center;
    color:white;
}

/* Floating Balloons */
.balloon{
    position:absolute;
    bottom:-100px;
    width:50px;
    height:70px;
    background:red;
    border-radius:50%;
    animation: float 8s infinite ease-in;
}

@keyframes float{
    0%{transform:translateY(0);}
    100%{transform:translateY(-110vh);}
}

h1{
    margin-top:100px;
    font-size:40px;
    animation: glow 2s infinite alternate;
}

@keyframes glow{
    from{text-shadow:0 0 10px #fff;}
    to{text-shadow:0 0 25px #ff4da6;}
}

.message{
    margin:40px;
    font-size:20px;
    max-width:700px;
    margin-left:auto;
    margin-right:auto;
}

button{
    padding:15px 30px;
    font-size:18px;
    border:none;
    border-radius:30px;
    background:white;
    color:#ff4da6;
    cursor:pointer;
    transition:0.3s;
}

button:hover{
    background:#ff4da6;
    color:white;
    transform:scale(1.1);
}

#surprise{
    display:none;
    margin-top:30px;
    font-size:22px;
    animation: fadeIn 2s forwards;
}

@keyframes fadeIn{
    from{opacity:0;}
    to{opacity:1;}
}
</style>
</head>

<body>

<h1>🎂 Happy Birthday My Queen 🎂</h1>

<div class="message">
    Today is the most special day because the most special person was born.  
    Your presence in my life is like sunshine after rain.  
    You make my bad days better, my good days perfect, and my life meaningful.  
    Without you, everything feels incomplete.  
    Thank you for being my happiness, my peace, and my biggest blessing. ❤️
</div>

<button onclick="showSurprise()">Click For Surprise 🎁</button>

<div id="surprise">
    🌟 You are not just part of my life...  
    You ARE my life.  
    I am so lucky to have you.  
    Happy Birthday, ❤️✨
</div>

<script>
function showSurprise(){
    document.getElementById("surprise").style.display="block";
}

// Create multiple balloons
for(let i=0;i<20;i++){
    let balloon=document.createElement("div");
    balloon.className="balloon";
    balloon.style.left=Math.random()*100+"vw";
    balloon.style.backgroundColor=`hsl(${Math.random()*360},70%,60%)`;
    balloon.style.animationDuration=(5+Math.random()*5)+"s";
    document.body.appendChild(balloon);
}
</script>

</body>
</html>
