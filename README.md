<!DOCTYPE html>
<html lang="en">
<head>
    <link rel="stylesheet" href="MarkStore.css">
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>MarkStore.com</title>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>
<body>
<style>
body {
background-color: black;
padding: 20px;
border-radius: 5px;
}
.texts-div { ;
color: yellowgreen;
font-size: 100px 200px;
text-align: center;
}
.registration-form button {
  width: 100%;
  padding: 10px;
  background-color: #4CAF50;
  color: white;
  border: none;
  border-radius: 5px;
  font-size: 16px;
  cursor: pointer;
}

.registration-form button:hover {
  background-color: #45a049;
}
 img {
width: 300px;
}
.nash1 {
    color: white;
    text-align: center;
    font-size: 25px;
}
.nash2 {
    color: white;
    text-align: center;
    font-size: 25px;
}
.nash1 {
width: 50px;
height: 50px;
background-color: black;
position: relative;
animation: nash1 4s infinite alternate;
}
@keyframes nash1 {
    0% {
        transform: translateX(300px);
    }
    100%{
        transform: translateX(0);
    }
}
.nash2 {
width: 50px;
height: 50px;
background-color: black;
position: relative;
animation: nash2 4s infinite alternate;
}
@keyframes nash2 {
    0% {
        transform: translateX(300px);
    }
    100%{
        transform: translateX(0);
    }
}
.info {
font-size: 30px;
color: yellowgreen;
text-align: center;
position: relative;
animation: info 4s infinite alternate;
}
@keyframes info{
    0%{
        transform: translateX(0);
    }
    100%{
        transform: translateX(300px);
    }
}
.info2 {
font-size: 30px;
color: yellowgreen;
text-align: center;
position: relative;
animation: info2 4s  infinite alternate;
}
@keyframes info2{
    0%{
        transform: translateX(0);
    }
    100%{
        transform: translateX(300px);
    }
}
.animated-text {
    font-size: 20px;
    color: yellowgreen;
    opacity: 0; /* Бастапқыда көрінбейді */
    transform: translateY(20px); /* Төмен орналасады */
    animation: fadeIn 2s ease-out forwards; /* Анимацияны қолдану */
}

/* @keyframes арқылы анимацияны анықтаймыз */
@keyframes fadeIn {
    0% {
        opacity: 0;
        transform: translateY(20px); /* Төменнен басталады */
    }
    100% {
        opacity: 1;
        transform: translateY(0); /* Бастапқы орнына келеді */
    }
}
.blure-image {
opacity: 0.5;
transition: opacity 0.3s ease;
filter: blur(3px);
}

.blure-image:hover {
opacity: 1;
filter: blur(0);
}
.airpro{
    font-size: 30px;
    color: yellowgreen;
}

.but-vid {
    text-align: center;
}

.vid {
    text-decoration: none;
    color: white;
    background-color: #007BFF;
    padding: 10px 40px;
    border-radius: 5px;
    font-size: 18px;
    font-weight: bold;
    transition: background-color 0.3s ease;
}

.vid:hover {
    background-color: #0056b3;
}
.zakaz {
    text-align: left;
}

.zakaz1 {
    text-decoration: none;
    color: white;
    background-color: #007BFF;
    padding: 10px 25px;
    border-radius: 10px;
    font-size: 15px;
    font-weight: bold;
    transition: background-color 0.3s ease;
}

.zakaz1:hover {
    background-color: #0056b3;
}
/* Әлеуметтік желілерді контейнерге орналастыру */
.social-links {
    position: fixed;
    top: 10px;
    right: 10px;
    display: flex;
    flex-direction: row; /* Бір қатарда */
    gap: 15px;
}

/* Әлеуметтік желі иконкаларының стилі */
.social-icon {
    display: block;
    width: 50px;
    height: 50px;
    background-color: #333;
    border-radius: 50%;
    overflow: hidden;
    
}

/* Әлеуметтік желілердің иконкаларының суреттері */
.social-icon img {
    width: 100%;
    height: 100%;
    object-fit: cover;
}

/* Әлеуметтік желілердің суреттері басылғанда түс өзгерту */
.instagram:hover {
    transform: scale(1.1);
    background-color: #E1306C;
}

.telegram:hover {
    transform: scale(1.1);
    background-color: #0088cc;
}

.youtube:hover {
    transform: scale(1.1);
    background-color: #FF0000;
}

