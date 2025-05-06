# landing-
<!DOCTYPE html>
<html lang="sr">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Prozornica - Kreativni Edukativni Centar</title>
  <link href="https://fonts.googleapis.com/css2?family=Baloo+2&family=Quicksand&display=swap" rel="stylesheet">
  <style>
    body {
      margin: 0;
      font-family: 'Quicksand', sans-serif;
      background-color: #fff8f2;
      color: #333;
    }

    header {
      background-color: #f26522;
      color: white;
      text-align: center;
      padding: 2rem 1rem;
    }

    header h1 {
      font-family: 'Baloo 2', cursive;
      font-size: 3rem;
      margin-bottom: 0.5rem;
    }

    header p {
      font-size: 1.2rem;
    }

    section {
      padding: 2rem;
      max-width: 1200px;
      margin: auto;
    }

    h2 {
      text-align: center;
      color: #f26522;
      margin-bottom: 1rem;
    }

    .program-cards {
      display: flex;
      flex-wrap: wrap;
      gap: 2rem;
      justify-content: center;
    }

    .program-card {
      background-color: #fff;
      border-radius: 16px;
      box-shadow: 0 4px 20px rgba(0, 0, 0, 0.1);
      padding: 1.5rem;
      width: 280px;
      text-align: center;
      transition: transform 0.3s ease-in-out;
    }

    .program-card:hover {
      transform: translateY(-10px);
    }

    .program-card img {
      width: 100%;
      border-radius: 12px;
      cursor: pointer;
    }

    .program-card h3 {
      margin-top: 1rem;
      color: #f26522;
    }

    .program-card p {
      font-size: 1rem;
    }

    .lightbox {
      display: none;
      position: fixed;
      z-index: 999;
      left: 0; top: 0;
      width: 100%;
      height: 100%;
      background: rgba(0,0,0,0.8);
      align-items: center;
      justify-content: center;
    }

    .lightbox img {
      max-width: 90%;
      max-height: 90%;
      border-radius: 10px;
    }

    .cta {
      text-align: center;
      margin-top: 3rem;
    }

    .cta a {
      background: #f26522;
      color: #fff;
      padding: 1rem 2rem;
      border-radius: 8px;
      text-decoration: none;
      font-size: 1.2rem;
    }
  </style>
</head>
<body>

<header>
  <h1>Prozornica</h1>
  <p>Kreativni edukativni centar za decu uzrasta od 4 do 14 godina</p>
</header>

<section>
  <h2>Naša misija</h2>
  <p>
    Edukativni centar „Prozornica” je mesto gde se znanje i igra sreću. Naša misija je da deci pružimo bezbedno, inspirativno i podsticajno okruženje za učenje i razvoj kroz pažljivo osmišljene radionice koje obuhvataju različite oblasti – od jezika, preko umetnosti i govora, do emocionalnog razvoja.
  </p>
</section>

<section>
  <h2>Radionice koje nudimo</h2>
  <div class="program-cards">
    <div class="program-card">
      <img src="https://i.imgur.com/Hiv5xOG.jpeg" alt="Pisanje sastava" onclick="openLightbox(this.src)">
      <h3>Pisanje sastava</h3>
      <p>Razvijamo maštu i izražavanje kroz pisanje pismenih zadataka i sastava na kreativne i zanimljive teme.</p>
    </div>
    <div class="program-card">
      <img src="https://i.imgur.com/N9xea54.jpeg" alt="Logopedske radionice" onclick="openLightbox(this.src)">
      <h3>Logopedske radionice</h3>
      <p>U saradnji sa stručnjacima radimo na poboljšanju izgovora, razumevanja i govorne komunikacije kod dece.</p>
    </div>
    <div class="program-card">
      <img src="https://i.imgur.com/jcp2lwL.jpeg" alt="Lutkarsko pozorište" onclick="openLightbox(this.src)">
      <h3>Lutkarsko pozorište</h3>
      <p>Umetnost izražavanja kroz igru lutkama razvija emocionalnu inteligenciju, empatiju i samopouzdanje.</p>
    </div>
    <div class="program-card">
      <img src="https://i.imgur.com/wrwfhcC.jpeg" alt="Relax Kids" onclick="openLightbox(this.src)">
      <h3>Relax Kids</h3>
      <p>Metod zasnovan na igri, disanju i meditaciji pomaže deci da se opuste, povežu sa sobom i drugima.</p>
    </div>
    <div class="program-card">
      <img src="https://i.imgur.com/O0dwDKb.jpeg" alt="Ekološke radionice" onclick="openLightbox(this.src)">
      <h3>Ekološke radionice</h3>
      <p>Učimo o važnosti očuvanja prirode kroz praktične radionice, sadnju, reciklažu i eksperimente u prirodi.</p>
    </div>
    <div class="program-card">
      <img src="https://i.imgur.com/a47hYio.jpeg" alt="Engleski jezik" onclick="openLightbox(this.src)">
      <h3>Engleski jezik</h3>
      <p>Kroz pesme, igru i pokret učimo osnove engleskog jezika prilagođene uzrastu deteta.</p>
    </div>
  </div>
</section>

<section class="cta">
  <h2>Pridružite nam se!</h2>
  <p>Zakoračite u svet mašte, znanja i radoznalosti. Prijavite svoje dete već danas!</p>
  <a href="#kontakt">Prijavi se</a>
</section>

<div class="lightbox" onclick="closeLightbox()">
  <img id="lightbox-img" src="" alt="Uvećana slika">
</div>

<script>
  function openLightbox(src) {
    document.getElementById('lightbox-img').src = src;
    document.querySelector('.lightbox').style.display = 'flex';
  }

  function closeLightbox() {
    document.querySelector('.lightbox').style.display = 'none';
  }
</script>

</body>
</html>
