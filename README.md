<html lang="id">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>SASTIK - Sanggar Seni Tiga Kendari</title>
  <meta name="description" content="Website resmi Sanggar Seni Tiga Kendari (SASTIK) – Sanggar seni tari tradisional dan modern dari Kendari." />
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">
  <style>
    :root{
      --merah-tua:#8B0000;
      --merah-cerah:#e63946;
      --emas:#FFD700;
      --putih:#fff;
      --hitam:#1a1a1a;
    }
    *{box-sizing:border-box;margin:0;padding:0;scroll-behavior:smooth;}
    body{font-family:Poppins,sans-serif;background:linear-gradient(180deg,var(--hitam),#330000);color:var(--putih);}
    header{position:sticky;top:0;background:rgba(139,0,0,0.9);backdrop-filter:blur(6px);padding:1rem 2rem;display:flex;align-items:center;justify-content:space-between;z-index:10;box-shadow:0 2px 10px rgba(0,0,0,0.4)}
    header h1{color:var(--emas);font-size:1.5rem;font-weight:700;}
    nav ul{display:flex;list-style:none;gap:1.5rem;}
    nav a{color:var(--putih);text-decoration:none;font-weight:500;transition:0.3s;}
    nav a:hover{color:var(--emas);}
    .hero{display:flex;flex-wrap:wrap;align-items:center;justify-content:space-between;padding:4rem 2rem;animation:fadeIn 2s ease-in;}
    .hero-text{flex:1;min-width:300px;}
    .hero-text h2{font-size:2.2rem;color:var(--emas);margin-bottom:1rem;}
    .hero-text p{max-width:550px;line-height:1.7;color:#fce8e8;}
    .hero-img{flex:1;min-width:300px;text-align:center;}
    .hero-img img{width:100%;max-width:400px;border-radius:12px;box-shadow:0 0 20px rgba(255,215,0,0.5);animation:float 4s ease-in-out infinite;}
    section{padding:3rem 2rem;}
    h2.section-title{text-align:center;color:var(--emas);margin-bottom:1rem;font-size:1.8rem;}
    p.section-sub{text-align:center;margin-bottom:2rem;color:#f8dcdc;}
    .profil,.tarian,.galeri,.kontak{max-width:1100px;margin:auto;}
    .profil-content{display:flex;flex-wrap:wrap;align-items:center;gap:2rem;}
    .profil-content img{width:100%;max-width:400px;border-radius:12px;box-shadow:0 0 15px rgba(255,255,255,0.2)}
    .profil-content div{flex:1;}
    .tarian-list{display:grid;grid-template-columns:repeat(auto-fit,minmax(220px,1fr));gap:1.5rem;}
    .tarian-card{background:rgba(255,255,255,0.05);border-radius:12px;padding:1rem;text-align:center;transition:transform 0.3s;}
    .tarian-card:hover{transform:scale(1.05);}
    .tarian-card img{width:100%;border-radius:10px;margin-bottom:.5rem;}
    .galeri-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(180px,1fr));gap:1rem;}
    .galeri-grid img{width:100%;border-radius:10px;transition:transform 0.3s,box-shadow 0.3s;}
    .galeri-grid img:hover{transform:scale(1.05);box-shadow:0 0 15px var(--emas);}
    .kontak-form{display:flex;flex-direction:column;gap:1rem;max-width:600px;margin:auto;}
    input,textarea{padding:.8rem;border:none;border-radius:8px;background:rgba(255,255,255,0.1);color:var(--putih);}
    button{padding:.8rem 1.5rem;background:var(--emas);color:var(--hitam);border:none;border-radius:8px;font-weight:600;cursor:pointer;transition:0.3s;}
    button:hover{background:var(--merah-cerah);color:var(--putih);}
    footer{text-align:center;padding:1.5rem;background:rgba(0,0,0,0.8);color:#ddd;margin-top:2rem;font-size:.9rem;}
    @keyframes fadeIn{from{opacity:0;transform:translateY(20px);}to{opacity:1;transform:translateY(0);}}
    @keyframes float{0%{transform:translateY(0);}50%{transform:translateY(-10px);}100%{transform:translateY(0);}}
    /* 🎭 ANIMASI TAMBAHAN UNTUK GAMBAR */
    @keyframes fadeInUp {
      from {opacity: 0; transform: translateY(30px);}
      to {opacity: 1; transform: translateY(0);}
    }
    img.animate {
      opacity: 0;
      transform: translateY(30px);
      transition: all 1s ease;
    }
    img.animate.show {
      opacity: 1;
      transform: translateY(0);
      animation: fadeInUp 1.2s ease forwards;
    }
    img:hover {
      transform: scale(1.07);
      box-shadow: 0 0 20px gold;
    }
  
  /* Gaya Wrapper Carousel */
.carousel-wrapper {
    position: relative;
    max-width: 1000px; /* Atur lebar maksimal */
    margin: 40px auto;
    overflow: hidden; /* Penting untuk menyembunyikan slide yang tidak aktif */
    border-radius: 15px;
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
}

/* Sembunyikan Input Radio */
.carousel-wrapper input[type="radio"] {
    display: none;
}

/* Kontainer yang akan bergeser */
.carousel-container {
    display: flex; /* Membuat slide berbaris horizontal */
    width: 300%; /* 3 slide * 100% = 300% */
    transition: transform 0.6s ease-in-out; /* Animasi pergeseran */
}

/* Gaya per Slide */
.slide {
    width: 99.99%; /* 100% / 3 slide */
    height: 400px;
    position: relative;
}

.slide img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    display: block;
}

/* Caption Teks */
.caption {
    position: absolute;
    bottom: 20px;
    left: 20px;
    color: white;
    font-size: 1.5rem;
    font-weight: bold;
    text-shadow: 0 0 5px rgba(0, 0, 0, 0.7);
}

/* Logic Pergeseran Slide (INTI) */
/* Ketika slide-2 aktif, geser kontainer ke kiri 33.33% */
#slide-2:checked ~ .carousel-container {
    transform: translateX(-33.33%);
}

/* Ketika slide-3 aktif, geser kontainer ke kiri 66.66% */
#slide-3:checked ~ .carousel-container {
    transform: translateX(-66.66%);
}