.whatsapp:hover {
    transform: scale(1.1);
    background-color: #25D366;
}


}
.navbar {
    background-color: #333;
    padding: 10px;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.navbar a {
    color: #FFD700; /* Сары сілтемелер */
    text-decoration: none;
    margin: 0 10px;
    font-size: 18px;
}

.navbar a:hover {
    text-decoration: underline; /* Hover әсер */
}
* {
  box-sizing: border-box; /* Элементтер дұрыс бейімделуі үшін */
}

body {
  margin: 0; /* Қажетсіз бос орындарды алып тастау */
  padding: 0;
  width: 100%;
  overflow-x: hidden; /* Горизонталь жылжытуды жою */
}
hr{
color: yellowgreen;
}

</style>
<div class="navbar">
    <a href="#home">Басты бет</a>
    <a href="#products">Өнімдер</a>
    <a href="#contact">Байланыс</a>
</div>
<div>
<button id="playBtn">Ойнау</button>
<button id="pauseBtn">Тоқтату</button>
<button id="forwardBtn">10 сек алға</button>
<button id="backwardBtn">10 сек артқа</button>
<audio id="music" src="music.mp3"></audio>
</div>
<div class="social-links">
    <a href="https://www.instagram.com/apple?igsh=eDhpYTYyZjBxaGl6" target="_blank" class="social-icon instagram">
        <img src="https://i.pinimg.com/originals/66/8c/7a/668c7a342c3c1f431a25dc9ff2e5ccd4.jpg" alt="Instagram">
    </a>
    <a href="https://t.me/apple" target="_blank" class="social-icon telegram">
        <img src="https://i.pinimg.com/originals/26/c5/45/26c54516bdc6b1476eede71ea7050455.jpg" alt="Telegram">
    </a>
    <a href="https://youtube.com/@apple-fu3mw?si=KFTf79qfe1trmubd" target="_blank" class="social-icon youtube">
        <img src="https://i.pinimg.com/736x/9f/97/d7/9f97d7590ff873e1e40e87d3d88b333f.jpg" alt="YouTube">
    </a>
    <a href="https://wa.me/your-number" target="_blank" class="social-icon whatsapp">
        <img src="https://i.pinimg.com/originals/8f/82/08/8f82081674b7c19714a463168c47bf4e.jpg" alt="WhatsApp">
    </a>
</div>
   <br><br><br>
<div class="texts-div">
   <div class="animated-text"> MarkStore<br><br>НАУШНИК ДУКЕНІ <br><br>бұл дүкен сізге арзан әрі сапалы өнімдегі наушниктерді ұсынады <br></div>
</div><hr>
<div class="nash1"><img src = "https://avatars.mds.yandex.net/i?id=a38e6ed2d91020289869f2b46378881f_l-8249876-images-thumbs&n=13" class="blure-image"></div>
    <div class="info"> AirPods Pro: <br> шуды басатын, <br> су өткізбейтін, <br> сымсыз құлаққаптар, <br> сенсорлы басқару, <br> ұзақ батарея.</div> <br> <br>
    <div class="airpro"> airpods pro <br> бағасы: 5500 тг</div>
    <div class="but-vid">
        <a href="video.html" class="vid">Видео</a>
    </div>
    <div class="zakaz"><a href="https://www.instagram.com/ordabekov.mm/profilecard/?igsh=MTVzemY5MXJ6ZXkzNw==" class="zakaz1">заказ беру ушін басыныз! </a></div> <br>
</div>
<form>
    <label > немесе номер енгізініз:</label>
    <input type="number" id="phone" name="phone" placeholder="номер жазыныз">
    <button type="sumbit">жберу</button>
</form> <br> <br> <br>
<hr>
 <div class="nash2"><img src="https://cdn.mos.cms.futurecdn.net/tRftM9zcFhGs62QHQ7Fb66.png" class="blure-image"> </div>
     <div class="info2"><h5><p2> AirPods 3: <br> кеңістіктік дыбыс, <br> су өткізбейтін, <br> жақсартылған дыбыс, <br> ұзақ батарея, <br> сымсыз зарядтау, <br> сенсорлы басқару. </p2></h5></div>
<br>
<br>
<br>
    <div class="airpro"> airpods 3 <br> бағасы: 6500 тг</div>
    <div class="but-vid">
        <a href="video.html" class="vid">Видео</a>
    </div>
    <div class="zakaz"><a href="https://www.instagram.com/ordabekov.mm/profilecard/?igsh=MTVzemY5MXJ6ZXkzNw==" class="zakaz1">заказ беру ушін басыныз! </a></div> <br>
<form>
    <label > немесе номер енгізініз:</label>
    <input type="number" id="phone" name="phone" placeholder="номер жазыныз">
    <button type="sumbit">жберу</button>
</form> <br> <br> <br> 
<hr>
<div class="nash1"><img src = "https://get.wallhere.com/photo/AKG-headphones-1876947.jpg" class="blure-image"></div>
    <div class="info"> ACG Pro: <br> шуды басатын, <br> су өткізбейтін, <br> сымсыз құлаққаптар, <br> сенсорлы басқару, <br> ұзақ батарея. </div> <br> <br>
     <div class="airpro"> ACG Pro <br> бағасы: 5500 тг</div>
    <div class="but-vid">
        <a href="video.html" class="vid">Видео</a>
    </div>
    <div class="zakaz"><a href="https://www.instagram.com/ordabekov.mm/profilecard/?igsh=MTVzemY5MXJ6ZXkzNw==" class="zakaz1">заказ беру ушін басыныз! </a></div> <br>
<form>
    <label > немесе номер енгізініз:</label>
    <input type="number" id="phone" name="phone" placeholder="номер жазыныз">
    <button type="sumbit">жберу</button>
</form> <br> <br> <br>
<hr>
<div class="nash1"><img src = "https://i.ytimg.com/vi/3vvqXDkARyQ/maxresdefault.jpg" class="blure-image"></div>
    <div class="info"> SpeedArt: <br> шуды басатын, <br> су өткізбейтін, <br> сымсыз құлаққаптар, <br> сенсорлы басқару, <br> ұзақ батарея.</div> <br> <br>
    <div class="airpro"> SpeedArt <br> бағасы: 5500 тг</div>
    <div class="but-vid">
        <a href="video.html" class="vid">Видео</a>
    </div>
    <div class="zakaz"><a href="https://www.instagram.com/ordabekov.mm/profilecard/?igsh=MTVzemY5MXJ6ZXkzNw==" class="zakaz1">заказ беру ушін басыныз! </a></div><br>
<form>
    <label > немесе номер енгізініз:</label>
    <input type="number" id="phone" name="phone" placeholder="номер жазыныз">
    <button type="sumbit">жберу</button>
</form> <br> <br> <br>
<hr>
<div class="nash1"><img src = "https://i.ytimg.com/vi/MxZD3ZIR0Go/maxresdefault.jpg" class="blure-image"></div>
    <div class="info"> JonyFirst: <br> шуды басатын, <br> су өткізбейтін, <br> сымсыз құлаққаптар, <br> сенсорлы басқару, <br> ұзақ батарея.</div> <br> <br>
     <div class="airpro"> Jonyfirst <br> бағасы: 5500 тг</div>
    <div class="but-vid">
        <a href="video.html" class="vid">Видео</a>
    </div>
    <div class="zakaz"><a href="https://www.instagram.com/ordabekov.mm/profilecard/?igsh=MTVzemY5MXJ6ZXkzNw==" class="zakaz1">заказ беру ушін басыныз! </a></div> <br>
<form>
    <label > немесе номер енгізініз:</label>
    <input type="number" id="phone" name="phone" placeholder="номер жазыныз">
    <button type="sumbit">жберу</button>
</form> <br> <br> <br>
<hr>

<script>
    // Элементтерді таңдау
const playButton = document.getElementById('playBtn');
const pauseButton = document.getElementById('pauseBtn');
const forwardButton = document.getElementById('forwardBtn');
const backwardButton = document.getElementById('backwardBtn');
const music = document.getElementById('music');

// Ойнау батырмасы
playButton.addEventListener('click', () => {
    music.play(); // Музыканы ойнату
});

// Тоқтату батырмасы
pauseButton.addEventListener('click', () => {
    music.pause(); // Музыканы тоқтату
});
// Алға 10 секунд
forwardButton.addEventListener('click', () => {
    music.currentTime += 10; // Ағымдағы уақытқа 10 секунд қосу
});

// Артқа 10 секунд
backwardButton.addEventListener('click', () => {
    music.currentTime -= 10; // Ағымдағы уақыттан 10 секунд шегеру
});
    
</script>



</body>
</html>
