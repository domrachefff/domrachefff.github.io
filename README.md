<!DOCTYPE html>
<html lang="ru">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Дмитрий & Анастасия — Свадьба</title>

<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@300;400;500;600&family=Montserrat:wght@300;400;500&display=swap" rel="stylesheet">

<style>

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
}

html{
    scroll-behavior:smooth;
}

body{
    background:#0d0d0d;
    color:white;
    font-family:'Montserrat',sans-serif;
    overflow-x:hidden;
}

/* ===== HERO ===== */

.hero{
    position:relative;
    width:100%;
    height:100vh;
    background:
    linear-gradient(rgba(0,0,0,.28), rgba(0,0,0,.42)),
    url('photo.jpg') center center/cover no-repeat;
    display:flex;
    align-items:center;
    padding:70px;
}

.hero::before{
    content:'';
    position:absolute;
    inset:0;
    background:linear-gradient(to right,
    rgba(0,0,0,.58) 0%,
    rgba(0,0,0,.35) 40%,
    rgba(0,0,0,.15) 100%);
}

.content{
    position:relative;
    z-index:2;
    max-width:520px;
}

.top-text{
    letter-spacing:6px;
    font-size:12px;
    margin-bottom:30px;
    opacity:.9;
}

.names{
    font-family:'Cormorant Garamond',serif;
    font-size:78px;
    line-height:0.95;
    font-weight:300;
}

.and{
    font-size:55px;
    margin:15px 0;
    opacity:.9;
}

.date{
    margin-top:35px;
    font-size:42px;
    font-family:'Cormorant Garamond',serif;
}

.desc{
    margin-top:30px;
    font-size:18px;
    line-height:1.9;
    max-width:420px;
    color:rgba(255,255,255,.92);
}

.info{
    margin-top:35px;
    display:flex;
    flex-direction:column;
    gap:18px;
}

.info div{
    display:flex;
    align-items:center;
    gap:14px;
    font-size:17px;
}

.arrow{
    margin-top:50px;
    font-size:42px;
    animation:move 1.7s infinite;
}

@keyframes move{
    0%{transform:translateY(0)}
    50%{transform:translateY(10px)}
    100%{transform:translateY(0)}
}

/* ===== STORY ===== */

.story{
    position:relative;
    padding:110px 10%;
    background:
    linear-gradient(rgba(0,0,0,.6), rgba(0,0,0,.72)),
    url('https://images.unsplash.com/photo-1519167758481-83f550bb49b3?q=80&w=2000&auto=format&fit=crop') center/cover;
}

.story h2{
    font-family:'Cormorant Garamond',serif;
    font-size:52px;
    font-weight:300;
    margin-bottom:30px;
}

.story p{
    max-width:720px;
    line-height:2;
    font-size:18px;
    color:rgba(255,255,255,.88);
}

/* ===== DETAILS ===== */

.details{
    display:grid;
    grid-template-columns:repeat(3,1fr);
    gap:25px;
    padding:90px 10%;
    background:#111;
}

.card{
    border:1px solid rgba(255,255,255,.12);
    background:rgba(255,255,255,.03);
    padding:45px 25px;
    text-align:center;
    backdrop-filter:blur(4px);
}

.card h3{
    font-family:'Cormorant Garamond',serif;
    font-size:36px;
    margin-bottom:15px;
    font-weight:300;
}

.card p{
    line-height:1.8;
    color:rgba(255,255,255,.8);
}

/* ===== TIMER ===== */

.timer{
    padding:110px 10%;
    text-align:center;
    background:#0c0c0c;
}

.timer h2{
    font-family:'Cormorant Garamond',serif;
    font-size:54px;
    font-weight:300;
}

.countdown{
    margin-top:50px;
    display:flex;
    justify-content:center;
    flex-wrap:wrap;
    gap:25px;
}

.time{
    min-width:160px;
    padding:35px 20px;
    border:1px solid rgba(255,255,255,.12);
    background:rgba(255,255,255,.03);
}

.number{
    font-size:64px;
    font-family:'Cormorant Garamond',serif;
}

.label{
    margin-top:12px;
    letter-spacing:2px;
    opacity:.75;
}

/* ===== DRESS CODE ===== */

.dress{
    display:grid;
    grid-template-columns:1fr 1fr;
    min-height:550px;
}

.dress-image{
    background:
    linear-gradient(rgba(0,0,0,.1), rgba(0,0,0,.1)),
    url('https://images.unsplash.com/photo-1496747611176-843222e1e57c?q=80&w=1974&auto=format&fit=crop') center/cover;
}

.dress-content{
    padding:90px 70px;
    background:#121212;
    display:flex;
    flex-direction:column;
    justify-content:center;
}

.dress-content h2{
    font-family:'Cormorant Garamond',serif;
    font-size:54px;
    font-weight:300;
    margin-bottom:25px;
}

.dress-content p{
    line-height:2;
    color:rgba(255,255,255,.88);
    font-size:17px;
}

.colors{
    display:flex;
    gap:18px;
    margin-top:35px;
}

.circle{
    width:45px;
    height:45px;
    border-radius:50%;
    border:1px solid rgba(255,255,255,.25);
}