#slide-4:checked ~ .carousel-container {
    transform: translateX(-99.99%);
}
  
/* Gaya Navigasi Dots */
.navigation-dots {
    position: absolute;
    bottom: 10px;
    left: 50%;
    transform: translateX(-50%);
    display: flex;
    gap: 10px;
}

.dot {
    cursor: pointer;
    height: 12px;
    width: 12px;
    background-color: #bbb;
    border-radius: 50%;
    display: block;
    transition: background-color 0.3s;
}
/* Gaya Dot yang Aktif */
#slide-1:checked ~ .navigation-dots .dot:nth-child(1),
#slide-2:checked ~ .navigation-dots .dot:nth-child(2),
#slide-3:checked ~ .navigation-dots .dot:nth-child(3),
#slide-4:checked ~ .navigation-dots .dot:nth-child(4){
    background-color: #fff;
    border: 2px solid #333;
}

.logo-box {
  display: flex;
  align-items: center;
  justify-content: center;
  margin-right: 10px;
}

.logo {
  width: 60px;
  height: 60px;
  border-radius: 50%;
  animation: logoPulse 3s infinite ease-in-out;
  box-shadow: 0 0 15px rgba(255,255,255,0.3);
}

/* Animasi lembut berdenyut */
@keyframes logoPulse {
  0% { transform: scale(1); box-shadow: 0 0 10px rgba(255,255,255,0.3); }
  50% { transform: scale(1.1); box-shadow: 0 0 20px gold; }
  100% { transform: scale(1); box-shadow: 0 0 10px rgba(255,255,255,0.3); }
}

