<!DOCTYPE html>
<html>
<head>
<title>Upin Fried Chicken</title>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<link rel="stylesheet" href="https://www.w3schools.com/w3css/4/w3.css">
<style>
body {font-family: "Times New Roman", Georgia, Serif;}
h1, h2, h3, h4, h5, h6 {
  font-family: "Playfair Display";
  letter-spacing: 5px;
}
</style>
</head>
<body>

<!-- Navbar (sit on top) -->
<div class="w3-top">
  <div class="w3-bar w3-white w3-padding w3-card" style="letter-spacing:4px;">
    <a href="#home" class="w3-bar-item w3-button">Upin Fried Chicken</a>
    <!-- Right-sided navbar links. Hide them on small screens -->
    <div class="w3-right w3-hide-small">
      <a href="#about" class="w3-bar-item w3-button">About</a>
      <a href="#menu" class="w3-bar-item w3-button">Menu</a>
      <a href="#contact" class="w3-bar-item w3-button">Contact</a>
    </div>
  </div>
</div>

<style>
  * {box-sizing: border-box}
  body {font-family: Verdana, sans-serif; margin:0}
  .mySlides {display: none}
  img {vertical-align: center;}
  
  /* Slideshow container */
  .slideshow-container {
    max-width: 1000px;
    position: relative;
    margin: auto;
  }
  
  /* Next & previous buttons */
  .prev, .next {
    cursor: pointer;
    position: absolute;
    top: 50%;
    width: auto;
    padding: 16px;
    margin-top: -22px;
    color: white;
    font-weight: bold;
    font-size: 18px;
    transition: 0.6s ease;
    border-radius: 0 3px 3px 0;
    user-select: none;
  }
  
  /* Position the "next button" to the right */
  .next {
    right: 0;
    border-radius: 3px 0 0 3px;
  }
  
  /* On hover, add a black background color with a little bit see-through */
  .prev:hover, .next:hover {
    background-color: rgba(0,0,0,0.8);
  }
  
  /* Caption text */
  .text {
    color: #f2f2f2;
    font-size: 15px;
    padding: 8px 12px;
    position: absolute;
    bottom: 8px;
    width: 100%;
    text-align: center;
  }
  
  /* Number text (1/3 etc) */
  .numbertext {
    color: #f2f2f2;
    font-size: 12px;
    padding: 8px 12px;
    position: absolute;
    top: 0;
  }
  
  /* The dots/bullets/indicators */
  .dot {
    cursor: pointer;
    height: 15px;
    width: 15px;
    margin: 0 2px;
    background-color: #bbb;
    border-radius: 50%;
    display: inline-block;
    transition: background-color 0.6s ease;
  }
  
  .active, .dot:hover {
    background-color: #717171;
  }
  
  /* Fading animation */
  .fade {
    animation-name: fade;
    animation-duration: 1.5s;
  }
  
  @keyframes fade {
    from {opacity: .4} 
    to {opacity: 1}
  }
  
  /* On smaller screens, decrease text size */
  @media only screen and (max-width: 300px) {
    .prev, .next,.text {font-size: 11px}
  }
  </style>
  </head>
  <body>
  
  <div class="slideshow-container">

  <div class="mySlides fade">
    <div class="numbertext">1 / 3</div>
    <img src="home 1.jpg" style="width:100%" id="home">
    <div class="text">Ayo cobain sensasi ayam goreng terbaik dari Upin Fried Chicken. <br> Mulai hari ini, nikmati promo spesial untuk setiap pembelian paket keluarga!</div>
  </div>
  
  <div class="mySlides fade">
    <div class="numbertext">2 / 3</div>
    <img src="home 2.jpg" style="width:100%" id="home 2">
    <div class="text">Manjakan lidahmu dengan ayam goreng renyah dari Upin Fried Chicken.<br>Gurihnya sempurna, bumbunya meresap sampai ke tulang! </div>
  </div>
  
  <div class="mySlides fade">
    <div class="numbertext">3 / 3</div>
    <img src="home 3.jpg." style="width:100%" id="home 3">
    <div class="text">Nikmati ayam goreng favorit semua usia—gurih, renyah, dan selalu fresh!<br>Pas banget untuk momen kumpul bareng orang tersayang.</div>
  </div>

  <a class="prev" onclick="plusSlides(-1)">❮</a>
  <a class="next" onclick="plusSlides(1)">❯</a>
  
  </div>
  <br>
  
  <div style="text-align:center">
    <span class="dot" onclick="currentSlide(1)"></span> 
    <span class="dot" onclick="currentSlide(2)"></span> 
    <span class="dot" onclick="currentSlide(3)"></span> 
  </div>
  
  <script>
  let slideIndex = 1;
  showSlides(slideIndex);
  
  function plusSlides(n) {
    showSlides(slideIndex += n);
  }
  
  function currentSlide(n) {
    showSlides(slideIndex = n);
  }
  
  function showSlides(n) {
    let i;
    let slides = document.getElementsByClassName("mySlides");
    let dots = document.getElementsByClassName("dot");
    if (n > slides.length) {slideIndex = 1}    
    if (n < 1) {slideIndex = slides.length}
    for (i = 0; i < slides.length; i++) {
      slides[i].style.display = "none";  
    }
    for (i = 0; i < dots.length; i++) {
      dots[i].className = dots[i].className.replace(" active", "");
    }
    slides[slideIndex-1].style.display = "block";  
    dots[slideIndex-1].className += " active";
  }
  </script>