.c1{background:#ffffff;}
.c2{background:#d8d1c9;}
.c3{background:#b4aba1;}
.c4{background:#7d7d7d;}
.c5{background:#000000;}

/* ===== GALLERY ===== */

.gallery{
    display:grid;
    grid-template-columns:repeat(4,1fr);
}

.gallery img{
    width:100%;
    height:260px;
    object-fit:cover;
}

/* ===== CONFIRM ===== */

.confirm{
    position:relative;
    padding:120px 10%;
    text-align:center;
    background:
    linear-gradient(rgba(0,0,0,.55), rgba(0,0,0,.7)),
    url('photo.jpg') center/cover;
}

.confirm h2{
    position:relative;
    z-index:2;
    font-family:'Cormorant Garamond',serif;
    font-size:56px;
    font-weight:300;
}

.confirm p{
    position:relative;
    z-index:2;
    margin-top:20px;
    font-size:18px;
    color:rgba(255,255,255,.9);
}

.btn{
    position:relative;
    z-index:2;
    margin-top:40px;
    display:inline-block;
    padding:18px 55px;
    border:1px solid rgba(255,255,255,.7);
    color:white;
    text-decoration:none;
    letter-spacing:2px;
    transition:.35s;
}

.btn:hover{
    background:white;
    color:black;
}

/* ===== MOBILE ===== */

@media(max-width:950px){

    .hero{
        padding:35px;
    }

    .names{
        font-size:52px;
    }

    .details{
        grid-template-columns:1fr;
    }

    .dress{
        grid-template-columns:1fr;
    }

    .gallery{
        grid-template-columns:1fr 1fr;
    }

    .dress-content{
        padding:50px 35px;
    }
}

@media(max-width:650px){

    .hero{
        height:auto;
        min-height:100vh;
        padding-top:100px;
        padding-bottom:80px;
    }

    .names{
        font-size:42px;
    }

    .date{
        font-size:32px;
    }

    .desc{
        font-size:16px;
    }

    .gallery{
        grid-template-columns:1fr;
    }

    .time{
        min-width:120px;
    }

    .number{
        font-size:48px;
    }

    .timer h2,
    .story h2,
    .dress-content h2,
    .confirm h2{
        font-size:42px;
    }
}

</style>
</head>

<body>

<!-- HERO -->

<section class="hero">

    <div class="content">

        <div class="top-text">
            СВАДЬБА
        </div>

        <div class="names">
            ДМИТРИЙ
            <div class="and">&</div>
            АНАСТАСИЯ
        </div>

        <div class="date">
            26.09.2026
        </div>

        <div class="desc">
            С огромной радостью приглашаем вас стать частью самого важного дня нашей жизни
        </div>

        <div class="info">
            <div>📍 СИМФЕРОПОЛЬ</div>
            <div>🏛 РЕСТОРАН «ЧИСТЫЕ ПРУДЫ»</div>
            <div>🕒 НАЧАЛО ТОРЖЕСТВА — 15:00</div>
        </div>

        <div class="arrow">
            ⌄
        </div>

    </div>

</section>

<!-- STORY -->

<section class="story">

    <h2>Наша история</h2>

    <p>
        Любовь — это когда два человека становятся одним миром друг для друга.
        Мы нашли своё счастье и хотим разделить этот день вместе с вами.
        <br><br>
        Спасибо, что вы с нами!
    </p>

</section>

<!-- DETAILS -->

<section class="details">

    <div class="card">
        <h3>Дата</h3>
        <p>26 сентября 2026</p>
    </div>

    <div class="card">
        <h3>Время</h3>
        <p>Сбор гостей с 15:00</p>
    </div>

    <div class="card">
        <h3>Место</h3>
        <p>Ресторан «Чистые пруды»<br>Симферополь</p>
    </div>

</section>

<!-- TIMER -->

<section class="timer">

    <h2>До нашей свадьбы осталось</h2>

    <div class="countdown">

        <div class="time">
            <div class="number" id="days">0</div>
            <div class="label">ДНЕЙ</div>
        </div>

        <div class="time">
            <div class="number" id="hours">0</div>
            <div class="label">ЧАСОВ</div>
        </div>

        <div class="time">
            <div class="number" id="minutes">0</div>
            <div class="label">МИНУТ</div>
        </div>

        <div class="time">
            <div class="number" id="seconds">0</div>
            <div class="label">СЕКУНД</div>
        </div>

    </div>

</section>

<!-- DRESS CODE -->

<section class="dress">

    <div class="dress-image"></div>

    <div class="dress-content">

        <h2>Dress Code</h2>

        <p>
            Мы будем рады, если вы поддержите цветовую палитру нашей свадьбы.
        </p>

        <div class="colors">
            <div class="circle c1"></div>
            <div class="circle c2"></div>
            <div class="circle c3"></div>
            <div class="circle c4"></div>
            <div class="circle c5"></div>
        </div>

    </div>

</section>

<!-- GALLERY -->

<section class="gallery">

<img src="photo.jpg">
<img src="https://images.unsplash.com/photo-1519741497674-611481863552?q=80&w=1974&auto=format&fit=crop">
<img src="https://images.unsplash.com/photo-1519225421980-715cb0215aed?q=80&w=1974&auto=format&fit=crop">
<img src="https://images.unsplash.com/photo-1511285560929-80b456fea0bc?q=80&w=1974&auto=format&fit=crop">

</section>

<!-- CONFIRM -->

<section class="confirm">

    <h2>Подтвердите своё присутствие</h2>

    <p>
        Пожалуйста, подтвердите ваше присутствие до 26 августа 2026 года
    </p>

    <a href="#" class="btn">
        ПОДТВЕРДИТЬ ПРИСУТСТВИЕ
    </a>

</section>

<script>

const weddingDate = new Date("September 26, 2026 15:00:00").getTime();

setInterval(() => {

    const now = new Date().getTime();

    const distance = weddingDate - now;

    const days = Math.floor(distance / (1000 * 60 * 60 * 24));
    const hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
    const minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
    const seconds = Math.floor((distance % (1000 * 60)) / 1000);

    document.getElementById("days").innerHTML = days;
    document.getElementById("hours").innerHTML = hours;
    document.getElementById("minutes").innerHTML = minutes;
    document.getElementById("seconds").innerHTML = seconds;

},1000);

</script>

</body>
</html>
