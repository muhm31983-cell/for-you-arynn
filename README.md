<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<title>Buat Arynn 🤍</title>
<style>
body{
    margin:0;
    height:100vh;
    background:linear-gradient(135deg,#ffd6e0,#ff9a9e);
    display:flex;
    justify-content:center;
    align-items:center;
    font-family:'Segoe UI',sans-serif;
}
.card{
    background:rgba(255,255,255,0.25);
    backdrop-filter:blur(10px);
    padding:30px;
    border-radius:25px;
    text-align:center;
    color:#fff;
    max-width:450px;
    box-shadow:0 10px 30px rgba(0,0,0,0.2);
}
.step{
    display:none;
    animation:fade 0.6s ease;
}
.step.active{
    display:block;
}
@keyframes fade{
    from{opacity:0; transform:translateY(10px);}
    to{opacity:1; transform:translateY(0);}
}
button{
    margin-top:20px;
    padding:12px 24px;
    border:none;
    border-radius:20px;
    background:#ff5c8a;
    color:white;
    font-size:14px;
    cursor:pointer;
}
button:hover{
    background:#ff3f75;
}
.emoji{
    font-size:34px;
}
</style>
</head>
<body>

<div class="card">

<!-- STEP 1 -->
<div class="step active">
    <div class="emoji">🐣💗</div>
    <h2>Haiy cantikk</h2>
    <p>
        Sebelum lanjut…  
        tarik napas dulu yaa 😌  
        <br><br>
        Kalau sudah siap,  
        klik tombolnya 🌸
    </p>
    <button onclick="nextStep()">aku siap 🐻</button>
</div>

<!-- STEP 2 -->
<div class="step">
    <div class="emoji">😆✨</div>
    <p>
        Iyaa kamuu…  
        <b>Julfa Arin Suryani Putri</b> 🤍  
        <br><br>
        Lagii sediii yaa sekaranggg? 😔  
        Abis baca ini  
        harusnya ketawaa sihhh 😆  
        <br><br>
        Sedihh gapapa koo,  
        itu wajarr 🌷
    </p>
    <button onclick="nextStep()">lanjut dikit 🐥</button>
</div>

<!-- STEP 3 -->
<div class="step">
    <div class="emoji">🕊🤍</div>
    <p>
        Semogaa orang yang  
        mungkin terdekat kamuu ituu,  
        <br>
        tenang di tempat terbaiknyaa 🤍  
        <br><br>
        Jangan lupaa buatt  
        terusss kirimm doa yaa  
        arynnnnn 🌸
    </p>
    <button onclick="nextStep()">aku baca 🤍</button>
</div>

<!-- STEP 4 -->
<div class="step">
    <div class="emoji">🐻🫶</div>
    <p>
        Kamuuu kaloo mau cerita  
        apapunn ituuu,  
        <br>
        bisaa ceritaainn  
        ke akuuu 😌  
        <br><br>
        Jangannn terlalu  
        mendam ituu  
        sendirii ya arynnnn 🐣
    </p>
    <button onclick="nextStep()">hampir selesai 🌈</button>
</div>

<!-- STEP 5 -->
<div class="step">
    <div class="emoji">💭🤍</div>
    <p>
        Mungkin aku juga bisaa  
        buat selalu bertanya…  
        <br><br>
        <i>“gimana hari kamu sekarangg?”</i> 😌  
        <br><br>
        Pelan-pelan yaa 🤍  
        Aku di sini kok 🌷
    </p>
    <button onclick="alert('Senyum dikit yaa 😄🤍')">
        selesai 🐰
    </button>
</div>

</div>

<!-- 🎵 LAGU INSTRUMENTAL ROMANTIS -->
<audio autoplay loop>
    <source src="https://www.soundhelix.com/examples/mp3/SoundHelix-Song-2.mp3" type="audio/mpeg">
</audio>

<script>
let current = 0;
const steps = document.querySelectorAll('.step');

function nextStep(){
    steps[current].classList.remove('active');
    current++;
    if(current < steps.length){
        steps[current].classList.add('active');
    }
}
</script>

</body>
</html>