/* ✨ Animasi teks di header (judul dan menu) */
header h1, nav a {
  position: relative;
  animation: fadeText 2s ease forwards;
  opacity: 0;
}

/* Urutan animasi untuk menu satu per satu */
nav a:nth-child(1) { animation-delay: 0.3s; }
nav a:nth-child(2) { animation-delay: 0.6s; }
nav a:nth-child(3) { animation-delay: 0.9s; }
nav a:nth-child(4) { animation-delay: 1.2s; }

/* Efek berkilau halus saat hover */
nav a::after {
  content: '';
  position: absolute;
  left: 0;
  bottom: -3px;
  width: 0%;
  height: 2px;
  background: gold;
  transition: width 0.4s ease;
}

nav a:hover::after {
  width: 100%;
}

/* Animasi masuk perlahan dari atas */
@keyframes fadeText {
  from {
    transform: translateY(-15px);
    opacity: 0;
  }
  to {
    transform: translateY(0);
    opacity: 1;
  }
}
</style>
</head>
<body>
  <header>
  <div class="logo-box">
    <img src="logo-sastik.jpg" alt="Logo SASTIK" class="logo animate-logo">
  </div>
  <h1>SASTIK</h1>
  <nav>
      <ul>
        <li><a href="#beranda">Beranda</a></li>
        <li><a href="#profil">Profil</a></li>
        <li><a href="#tarian">Tarian</a></li>
        <li><a href="#galeri">Galeri</a></li>
      </ul>
    </nav>
  </header>
  <section id="beranda" class="hero">
    <div class="hero-text">
      <h2>Sanggar Seni Tiga Kendari (SASTIK)</h2>
      <p>Tempat kami menyalurkan cinta terhadap budaya dan tarian tradisional. Di SASTIK, menari bukan sekadar gerak, tetapi juga wujud rasa, makna, dan kebersamaan keluarga seni.</p>
    </div>
    <div class="tarian-card">
      <img src="IMG-satu.jpg" alt="Penari tradisional SASTIK" class="animate">
    </div>
  </section>

  <section id="profil" class="profil">
    <h2 class="section-title">Profil Sanggar</h2>
    <p class="section-sub">Menjaga dan melestarikan seni tari tradisional Kendari</p>
    <div class="profil-content">
      <img src="IMG-tiga.jpg" alt="Latihan tari di sanggar" class="animate">
      <div>
        <p>SASTIK (Sanggar Seni Tiga Kendari) didirikan dengan semangat untuk melestarikan budaya lokal melalui tari. Kami adalah keluarga besar penari muda yang berlatih, tampil, dan berbagi kebahagiaan lewat gerak dan irama.</p>
        <p>Dengan pelatih berpengalaman dan anggota yang solid, kami telah tampil di berbagai acara budaya dan festival daerah. Kami percaya bahwa setiap gerakan memiliki cerita dan setiap tarian adalah warisan.</p>
      </div>
    </div>
  </section>

  <section id="tarian" class="tarian">
    <h2 class="section-title">Tarian Kami</h2>
    <p class="section-sub">Karya tari yang pernah kami tampilkan</p>
    <div class="tarian-list">
      <div class="tarian-card">
        <img src="IMG-parang.jpg" alt="Tari Haluoleo" class="animate">
        <h3>Haluoleo</h3>
        <p>Tari penyambutan khas Sulawesi Tenggara yang menggambarkan kehangatan dan persaudaraan.</p>
      </div>
      <div class="tarian-card">
        <img src="IMG-tameng.jpg" alt="Tari Amoara" class="animate">
        <h3>Amoara & mondotambe</h3>
        <p>Tarian kebanggaan SASTIK yang memadukan energi muda dan tradisi daerah dengan gaya elegan.</p>
      </div>
      <div class="tarian-card">
        <img src="IMG-toraja.jpg" alt="Tari 4 etnis" class="animate">
        <h3>4 etnis</h3>
        <p>Tari 4 Etnis adalah tarian kreasi yang berasal dari Sulawesi Selatan yang memadukan unsur-unsur dari empat etnis terbesar di wilayah tersebut: Bugis, Makassar, Mandar, dan Toraja..</p>
      </div>
      <div class="tarian-card">
        <img src="IMG-paduppa.jpg" alt="paduppa" class="animate">
        <h3>paduppa</h3>
        <p>Tari Paduppa adalah tarian tradisional dari suku Bugis-Makassar yang berfungsi sebagai tarian penyambutan tamu, sering disebut sebagai tarian selamat datang</p>
      </div>
    </div>
  </section>
  <div class="carousel-wrapper">
    <input type="radio" name="slider" id="slide-1" checked>
    <input type="radio" name="slider" id="slide-2">
    <input type="radio" name="slider" id="slide-3">
    <input type="radio" name="slider" id="slide-4">
    <div class="carousel-container">
        <div class="slide" id="s1">
            <img src="hitam.JPG" alt="Slide 1 - Hutan">
            <div class="caption">SASTIK</div>
        </div>
        <div class="slide" id="s2">
            <img src="IMG-merah.jpg" alt="Slide 2 - Pegunungan">
            <div class="caption">SASTIK</div>
        </div>
        <div class="slide" id="s3">
            <img src="IMG-luloo5.jpg" alt="Slide 3 - Gurun">
            <div class="caption">SASTIK</div>
        </div>
    </div>    
    <div class="slide" id="s4">
      <img src="IMG-sisi.jpg" alt="Slide 4 - sisii">
      <div class="caption">SASTIK</div>
    </div>
    <div class="navigation-dots">
        <label for="slide-1" class="dot"></label>
        <label for="slide-2" class="dot"></label>
        <label for="slide-3" class="dot"></label>
        <label for="slide-4" class="dot"></label>
    </div>
