
<html lang="id">
<head>
  <meta charset="utf-8" />
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>SASTIK - Sanggar Seni Tiga Kendari</title>
  <meta name="description" content="Website resmi Sanggar Seni Tiga Kendari (SASTIK) – Sanggar seni tari tradisional dan modern dari Kendari." />
  <meta name="generator" content="Jekyll v3.10.0" />
  <meta property="og:title" content="sastik" />
  <meta property="og:locale" content="en_US" />
  <meta property="og:description" content="website" />
  <meta property="og:url" content="https://assikraa-ops.github.io/sastik/" />
  <meta property="og:site_name" content="sastik" />
  <meta property="og:type" content="website" />
  <meta name="twitter:card" content="summary" />
  <meta property="twitter:title" content="sastik" />
  <link rel="canonical" href="https://assikraa-ops.github.io/sastik/" />
  <script type="application/ld+json">
    {"@context":"https://schema.org","@type":"WebSite","description":"website","headline":"sastik","name":"sastik","url":"https://assikraa-ops.github.io/sastik/"}
  </script>

  <!-- jika punya file css eksternal tetap bisa dipakai -->
  <link rel="stylesheet" href="/sastik/assets/css/style.css?v=a9c3450857110ad44de46de247294a3e4e4d0113">

  <!-- ====== Style internal (dari kode awal) ====== -->
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
    @keyframes fadeIn{from{opacity:0;transform:translateY(20px);}to{opacity:1;transform:translateY(0);} }
    @keyframes float{0%{transform:translateY(0);}50%{transform:translateY(-10px);}100%{transform:translateY(0);} }
    @keyframes fadeInUp {from {opacity: 0; transform: translateY(30px);} to {opacity: 1; transform: translateY(0);} }
    img.animate {opacity: 0; transform: translateY(30px); transition: all 1s ease;}
    img.animate.show {opacity: 1; transform: translateY(0); animation: fadeInUp 1.2s ease forwards;}
    img:hover {transform: scale(1.07); box-shadow: 0 0 20px gold;}
    .carousel-wrapper {position: relative; max-width: 1000px; margin: 40px auto; overflow: hidden; border-radius: 15px; box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2); }

    /* Sembunyikan input radio dengan cara yang aman (tidak menampilkan teks HTML di halaman) */
    .carousel-wrapper input[type="radio"] { position: absolute; left: -9999px; }

    .carousel-container {display: flex; width: 400%; transition: transform 0.6s ease-in-out; }
    .slide { width: 25%; height: 400px; position: relative; }
    .slide img { width: 100%; height: 100%; object-fit: cover; display: block; }
    .caption { position: absolute; bottom: 20px; left: 20px; color: white; font-size: 1.5rem; font-weight: bold; text-shadow: 0 0 5px rgba(0, 0, 0, 0.7); }

    /* Logic Pergeseran Slide (menggeser berdasarkan radio yang dipilih) */
    #slide-1:checked ~ .carousel-container { transform: translateX(0%); }
    #slide-2:checked ~ .carousel-container { transform: translateX(-25%); }
    #slide-3:checked ~ .carousel-container { transform: translateX(-50%); }
    #slide-4:checked ~ .carousel-container { transform: translateX(-75%); }

    /* Gaya Navigasi Dots */
    .navigation-dots { position: absolute; bottom: 10px; left: 50%; transform: translateX(-50%); display: flex; gap: 10px; }
    .dot { cursor: pointer; height: 12px; width: 12px; background-color: #E57373; border-radius: 50%; display: block; transition: background-color 0.3s; }

    /* Menandai dot aktif sesuai radio yang terpilih */
    #slide-1:checked ~ .navigation-dots .dot:nth-child(1),
    #slide-2:checked ~ .navigation-dots .dot:nth-child(2),
    #slide-3:checked ~ .navigation-dots .dot:nth-child(3),
    #slide-4:checked ~ .navigation-dots .dot:nth-child(4) {
      background-color: white; border: 2px solid #D32F2F;
    }

    .logo { width: 60px; height: 60px; border-radius: 50%; animation: logoPulse 3s infinite ease-in-out; box-shadow: 0 0 15px rgba(255,255,255,0.3); }
    @keyframes logoPulse { 0% { transform: scale(1); box-shadow: 0 0 10px rgba(255,255,255,0.3); } 50% { transform: scale(1.1); box-shadow: 0 0 20px gold; } 100% { transform: scale(1); box-shadow: 0 0 10px rgba(255,255,255,0.3); } }
    header h1, nav a { position: relative; animation: fadeText 2s ease forwards; opacity: 0; }
    nav a:nth-child(1) { animation-delay: 0.3s; } nav a:nth-child(2) { animation-delay: 0.6s; } nav a:nth-child(3) { animation-delay: 0.9s; } nav a:nth-child(4) { animation-delay: 1.2s; }
    nav a::after { content: ''; position: absolute; left: 0; bottom: -3px; width: 0%; height: 2px; background: gold; transition: width 0.4s ease; }
    nav a:hover::after { width: 100%; }
    @keyframes fadeText { from { transform: translateY(-15px); opacity: 0; } to { transform: translateY(0); opacity: 1; } }

