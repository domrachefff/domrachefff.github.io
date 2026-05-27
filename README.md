ion:.3s;
    }

    button:hover{
      background:#d8d8d8;
    }

    footer{
      padding:60px 20px;
      text-align:center;
      opacity:.7;
      font-size:14px;
    }

    [club66008961|@keyframes] fade{
      from{
        opacity:0;
        transform:translateY(30px);
      }
      to{
        opacity:1;
        transform:translateY(0);
      }
    }

    [id705766|max-width:768px]{

      h1{
        font-size:58px;
      }

      .story{
        grid-template-columns:1fr;
      }

      .timer-box{
        width:120px;
        height:120px;
      }

      .timer-box span{
        font-size:40px;
      }

    }

  </style>
</head>

<body>

<section class="hero">

  <div class="hero-content">

    <div class="subtitle">
      WEDDING DAY
    </div>

    <h1>
      Дмитрий 

      & 

      Анастасия
    </h1>

    <div class="date">
      26 • 09 • 2026
    </div>

    <div class="text">
      С огромной радостью приглашаем вас
      стать частью самого важного дня нашей жизни
    </div>

    <div class="info">
      <div>📍 Симферополь</div>
      <div>🏛 Ресторан «Чистые пруды»</div>
      <div>🕓 Начало торжества — 15:00</div>
    </div>

  </div>

</section>

<section class="section">

  <div class="section-title">
    Наша история
  </div>

  <div class="story">

    <img src="your-photo-2.jpg">

    <div class="story-text">
      Любовь — это когда два человека
      становятся одним миром друг для друга.
      <br

    Мы нашли своё счастье
      и хотим разделить этот день вместе с вами.
    </div>

  </div>

</section>

<section class="section">

  <div class="section-title">
    Детали торжества
  </div>

  <div class="details">

    <div class="card">
      <h3>Дата</h3>
      <p>26 сентября 2026</p>
    </div>

    <div class="card">
      <h3>Время</h3>
      <p>15:00</p>
    </div>

    <div class="card">
      <h3>Место</h3>
      <p>Ресторан «Чистые пруды»<br
ферополь</p>
    </div>

  </div>

</section>

<section class="section">

  <div class="section-title">
    До свадьбы осталось
  </div>

  <div class="timer">

    <div class="timer-box">
      <span id="days">0</span>
      дней
    </div>

    <div class="timer-box">
      <span id="hours">0</span>
      часов
    </div>

    <div class="timer-box">
      <span id="minutes">0</span>
      минут
    </div>

    <div class="timer-box">
      <span id="seconds">0</span>
      секунд
    </div>

  </div>

</section>

<section class="section dress">

  <div class="section-title">
    Dress Code
  </div>

  <div class="text">
    Loft Elegant
    <br

  Будем рады,
    если вы поддержите цветовую гамму свадьбы
  </div>

  <div class="colors">

    <div class="color white"></div>
    <div class="color beige"></div>
    <div class="color black"></div>

  </div>

</section>

<section class="section rsvp">

  <div class="section-title">
    Подтвердите присутствие
  </div>

  <form>

    <input type="text" placeholder="Ваше имя">

    <input type="text" placeholder="Телефон">

    <button>
      Подтвердить
    </button>

  </form>

</section>

<footer>
  Дмитрий & Анастасия — 2026
</footer>

<audio autoplay loop>
  <source src="music.mp3" type="audio/mpeg">
</audio>

<script>

const weddingDate = new Date("Sep 26, 2026 15:00:00").getTime();

setInterval(function(){

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
</html> transit
