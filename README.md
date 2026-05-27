<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Дмитрий & Анастасия — Свадьба</title>

  <link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@300;400;600&family=Montserrat:wght@300;400;500&display=swap" rel="stylesheet">

  <style>
    *{
      margin:0;
      padding:0;
      box-sizing:border-box;
      scroll-behavior:smooth;
    }

    body{
      background:#0e0e0e;
      color:white;
      font-family:'Montserrat',sans-serif;
      overflow-x:hidden;
    }

    section{
      position:relative;
      width:100%;
    }

    .hero{
      height:100vh;
      background:url('https://images.unsplash.com/photo-1511285560929-80b456fea0bc?q=80&w=1974&auto=format&fit=crop') center/cover no-repeat;
      display:flex;
      align-items:center;
      padding:60px;
    }

    .overlay{
      position:absolute;
      inset:0;
      background:rgba(0,0,0,.55);
    }

    .content{
      position:relative;
      z-index:2;
      max-width:520px;
    }

    .mini{
      letter-spacing:6px;
      font-size:12px;
      margin-bottom:25px;
      opacity:.8;
    }

    h1{
      font-family:'Cormorant Garamond',serif;
      font-size:72px;
      font-weight:300;
      line-height:1;
      margin-bottom:20px;
    }

    .amp{
      font-size:50px;
      margin:10px 0;
    }

    .date{
      font-size:38px;
      margin:25px 0;
      font-family:'Cormorant Garamond',serif;
    }

    .text{
      font-size:17px;
      line-height:1.8;
      opacity:.92;
      margin-bottom:35px;
    }

    .info{
      display:flex;
      flex-direction:column;
      gap:16px;
      font-size:16px;
    }

    .info div{
      display:flex;
      align-items:center;
      gap:12px;
    }

    .arrow{
      margin-top:45px;
      font-size:40px;
      animation:down 1.8s infinite;
    }

    @keyframes down{
      0%{transform:translateY(0)}
      50%{transform:translateY(10px)}
      100%{transform:translateY(0)}
    }

    .story{
      padding:100px 10%;
      background:url('https://images.unsplash.com/photo-1519167758481-83f550bb49b3?q=80&w=1974&auto=format&fit=crop') center/cover no-repeat;
    }

    .dark{
      background:rgba(0,0,0,.7);
      padding:60px;
      backdrop-filter:blur(3px);
    }

    h2{
      font-family:'Cormorant Garamond',serif;
      font-size:46px;
      margin-bottom:30px;
      font-weight:300;
    }

    .story p{
      line-height:2;
      max-width:700px;
      font-size:18px;
    }

    .details{
      display:grid;
      grid-template-columns:repeat(3,1fr);
      gap:30px;
      padding:90px 10%;
      background:#121212;
    }

    .card{
      border:1px solid rgba(255,255,255,.15);
      padding:45px 25px;
      text-align:center;
      background:rgba(255,255,255,.03);
    }

    .card h3{
      font-family:'Cormorant Garamond',serif;
      font-size:34px;
      margin-bottom:15px;
      font-weight:300;
    }

    .timer{
      padding:100px 10%;
      text-align:center;
      background:#0b0b0b;
    }

    .countdown{
      display:flex;
      justify-content:center;
      gap:35px;
      margin-top:40px;
      flex-wrap:wrap;
    }

    .time{
      min-width:140px;
      padding:30px;
      border:1px solid rgba(255,255,255,.15);
    }

    .num{
      font-size:58px;
      font-family:'Cormorant Garamond',serif;
    }

    .label{
      margin-top:10px;
      opacity:.75;
      letter-spacing:2px;
    }

    .dress{
      display:grid;
      grid-template-columns:1fr 1fr;
      min-height:500px;
    }

    .dress-img{
      background:url('https://images.unsplash.com/photo-1512436991641-6745cdb1723f?q=80&w=1974&auto=format&fit=crop') center/cover no-repeat;
    }

    .dress-content{
      padding:80px;
      display:flex;
      flex-direction:column;
      justify-content:center;
      background:#111;
    }

    .colors{
      display:flex;
      gap:18px;
      margin-top:35px;
    }

    .circle{
      width:42px;
      height:42px;
      border-radius:50%;
      border:1px solid rgba(255,255,255,.3);
    }

    .c1{background:#ffffff;}
    .c2{background:#d9d2ca;}
    .c3{background:#b9aea3;}
    .c4{background:#6d6d6d;}
    .c5{background:#000000;}

    .gallery{
      display:grid;
      grid-template-columns:repeat(4,1fr);
    }

    .gallery img{
      width:100%;
      height:260px;
      object-fit:cover;
    }

    .confirm{
      padding:120px 10%;
      text-align:center;
      background:url('https://images.unsplash.com/photo-1519225421980-715cb0215aed?q=80&w=1974&auto=format&fit=crop') center/cover no-repeat;
      position:relative;
    }

    .confirm::before{
      content:'';
      position:absolute;
      inset:0;
      background:rgba(0,0,0,.7);
    }

    .confirm-content{
      position:relative;
      z-index:2;
    }

    .btn{
      display:inline-block;
      margin-top:35px;
      padding:18px 55px;
      border:1px solid white;
      color:white;
      text-decoration:none;
      letter-spacing:2px;
      transition:.4s;
    }

    .btn:hover{
      background:white;
      color:black;
    }

    @media(max-width:900px){

      .hero{
        padding:30px;
      }

      h1{
        font-size:48px;
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
        padding:45px 30px;
      }

      .dark{
        padding:35px;
      }
    }

    @media(max-width:600px){

      h1{
        font-size:40px;
      }

      .date{
        font-size:28px;
      }

      .gallery{
        grid-template-columns:1fr;
      }

      .countdown{
        gap:15px;
      }

      .time{
        min-width:110px;
      }

      .num{
        font-size:42px;
      }
    }
  </style>
</head>
<body>

<section class="hero">
  <div class="overlay"></div>

  <div class="content">
    <div class="mini">СВАДЬБА</div>

    <h1>
      ДМИТРИЙ
      <div class="amp">&</div>
      АНАСТАСИЯ
    </h1>

    <div class="date">26.09.2026</div>

    <div class="text">
      С огромной радостью приглашаем вас стать частью самого важного дня нашей жизни
    </div>

    <div class="info">
      <div>📍 Симферополь</div>
      <div>🏛 Ресторан «Чистые пруды»</div>
      <div>🕒 Начало торжества — 15:00</div>
    </div>

    <div class="arrow">⌄</div>
  </div>
</section>

<section class="story">
  <div class="dark">
    <h2>Наша история</h2>

    <p>
      Любовь — это когда два человека становятся одним миром друг для друга.
      Мы нашли своё счастье и хотим разделить этот день вместе с вами.
      <br><br>
      Спасибо, что вы с нами!
    </p>
  </div>
</section>

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

<section class="timer">

  <h2>До нашей свадьбы осталось</h2>

  <div class="countdown">

    <div class="time">
      <div class="num" id="days">0</div>
      <div class="label">ДНЕЙ</div>
    </div>

    <div class="time">
      <div class="num" id="hours">0</div>
      <div class="label">ЧАСОВ</div>
    </div>

    <div class="time">
      <div class="num" id="minutes">0</div>
      <div class="label">МИНУТ</div>
    </div>

    <div class="time">
      <div class="num" id="seconds">0</div>
      <div class="label">СЕКУНД</div>
    </div>

  </div>

</section>

<section class="dress">

  <div class="dress-img"></div>

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

<section class="gallery">

  <img src="https://images.unsplash.com/photo-1519741497674-611481863552?q=80&w=1974&auto=format&fit=crop">
  <img src="https://images.unsplash.com/photo-1522673607200-164d1b6ce486?q=80&w=1974&auto=format&fit=crop">
  <img src="https://images.unsplash.com/photo-1511285560929-80b456fea0bc?q=80&w=1974&auto=format&fit=crop">
  <img src="https://images.unsplash.com/photo-1519225421980-715cb0215aed?q=80&w=1974&auto=format&fit=crop">

</section>

<section class="confirm">

  <div class="confirm-content">

    <h2>Подтвердите своё присутствие</h2>

    <p>
      Пожалуйста, подтвердите ваше присутствие до 26 августа 2026 года
    </p>

    <a href="#" class="btn">ПОДТВЕРДИТЬ ПРИСУТСТВИЕ</a>

  </div>

</section>

<script>

const weddingDate = new Date("September 26, 2026 15:00:00").getTime();

const timer = setInterval(function(){

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