@keyframes putar3D {
  0% { transform: rotateY(0deg); }
  100% { transform: rotateY(360deg); }
}


  </style>
</head>
<body>
  <div class="container-lg px-3 my-5 markdown-body">

    <header>
      <div class="logo-box">
        <img src="logo-sastik.jpg" alt="Logo SASTIK" class="logo animate-logo" />
<p>logo-sastik.jpg</p>
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
        <img src="IMG-satu.jpg" alt="Penari tradisional SASTIK" class="animate" />
<p>IMG-satu.jpg</p>
      </div>
    </section>

    <section id="profil" class="profil">
      <h2 class="section-title">Profil Sanggar</h2>
      <p class="section-sub">Menjaga dan melestarikan seni tari tradisional Kendari</p>
      <div class="profil-content">
        <img src="IMG-tiga.jpg" alt="Latihan tari di sanggar" class="animate" />
<p>IMG-tiga.jpg</p>
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
          <img src="sedow.png" alt="Tari Haluoleo" class="animate" />
<p>sedow.png</p>
          <h3>Haluoleo</h3>
          <p>Tari penyambutan khas Sulawesi Tenggara yang menggambarkan kehangatan dan persaudaraan.</p>
        </div>
        <div class="tarian-card">
          <img src="IMG-tameng.jpg" alt="Tari Amoara" class="animate" />
<p>IMG-tameng.jpg</p>
          <h3>Amoara &amp; mondotambe</h3>
          <p>Tarian kebanggaan SASTIK yang memadukan energi muda dan tradisi daerah dengan gaya elegan.</p>
        </div>
        <div class="tarian-card">
          <img src="IMG-toraja.jpg" alt="Tari 4 etnis" class="animate" />
<p>IMG-toraja.jpg</p>
          <h3>4 etnis</h3>
          <p>Tari 4 Etnis adalah tarian kreasi yang berasal dari Sulawesi Selatan yang memadukan unsur-unsur dari empat etnis terbesar di wilayah tersebut: Bugis, Makassar, Mandar, dan Toraja.</p>
        </div>
        <div class="tarian-card">
          <img src="IMG-paduppa.jpg" alt="paduppa" class="animate" />
<p>IMG-paduppa.jpg</p>
          <h3>paduppa</h3>
          <p>Tari Paduppa adalah tarian tradisional dari suku Bugis-Makassar yang berfungsi sebagai tarian penyambutan tamu.</p>
        </div>
      </div>
    </section>

    <!-- Struktur Organisasi -->
    <section id="struktur" class="struktur">
      <h2 class="section-title">Struktur Organisasi</h2>
      <p class="section-sub">Struktur kepengurusan Sanggar Seni Tiga Kendari</p>
      <div class="profil-content" style="flex-direction:column;text-align:center;gap:1.5rem;">
        <div><strong>Pembina:</strong>WAHYU CAESAR.R</div>
        <div><strong>Pelatih:</strong>ARDI</div>
        <div><strong>Ketua:</strong>SRI</div>
        <div><strong>Wakil Ketua:</strong>GEDE FAJAR JULIANA</div>
        <div><strong>Sekretaris:</strong>ARIFIN</div>
        <div><strong>Bendahara:</strong>KAK INTAN</div>
      </div>
    </section>

    <!-- Carousel: input radio harus jadi sibling langsung dari container (telah diperbaiki) -->
    <div class="carousel-wrapper">
      <!-- radio harus berada di dalam wrapper dan menjadi sibling langsung dari .carousel-container dan .navigation-dots -->
      <input type="radio" name="slider" id="slide-1" checked />
      <input type="radio" name="slider" id="slide-2" />
      <input type="radio" name="slider" id="slide-3" />
      <input type="radio" name="slider" id="slide-4" />

      <div class="carousel-container">
        <div class="slide" id="s1">
          <img src="hitam.jpg" alt="Slide 1 - Tarian Tradisional" />