</div>

<section id="video" class="video">
  <h2 class="section-title">Nonton Video Kami</h2>
  <p class="section-sub">Saksikan penampilan tarian kami secara langsung</p>
  <div class="video-grid" style="display:flex;justify-content:center;flex-wrap:wrap;gap:2rem;">
    <div style="flex:1;min-width:300px;max-width:372px;cursor:pointer;">
      <img src="IMG-video.png" alt="Video Tari SASTIK" 
           style="width:100%;border-radius:12px;box-shadow:0 0 15px rgba(255,215,0,0.5);transition:0.3s;" 
           onclick="tontonVideo('5cQ68zCqpKw')">
      <p class="section-sub">tarian 4 etnis sulawesi selatan yang di bawakan oleh smk n 3 kendari</p>
    </div>
  </div>
</section>

<div class="video-grid" style="display:flex;justify-content:center;flex-wrap:wrap;gap:2rem;">
    <div style="flex:1;min-width:300px;max-width:372px;cursor:pointer;">
      <img src="IMG-video.png" alt="Video Tari SASTIK" 
           style="width:100%;border-radius:12px;box-shadow:0 0 15px rgba(255,215,0,0.5);transition:0.3s;" 
           onclick="tontonVideo('5cQ68zCqpKw')">
      <p class="section-sub">tarian haluoleo yang di bawakan oleh smk n 3 kendari</p>
    </div>
  </div>
</section>

  <div class="video-grid" style="display:flex;justify-content:center;flex-wrap:wrap;gap:2rem;">
    <div style="flex:1;min-width:300px;max-width:372px;cursor:pointer;">
      <img src="IMG-video.png" alt="Video Tari SASTIK" 
           style="width:100%;border-radius:12px;box-shadow:0 0 15px rgba(255,215,0,0.5);transition:0.3s;" 
           onclick="tontonVideo('5cQ68zCqpKw')">
      <p class="section-sub">tarian lulo tapis yang di bawakan oleh smk n 3 kendari</p>
    </div>
  </div>
  
