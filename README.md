<html lang="pl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Kacper Milcarz – Grafik</title>

<link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@900&family=Inter:wght@300;400;600&display=swap" rel="stylesheet">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">

<style>
*{margin:0;padding:0;box-sizing:border-box}
html{scroll-behavior:smooth;}
body{background:#0f0f0f;color:#fff;font-family:'Inter',sans-serif;}

/* ===== HEADER ===== */
header{padding:80px 20px 60px;text-align:center;background:radial-gradient(circle at top,#222,#000);}
header h1{font-size:2.6rem;margin-bottom:10px;font-family:Impact,'Arial Black',sans-serif;}
header p{opacity:.7;font-size:.95rem;}

/* ===== O MNIE ===== */
.about-me{margin-top:35px;max-width:620px;margin-inline:auto;padding:25px;background:#151515;border-radius:18px;transition:.4s;}
.about-me:hover{transform:translateY(-6px);box-shadow:0 0 30px rgba(255,255,255,.12);}
.about-me p{font-size:.9rem;line-height:1.7;opacity:.85;}

/* ===== KAFELKI ===== */
.tiles{margin-top:50px;display:grid;grid-template-columns:repeat(auto-fit,minmax(160px,1fr));gap:20px;max-width:900px;margin-inline:auto;}
.tile{background:#151515;padding:25px 20px;border-radius:18px;text-align:center;cursor:pointer;transition:.35s;text-decoration:none;color:#fff;}
.tile i{font-size:1.6rem;margin-bottom:12px;opacity:.85;}
.tile span{display:block;font-size:.85rem;letter-spacing:1px;}
.tile:hover{transform:translateY(-8px);box-shadow:0 15px 35px rgba(0,0,0,.7);}

/* ===== MAIN ===== */
main{padding:80px 20px;display:flex;flex-direction:column;gap:80px;align-items:center;}

/* ===== PRACE ===== */
.gallery{width:100%;max-width:1100px;display:grid;grid-template-columns:repeat(auto-fit,minmax(260px,1fr));gap:30px;}
.work{background:#151515;padding:25px;border-radius:18px;cursor:pointer;}
.work h2{font-family:Impact,'Arial Black',sans-serif;margin-bottom:8px;}

/* ===== PORTFOLIO ===== */
#portfolio{width:100%;max-width:900px;}
.portfolio-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(220px,1fr));gap:20px;}
.portfolio-item{background:#151515;border-radius:16px;overflow:hidden;text-align:center;padding-bottom:15px;transition:.3s;position:relative;}
.portfolio-item:hover{transform:translateY(-6px);}
.portfolio-item img{width:100%;height:200px;object-fit:contain;filter:grayscale(100%);transition:.3s;cursor:pointer;}
.portfolio-item:hover img{filter:grayscale(0%);}
.read-more{display:inline-block;margin-top:12px;font-size:.8rem;cursor:pointer;opacity:.85;transition:.3s;}
.read-more:hover{letter-spacing:1px;}

/* ===== ACCORDION (CENNIK) ===== */
.accordion-btn{background:#151515;color:#fff;cursor:pointer;padding:15px;border:none;text-align:left;outline:none;font-size:1rem;width:100%;border-radius:12px;margin-bottom:8px;transition:.3s;}
.accordion-btn:hover{background:#222;}
.panel{padding:0 15px;display:none;background:#111;border-radius:12px;margin-bottom:10px;}
.panel ul{list-style:none;padding:10px 0;}
.panel li{padding:5px 0;border-bottom:1px solid #222;}
.panel li:last-child{border-bottom:none;}

/* ===== MODALE ===== */
.modal{display:none;position:fixed;inset:0;background:rgba(0,0,0,.95);justify-content:center;align-items:center;z-index:9999;}
.modal.active{display:flex;}
.modal img{max-width:95%;max-height:95%;border-radius:16px;}

/* ===== FORMULARZ ===== */
.form-box{width:420px;padding:40px;background:#111;border-radius:18px;}
.form-box h2{text-align:center;margin-bottom:30px;}
.input-box{margin-bottom:25px;}
.input-box input,.input-box select{width:100%;padding:12px;background:transparent;border:none;border-bottom:2px solid #444;color:#fff;}
button{width:100%;padding:14px;border:none;background:#fff;color:#000;border-radius:30px;font-weight:600;cursor:pointer;}

/* ===== MEDIA / KONTAKT ===== */
.links,.contact{background:#151515;padding:35px;border-radius:18px;text-align:center;max-width:900px;width:100%;}
.links a{display:block;margin:12px 0;color:#fff;text-decoration:none;}
#scheduleBtn{display:inline-block;margin-top:15px;padding:12px 22px;background:#fff;color:#000;border-radius:22px;cursor:pointer;}
footer{text-align:center;padding:30px;font-size:.7rem;opacity:.4;}
</style>
</head>

<body>

<header id="about">
  <h1>Kacper Milcarz – Grafik</h1>
  <p>Grafika, która przyciąga uwagę w mediach społecznościowych</p>
  <div class="about-me">
    <p>Jestem grafikiem specjalizującym się w projektach sportowych oraz grafikach do social mediów. Tworzę estetyczne i dynamiczne materiały, które budują wizerunek i zwiększają zaangażowanie w internecie.</p>
  </div>
  <div class="tiles">
    <a href="#works" class="tile"><i class="fa-solid fa-pen-nib"></i><span>Prace</span></a>
    <a href="#portfolio" class="tile"><i class="fa-solid fa-image"></i><span>Portfolio</span></a>
    <a href="#pricing" class="tile"><i class="fa-solid fa-list"></i><span>Cennik</span></a>
    <a href="#media" class="tile"><i class="fa-solid fa-hashtag"></i><span>Media</span></a>
    <a href="#contact" class="tile"><i class="fa-solid fa-phone"></i><span>Kontakt</span></a>
  </div>
</header>

<main>

<!-- PRACE -->
<section id="works" class="gallery">
  <div class="work"><h2>Strony internetowe</h2><p>Projekowanie dla firm, klubów sportowych oraz twórców.</p></div>
  <div class="work"><h2>Social Media</h2><p>Prowadzenie Facebooka, Instagrama, TikToka.</p></div>
  <div class="work"><h2>Event i reklamy</h2><p>Banery i grafiki reklamowe.</p></div>
</section>

<!-- PORTFOLIO -->
<section id="portfolio">
  <h2 style="text-align:center;margin-bottom:30px;">Portfolio</h2>
  <div class="portfolio-grid">
    <div class="portfolio-item">
      <img src="https://i.postimg.cc/mhHPWRNQ/Grafika-Wynik-Meczu-Wierna-Malogoszcz.jpg" onclick="openModal(this)">
    </div>
    <div class="portfolio-item">
      <img src="https://i.postimg.cc/DmXS3FdP/Grafika-Sklad-Wierna-Malogoszcz.jpg" onclick="openModal(this)">
    </div>
    <div class="portfolio-item">
      <img src="https://i.postimg.cc/0rwz1xdd/Grafika-Dzien-Meczowy-Wierna-Malogoszcz.jpg" onclick="openModal(this)">
      <span class="read-more" onclick="showMore()">Czytaj więcej</span>
    </div>
  </div>
  <div id="moreImages" style="display:none; margin-top:20px;" class="portfolio-grid">
    <div class="portfolio-item"><img src="https://i.postimg.cc/KKjYqyvV/Picsart-26-02-13-17-36-50-090.jpg" onclick="openModal(this)"></div>
    <div class="portfolio-item"><img src="https://i.postimg.cc/gwj0SP2b/Picsart-26-02-14-17-58-01-515.jpg" onclick="openModal(this)"></div>
    <div class="portfolio-item"><img src="https://i.postimg.cc/VSvNGckQ/Picsart-26-02-14-20-42-41-620.jpg" onclick="openModal(this)"></div>
    <div class="portfolio-item">
  <img src="https://i.postimg.cc/BL9Hxbmx/2-20260306-211005-0001.png" onclick="openModal(this)">
</div>

<div class="portfolio-item">
  <img src="https://i.postimg.cc/9R5ZG0L1/3-20260306-211005-0002.png" onclick="openModal(this)">
    </div>
    <div class="portfolio-item"><img src="https://i.postimg.cc/8FcCKVz8/Picsart-26-02-15-00-24-47-924.jpg" onclick="openModal(this)"></div>
  </div>
</section>

<!-- CENNIK / OFERTA -->
<section id="pricing" class="links">
  <h2 style="text-align:center;margin-bottom:30px;">Oferta usług graficznych / Cennik</h2>

  <!-- Reklamy i marketing -->
  <button class="accordion-btn">Reklamy i marketing</button>
  <div class="panel">
    <ul>
      <li>Projektowanie bannerów, plakatów, ulotek, billboardów – 150 zł/szt</li>
      <li>Wizytówki – 120 zł/szt</li>
    </ul>
  </div>

  <!-- Grafiki do mediów społecznościowych -->
  <button class="accordion-btn">Grafiki do mediów społecznościowych</button>
  <div class="panel">
    <ul>
      <li>Grafiki na kanały social media (Facebook, Instagram, TikTok) – 150 zł/szt</li>
      <li>Miniaturki do filmów na YouTube – 140 zł/szt</li>
      <li>Szablony do Instagram Stories, postów i reelsów – 160 zł/szt</li>
    </ul>
  </div>

  <!-- Branding i identyfikacja wizualna -->
  <button class="accordion-btn">Branding i identyfikacja wizualna</button>
  <div class="panel">
    <ul>
      <li>Tworzenie logo – od 400 zł</li>
      <li>System identyfikacji wizualnej firmy – 800 zł</li>
      <li>Projektowanie stron internetowych – wycena indywidualna </li>
    </ul>
  </div>

  <!-- Współprace -->
  <button class="accordion-btn">Współprace – prowadzenie Social Mediów</button>
  <div class="panel">
    <ul>
      <li>Basic: 4 grafiki tygodniowo – 300 zł/mies</li>
      <li>Standard: 7 grafik tygodniowo – 500 zł/mies</li>
      <li>Premium: 7 grafik tygodniowo + animacje – 600 zł/mies</li>
        </ul>
      </li>
      <li>Miniaturki do filmów na YouTube:
        <ul>
          <li>4/mies – 400 zł</li>
          <li>8/mies – 800 zł</li>
          <li>12/mies – 1000 zł</li>
        </ul>
      </li>
      <li>Szablony do Instagram Stories, postów i reelsów:
        <ul>
          <li>5 szablonów – 600 zł</li>
          <li>10 szablonów – 1200 zł</li>
        </ul>
      </li>
    </ul>
  </div>

  <!-- Współprace z klubami sportowymi -->
  <button class="accordion-btn">Współprace z klubami sportowymi</button>
  <div class="panel">
  <ul>
          <li>Basic – 250 zł/mies   
    (wyniki meczowe,zapowiedzi meczy,informacje klubowe)</li>
          <li>Standard – 350 zł/mies
    (wyniki meczowe,zapowiedzi meczy,składy,*plakaty,dzień meczowy,informacje klubowe)</li>
          <li>Premium – 400 zł/mies
    (wyniki meczowe,zapowiedzi meczy,składy,*plakaty,dzień meczowy,informacje klubowe,animacje-video,wywiady-video)</li>
          <li>Pakiet + (animacje, wywiady, transmisje live, skróty meczów) - wycena indywidualna</li>
        </ul>
      </li>
    </ul>
  </div>
    
    
  <!-- Multimedia i animacje -->
  <button class="accordion-btn">Multimedia i animacje</button>
  <div class="panel">
    <ul>
      <li>Animowane reklamy i intro do filmów – 400–600 zł/szt</li>
      <li>Motion design – wycena indywidualna</li>
    </ul>
  </div>

  <!-- Projekty niestandardowe -->
  <button class="accordion-btn">Projekty niestandardowe</button>
  <div class="panel">
    <ul>
      <li>Infografiki do raportów, prezentacji, postów edukacyjnych – 200–400 zł/szt</li>
      <li>Grafiki do gier i aplikacji – wycena indywidualna</li>
    </ul>
  </div>
</section>

<!-- MEDIA -->
<section id="media" class="links">
  <h2>Media społecznościowe</h2>
  <a href="https://www.facebook.com/share/1HFEaFoNi3/" target="_blank">Facebook</a>
  <a href="https://www.instagram.com/14kapi" target="_blank">Instagram</a>
</section>

<!-- KONTAKT -->
<section id="contact" class="contact">
  <p>
    <a href="mailto:milcarzkacper65@gmail.com" style="color:white;text-decoration:none;font-size:1.1rem;">
      <i class="fa-solid fa-envelope"></i> milcarzkacper65@gmail.com
    </a>
  </p>
  <span id="scheduleBtn" onclick="openForm()">Umów się</span>
</section>


<footer>© 2026 Kacper Milcarz</footer>

<!-- MODALE -->
<div class="modal" id="imgModal" onclick="closeModal()">
  <img id="modalImg">
</div>

<div class="modal" id="formModal">
  <div class="form-box">
    <h2>Umów spotkanie</h2>
    <form id="meetingForm">
      <div class="input-box"><input type="text" placeholder="Imię i nazwisko" required></div>
      <div class="input-box"><input type="tel" placeholder="Numer telefonu" required></div>
      <div class="input-box">
        <select required>
          <option value="">Rodzaj współpracy</option>
          <option>Prowadzenie social mediów</option>
          <option>Grafiki firmowe</option>
          <option>Grafiki sportowe</option>
          <option>Strona internetowa</option>
        </select>
      </div>
      <button type="submit">Wyślij zgłoszenie</button>
    </form>
  </div>
</div>

<script>
function openModal(img){
  modalImg.src = img.src;
  imgModal.classList.add("active");
}
function closeModal(){
  imgModal.classList.remove("active");
  formModal.classList.remove("active");
}
function openForm(){
  formModal.classList.add("active");
}

// Formularz z komunikatem Gmail
meetingForm.addEventListener("submit", e=>{
  e.preventDefault();
  alert("Potwierdź zainteresowanie wysłaniem wiadomości na Gmail: milcarzkacper65@gmail.com");
  formModal.classList.remove("active");
});

// Funkcja do wyświetlania dodatkowych zdjęć po kliknięciu "Czytaj więcej"
function showMore(){
  document.getElementById("moreImages").style.display="grid";
}

// Accordion (cennik)
const acc = document.getElementsByClassName("accordion-btn");
for(let i=0;i<acc.length;i++){
  acc[i].addEventListener("click", function(){
    this.classList.toggle("active");
    const panel = this.nextElementSibling;
    if(panel.style.display === "block"){ panel.style.display = "none"; }
    else{ panel.style.display = "block"; }
  });
}
</script>