<p>hitam.jpg</p>
          <div class="caption">SASTIK</div>
        </div>
        <div class="slide" id="s2">
          <img src="IMG-luloo5.jpg" alt="Slide 2 - Penari SASTIK" />
<p>IMG-luloo5.jpg</p>
          <div class="caption">SASTIK</div>
        </div>
        <div class="slide" id="s3">
          <img src="IMG-merah.jpg" alt="Slide 3 - Panggung Pertunjukan" />
<p>IMG-merah.jpg</p>
          <div class="caption">SASTIK</div>
        </div>
        <div class="slide" id="s4">
          <img src="IMG-sisi.jpg" alt="Slide 4 - Latihan Bersama" />
<p>IMG-sisi.jpg</p>
          <div class="caption">SASTIK</div>
        </div>
      </div>

      <div class="navigation-dots">
        <label for="slide-1" class="dot" aria-label="Slide 1"></label>
        <label for="slide-2" class="dot" aria-label="Slide 2"></label>
        <label for="slide-3" class="dot" aria-label="Slide 3"></label>
        <label for="slide-4" class="dot" aria-label="Slide 4"></label>
      </div>
    </div>

    <section id="video" class="video">
      <h2 class="section-title">Nonton Video Kami</h2>
      <p class="section-sub">Saksikan penampilan tarian kami secara langsung</p>
      <div class="video-grid" style="display:flex;justify-content:center;flex-wrap:wrap;gap:2rem;">
        <div style="flex:1;min-width:300px;max-width:372px;cursor:pointer;">
          <img src="IMG-video.png" alt="Video Tari SASTIK" style="width:100%;border-radius:12px;box-shadow:0 0 15px rgba(255,215,0,0.5);transition:0.3s;" onclick="tontonVideo('5cQ68zCqpKw')" />
<p>IMG-video.png</p>
          <p class="section-sub">tarian 4 etnis sulawesi selatan yang di bawakan oleh smk n 3 kendari</p>
        </div>
      </div>

      <div class="video-grid" style="display:flex;justify-content:center;flex-wrap:wrap;gap:2rem;">
        <div style="flex:1;min-width:300px;max-width:373px;cursor:pointer;">
          <img src="IMG-video.png" alt="Video Tari SASTIK" style="width:100%;border-radius:12px;box-shadow:0 0 15px rgba(255,215,0,0.5);transition:0.3s;" onclick="tontonVideo('5cQ68zCqpKw')" />
<p>IMG-video.png</p>
          <p class="section-sub">tarian haluoleo yang di bawakan oleh smk n 3 kendari</p>
        </div>
      </div>

      <div class="video-grid" style="display:flex;justify-content:center;flex-wrap:wrap;gap:2rem;">
        <div style="flex:1;min-width:300px;max-width:373px;cursor:pointer;">
          <img src="IMG-video.png" alt="Video Tari SASTIK" style="width:100%;border-radius:12px;box-shadow:0 0 15px rgba(255,215,0,0.5);transition:0.3s;" onclick="tontonVideo('5cQ68zCqpKw')" />
<p>IMG-video.png</p>
          <p class="section-sub">tarian lulo tapis yang di bawakan oleh smk n 3 kendari</p>
        </div>
      </div>
    </section>

    <section id="galeri" class="galeri">
      <h2 class="section-title">Galeri</h2>
      <p class="section-sub">Potret kebersamaan dan penampilan kami</p>
      <div class="galeri-grid">
        <img src="IMG-ulta.jpg" alt="Penampilan tari" class="animate" />
<p>IMG-ulta.jpg</p>
        <img src="IMG-toraja.jpg" alt="Latihan tari" class="animate" />