<script>
  function tontonVideo(id){
    const popup = document.createElement('div');
    popup.style.position = 'fixed';
    popup.style.top = 0;
    popup.style.left = 0;
    popup.style.width = '100%';
    popup.style.height = '100%';
    popup.style.background = 'rgba(0,0,0,0.9)';
    popup.style.display = 'flex';
    popup.style.alignItems = 'center';
    popup.style.justifyContent = 'center';
    popup.style.zIndex = 9999;  
    popup.style.cursor = 'pointer';
    popup.innerHTML = `<iframe width="90%" height="80%" src="https://www.youtube.com/embed/${id}?autoplay=1" 
      frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>`;
    popup.addEventListener('click', (e)=>{
      if(e.target === popup) popup.remove();  
    });
    document.body.appendChild(popup);
  }
</script>
  
  <section id="galeri" class="galeri">
    <h2 class="section-title">Galeri</h2>
    <p class="section-sub">Potret kebersamaan dan penampilan kami</p>
    <div class="galeri-grid">
      <img src="IMG-ulta.jpg" alt="Penampilan tari" class="animate">
      <img src="IMG-toraja.jpg" alt="Latihan tari" class="animate">
      <img src="IMG-satu.jpg" alt="Kostum tari" class="animate">
      <img src="IMG-tiga.jpg" alt="Pertunjukan panggung" class="animate">
      <img src="IMG-sisi.jpg" alt="sisi andriani" class="animate">
      <img src="IMG-hotel.jpg" alt="sastik" class="animate">
    </div>
  </section>

  <footer>
    <p>© 2025 SASTIK - Sanggar Seni Tiga Kendari.</p>
  </footer>

  <script>
    function kirimPesan(e){
      e.preventDefault();
      const nama=document.getElementById('nama').value;
      alert('Terima kasih '+nama+'! Pesan kamu sudah terkirim ke SASTIK.');
      e.target.reset();
    }

    // 🔸 Efek animasi saat discroll
    const animElements = document.querySelectorAll('img.animate');
    function animOnScroll(){
      animElements.forEach(el=>{
        const rect = el.getBoundingClientRect();
        if(rect.top < window.innerHeight - 100){
          el.classList.add('show');
        }
      });
    }
    window.addEventListener('scroll', animOnScroll);
    animOnScroll();
  </script>
  
  <canvas id="bintang"></canvas>
<script>
const canvas=document.getElementById('bintang');
const ctx=canvas.getContext('2d');
canvas.width=innerWidth;canvas.height=innerHeight;
const stars=[];
for(let i=0;i<100;i++){stars.push({x:Math.random()*innerWidth,y:Math.random()*innerHeight,r:Math.random()*1.5});}
function draw(){
  ctx.clearRect(0,0,canvas.width,canvas.height);
  ctx.fillStyle='white';
  stars.forEach(s=>{
    ctx.beginPath();
    ctx.arc(s.x,s.y,s.r,0,Math.PI*2);
    ctx.fill();
  });
}
function update(){
  stars.forEach(s=>{
    s.y+=0.2;
    if(s.y>innerHeight){s.y=0;s.x=Math.random()*innerWidth;}
  });
}
function animate(){draw();update();requestAnimationFrame(animate);}
animate();
</script>
  
  <script>
const imgs=document.querySelectorAll('.galeri-grid img');
imgs.forEach(img=>{
  img.addEventListener('click',()=>{
    const popup=document.createElement('div');
    popup.style.position='fixed';
    popup.style.top='0';popup.style.left='0';
    popup.style.width='100%';popup.style.height='100%';
    popup.style.background='rgba(0,0,0,0.9)';
    popup.style.display='flex';popup.style.alignItems='center';popup.style.justifyContent='center';
    popup.innerHTML=`<img src="${img.src}" style="max-width:90%;max-height:90%;border-radius:10px;">`;
    popup.onclick=()=>popup.remove();
    document.body.appendChild(popup);
  });
});
</script>
</body>
</html>