<!-- Page content -->
<div class="w3-content" style="max-width:1100px">

  <!-- About Section -->
  <div class="w3-row w3-padding-64" id="about">
    <div class="w3-col m6 w3-padding-large w3-hide-small">
     <img src="about.jpg" class="w3-round w3-image w3-opacity-min" alt="Table Setting" width="600" height="750">
    </div>

    <div class="w3-col m6 w3-padding-large">
      <h1 class="w3-center">Selamat Datang di Upin Fried Chicken</h1><br>
      <h5 class="w3-center">Berdiri sejak 2010</h5>
      <p class="w3-large">Nikmati sensasi kelezatan ayam goreng yang renyah, gurih, dan penuh cita rasa khas! Upin Fried Chicken adalah destinasi sempurna bagi para pecinta ayam goreng crispy dengan cita rasa spesial yang cocok untuk seluruh keluarga. Dibuat dengan bahan-bahan berkualitas terbaik dan bumbu rahasia istimewa, setiap gigitan ayam goreng kami memberikan <span class="w3-tag w3-light-grey">kepuasan tak terlupakan.</span></p>
      <p class="w3-large w3-text-grey w3-hide-medium">Experience the Crispy, Savory, and Unforgettable Delight of Fried Chicken! Upin Fried Chicken is the perfect destination for lovers of crispy fried chicken with a unique and special flavor, perfect for the whole family. Made with the finest quality ingredients and a signature secret recipe, every bite of our fried chicken delivers unparalleled satisfaction.</p>
    </div>
  </div>
  
  <hr>
  
  <!-- Menu Section -->
  <div class="w3-row w3-padding-64" id="menu">
    <div class="w3-col l6 w3-padding-large">
      <h1 class="w3-center">Menu Andalan</h1><br>
      <h4>Ayam Goreng Spesial Upin:</h4>
      <p class="w3-text-grey">Ayam goreng renyah dengan bumbu spesial yang meresap hingga ke tulang. <span class="w3-tag w3-light-grey">Rp.25.000</span> </p><br>
    
      <h4>Paket Hemat Keluarga:</h4>
      <p class="w3-text-grey">Pilihan paket komplit dengan ayam, nasi, kentang goreng, dan minuman menyegarkan. <span class="w3-tag w3-light-grey">Rp.140.000</span></p><br>
    
      <h4>Paket Ayam Goreng 2 Potong</h4>
      <p class="w3-text-grey">Lebih puas dengan 2 potong ayam goreng, nasi, dan minuman. <span class="w3-tag w3-light-grey">Rp.40.000</span> </p><br>
    
      <h4>Ayam Goreng Pedas (1 Potong)</h4>
      <p class="w3-text-grey">Untuk pencinta pedas! Ayam goreng dengan bumbu pedas spesial. <span class="w3-tag w3-light-grey">Rp.18.000</span></p><br>
    
      <h4>Nugget Ayam (6 pcs) </span></h4>
      <p class="w3-text-grey">Nugget ayam renyah dengan rasa lezat. <span class="w3-tag w3-light-grey">Rp.20.000</p>    
    </div>
    
    <div class="w3-col l6 w3-padding-large">
      <img src="menu.jpg" class="w3-round w3-image w3-opacity-min" alt="Menu" style="width:100%">
    </div>
  </div>

  <hr>

  <!-- Contact Section -->
  <div class="w3-container w3-padding-64" id="contact">
    <h1>Contact</h1><br>
    <p>Nikmati kelezatan Upin Fried Chicken tanpa perlu keluar rumah!<br>
      Kami hadir dengan layanan pengantaran yang cepat, aman, dan higienis langsung ke depan pintu Anda. Dengan tim kami yang profesional, pesanan Anda akan sampai dalam keadaan hangat, renyah, dan penuh rasa.</p>
    <p class="w3-text-blue-grey w3-large"><b>Upin Fried Chicken Surakarta, Jl. Ayam Goreng No. 15, Jebres, Surakarta</b></p>
    <p>Jika Anda memiliki pertanyaan, ingin memesan, atau membutuhkan bantuan, tim Upin Fried Chicken selalu siap melayani Anda!<br>
    Hubungi melalui Whatsapp +62 812 3456 7890 atau email upinfriedchicken@gmail.com</p>
    <form action="/action_page.php" target="_blank">
      <p><input class="w3-input w3-padding-16" type="text" placeholder="Nama" required name="Name"></p>
      <p><input class="w3-input w3-padding-16" type="number" placeholder="Banyaknya pesanan" required name="People"></p>
      <p><input class="w3-input w3-padding-16" type="datetime-local" placeholder="Date and time" required name="date" value="2020-11-16T20:00"></p>
      <p><input class="w3-input w3-padding-16" type="text" placeholder="Pesanan \ catatan khusus" required name="Message"></p>
      <p><button class="w3-button w3-light-grey w3-section" type="submit">KIRIM PESAN</button></p>
    </form>
  </div>
  
<!-- End page content -->
</div>

<!-- Footer -->
<footer class="w3-center w3-light-grey w3-padding-32">
  <p>© Argaventa Aryadharma NIM.C0722022</a></p>
</footer>

</body>
</html>