<p>IMG-toraja.jpg</p>
        <img src="IMG-satu.jpg" alt="Kostum tari" class="animate" />
<p>IMG-satu.jpg</p>
        <img src="IMG-tiga.jpg" alt="Pertunjukan panggung" class="animate" />
<p>IMG-tiga.jpg</p>
        <img src="IMG-sisi.jpg" alt="sisi andriani" class="animate" />
<p>IMG-sisi.jpg</p>
        <img src="IMG-hotel.jpg" alt="sastik" class="animate" />
<p>IMG-hotel.jpg</p>
      </div>
    </section>

<!-- Logo 3D di bawah galeri -->
<section id="logo-3d" style="text-align:center; padding:3rem 0;">
  <h2 class="section-title">Logo 3D SASTIK</h2>
  <p class="section-sub">SASTIK</p>

  <div style="
    display: inline-block;
    padding: 20px;
    background: rgba(255,255,255,0.05);
    border-radius: 20px;
    box-shadow: 
      0 10px 25px rgba(0,0,0,0.5),
      inset 0 0 20px rgba(255,215,0,0.2);
    transform-style: preserve-3d;
    animation: putar3D 8s infinite linear;
  ">
    <img src="logo-sastik.jpg" alt="Logo 3D SASTIK" style="
      width: 200px;
      height: 200px;
      border-radius: 50%;
      box-shadow:
        0 0 20px rgba(255,215,0,0.7),
        inset 0 0 15px rgba(255,255,255,0.5);
      transform: translateZ(30px);
    ">
  </div>
</section>

    <footer>
      <p>© 2025 SASTIK - Sanggar Seni Tiga Kendari.</p>
    </footer>

  </div>

  <!-- SCRIPTS -->
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
      popup.innerHTML = <iframe width="90%" height="80%" src="https://www.youtube.com/embed/${id}?autoplay=1" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>;
      popup.addEventListener('click', (e)=>{
        if(e.target === popup) popup.remove();
      });
      document.body.appendChild(popup);
    }

    // efek anim saat discroll
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

    // popup galeri
    const imgs = document.querySelectorAll('.galeri-grid img');
    imgs.forEach(img=>{
      img.addEventListener('click',()=>{
        const popup=document.createElement('div');
        popup.style.position='fixed';
        popup.style.top='0';popup.style.left='0';
        popup.style.width='100%';popup.style.height='100%';
        popup.style.background='rgba(0,0,0,0.9)';
        popup.style.display='flex';popup.style.alignItems='center';popup.style.justifyContent='center';
        popup.innerHTML=`<img src="${img.src}" style="max-width:90%;max-height:90%;border-radius:10px;">
<p>${img.src}</p>`;
        popup.onclick=()=>popup.remove();
        document.body.appendChild(popup);
      });
    });

    // canvas bintang
    (function(){
      const canvas=document.createElement('canvas');
      canvas.id='bintang';
      document.body.appendChild(canvas);
      const ctx=canvas.getContext('2d');
      function resize(){ canvas.width=innerWidth; canvas.height=innerHeight; }
      window.addEventListener('resize', resize); resize();
      const stars=[];
      for(let i=0;i<100;i++){ stars.push({x:Math.random()*innerWidth,y:Math.random()*innerHeight,r:Math.random()*1.5});}
      function draw(){ ctx.clearRect(0,0,canvas.width,canvas.height); ctx.fillStyle='white'; stars.forEach(s=>{ ctx.beginPath(); ctx.arc(s.x,s.y,s.r,0,Math.PI*2); ctx.fill(); }); }
      function update(){ stars.forEach(s=>{ s.y+=0.2; if(s.y>innerHeight){s.y=0;s.x=Math.random()*innerWidth;} }); }
      function animate(){ draw(); update(); requestAnimationFrame(animate); }
      animate();
    })();
  </script>

  <!-- Anchor.js (kalau perlu) -->
  <script src="https://cdnjs.cloudflare.com/ajax/libs/anchor-js/4.1.0/anchor.min.js" integrity="sha256-lZaRhKri35AyJSypXXs4o6OPFTbTmUoltBbDCbdzegg=" crossorigin="anonymous"></script>
  <script> if(window.anchors) anchors.add(); </script>
</b
          
