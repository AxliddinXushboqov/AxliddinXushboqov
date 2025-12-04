<div align="center" style="margin-top: '70px';">
  <img src="https://miro.medium.com/v2/resize:fit:996/1*xNQKHj5vR7w9AcY_bDKYYw.gif" alt="image"/>
</div>

<h2 align="center">🌐 Socials:</h2>
<div align="center"> 
  <a href="mailto:xushboqovaxliddin7@gmail.com">
    <img src="https://img.shields.io/badge/Gmail-333333?style=for-the-badge&logo=gmail&logoColor=red" />
  </a>
  <a href="https://www.linkedin.com/in/axliddin-xushboqov-b74a38273/" target="_blank">
    <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" />
  </a>
  <a href="https://github.com/AxliddinXushboqov" target="_blank">
    <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" />
  </a>
  <a href="https://t.me/Khushbokov_D" target="_blank">
    <img src="https://img.shields.io/badge/Telegram-0088CC?style=for-the-badge&logo=telegram&logoColor=white" />
  </a>
</div>



<h2 align="center">⚒️ Languages, Frameworks & Tools ⚒️</h2>
<br/>

<div align="center">

  <!-- Frontend -->
  <h3>🌐 Frontend</h3>
  <div style="display:flex; gap:10px; justify-content:center; flex-wrap:wrap;">
    <img src="https://skillicons.dev/icons?i=html,css,bootstrap,javascript" alt="Frontend Icons" />
  </div>
  <br/>

  <!-- Backend -->
  <h3>🖥️ Backend</h3>
  <div style="display:flex; gap:10px; justify-content:center; flex-wrap:wrap;">
    <img src="https://skillicons.dev/icons?i=python,dotnet,java,cs,cpp" alt="Backend Icons" />
  </div>
  <br/>

  <!-- Database -->
  <h3>🗄️ Databases</h3>
  <div style="display:flex; gap:10px; justify-content:center; flex-wrap:wrap;">
    <img src="https://skillicons.dev/icons?i=mongodb,postgres,sqlite" alt="Database Icons" />
  </div>
  <br/>

  <!-- Tools -->
  <h3>🛠️ Tools & IDEs</h3>
  <div style="display:flex; gap:10px; justify-content:center; flex-wrap:wrap;">
    <img src="https://skillicons.dev/icons?i=vscode,visualstudio,github,postman,kali" alt="Tools Icons" />
  </div>
</div>

<hr/>


# 📊 GitHub Stats:
<div align=center>
  <img width=390 src="https://github-readme-streak-stats-salesp07.vercel.app/?user=AxliddinXushboqov&count_private=true&theme=react&border_radius=10" alt="streak stats"/>
  <img width=390 src="https://github-readme-stats-salesp07.vercel.app/api?username=AxliddinXushboqov&count_private=true&show_icons=true&theme=react&rank_icon=github&border_radius=10" alt="readme stats" />
  <br/>
  <img width=325 align="center" src="https://github-readme-stats-salesp07.vercel.app/api/top-langs/?username=AxliddinXushboqov&hide=HTML&langs_count=8&layout=compact&theme=react&border_radius=10&size_weight=0.5&count_weight=0.5&exclude_repo=github-readme-stats" alt="top langs" />
</div>

<br/><br/>


<div align="center">
  <h2>🐍 My Contributions 🐍</h2>
  <br>
  <img alt="snake eating my contributions" src="https://github.com/marjan-ahmed/marjan-ahmed/blob/manual-run-output/only-svg/github-contribution-grid-snake-dark.svg" />
  
  <br/><br/><br/>

<!-- Proudly created with GPRM ( https://gprm.itsvg.in ) -->

<!doctype html>
<html lang="uz">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Mening sahifam</title>
  <style>
    body{font-family:system-ui,Segoe UI,Roboto,Arial;margin:0;height:100vh;overflow:hidden;background:#0b1020;color:#fff}
    .center {
      position: absolute; left:50%; top:50%; transform:translate(-50%,-50%);
      text-align:center;
    }
    .avatar{
      width:120px;height:120px;border-radius:50%;background:white;background-image:url('https://avatars.githubusercontent.com/<username>');background-size:cover;margin:0 auto 12px;border:4px solid rgba(255,255,255,0.12);
    }
    /* Suzuvchi elementlar */
    .float {
      position: absolute;
      pointer-events: none;
      font-weight:700;
      transform: translate(-50%,-50%);
      user-select: none;
      -webkit-user-select: none;
      opacity: 0.95;
      text-shadow: 0 2px 8px rgba(0,0,0,.6);
      mix-blend-mode: screen;
    }
  </style>
</head>
<body>
  <div class="center">
    <div class="avatar" id="myAvatar"></div>
    <h1>@<span id="uname">USERNAME</span></h1>
    <p>Assalomu alaykum — sizning sahifangizga xush kelibsiz!</p>
  </div>

  <script>
    // --- SOZLAMALAR ---
    const texts = ['Salom', 'Welcome', 'Hallo', 'Assalom', '👋', '🚀', '🔥']; // suzuvchi so'zlar
    const maxItems = 14; // nechta element bo'lishi mumkin
    const speed = 0.6; // harakat tezligi (katta bo'lsa tezroq)

    // Sahifaga elementlar qo'shish
    function createFloat(i){
      const el = document.createElement('div');
      el.className = 'float';
      el.textContent = texts[i % texts.length];
      el.style.left = (50 + (Math.random()*80-40)) + '%';
      el.style.top = (50 + (Math.random()*80-40)) + '%';
      el.style.fontSize = (12 + Math.random()*28) + 'px';
      el.style.color = `hsl(${Math.floor(Math.random()*360)}, 80%, 65%)`;
      el.dataset.vx = (Math.random()*2-1) * speed;
      el.dataset.vy = (Math.random()*2-1) * speed;
      document.body.appendChild(el);
      return el;
    }

    // yarating
    const floats = [];
    for(let i=0;i<maxItems;i++) floats.push(createFloat(i));

    // animatsiya loop
    function tick(){
      for(const f of floats){
        let x = parseFloat(f.style.left) || 50;
        let y = parseFloat(f.style.top) || 50;
        x += parseFloat(f.dataset.vx);
        y += parseFloat(f.dataset.vy);
        // boshqa tomonlarga chiqmasligi uchun cheklash va "sakrash"
        if(x < 2 || x > 98) f.dataset.vx *= -1;
        if(y < 2 || y > 98) f.dataset.vy *= -1;
        f.style.left = x + '%';
        f.style.top  = y + '%';
      }
      requestAnimationFrame(tick);
    }
    tick();

    // OPTIONAL: avatar ostidagi username-ni dinamik to'ldirish
    (function setUser(){
      const name = location.pathname.split('/')[1] || 'USERNAME';
      document.getElementById('uname').textContent = name.toLowerCase() === '' ? 'USERNAME' : name;
      // Agar GitHub avatar dan foydalanmoqchi bo'lsangiz:
      const av = document.getElementById('myAvatar');
      av.style.backgroundImage = "url('https://github.com/<AxliddinXushboqov>.png')";
    })();
  </script>
</body>
</html>

