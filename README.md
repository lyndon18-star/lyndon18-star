<style>
  @import url('https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@400;600;700&display=swap');

  .ghp {
    font-family: 'Space Grotesk', system-ui, sans-serif;
    color: #e6edf3;
  }

  .ghp .hero {
    text-align: center;
    padding: 3rem 1rem 2rem;
  }

  .ghp .badge {
    display: inline-block;
    padding: 0.35rem 1rem;
    margin: 0.25rem;
    font-size: 0.8rem;
    font-weight: 600;
    letter-spacing: 0.08em;
    text-transform: uppercase;
    border-radius: 999px;
    border: 1px solid #30363d;
    background: linear-gradient(135deg, rgba(56,139,253,.12), rgba(121,192,255,.06));
    color: #79c0ff;
    transition: transform .25s ease, box-shadow .25s ease, border-color .25s ease;
  }
  .ghp .badge:hover {
    transform: translateY(-2px);
    border-color: #79c0ff;
    box-shadow: 0 4px 20px rgba(56,139,253,.25);
  }

  .ghp h1 {
    font-size: 3rem;
    font-weight: 700;
    margin: 1rem 0 0.5rem;
    background: linear-gradient(90deg, #58a6ff, #bc8cff, #f778ba, #58a6ff);
    background-size: 300% 100%;
    -webkit-background-clip: text;
    background-clip: text;
    -webkit-text-fill-color: transparent;
    animation: ghp-gradient 6s ease infinite;
  }

  .ghp .tagline {
    font-size: 1.15rem;
    color: #8b949e;
    margin-bottom: 1.5rem;
  }

  .ghp .typed {
    display: inline-block;
    color: #79c0ff;
    font-weight: 600;
  }
  .ghp .typed::after {
    content: '▋';
    color: #f778ba;
    animation: ghp-blink 1s steps(1) infinite;
  }

  .ghp h2 {
    font-size: 1.35rem;
    font-weight: 600;
    margin-top: 3rem;
    margin-bottom: 1rem;
    padding-bottom: 0.5rem;
    border-bottom: 2px solid;
    border-image: linear-gradient(90deg, #58a6ff, transparent) 1;
  }

  .ghp .card {
    border: 1px solid #30363d;
    border-radius: 14px;
    padding: 1.5rem 2rem;
    margin: 1rem auto;
    max-width: 760px;
    background: linear-gradient(160deg, #161b22, #0d1117);
    box-shadow: 0 8px 24px rgba(0,0,0,.4);
    transition: transform .3s ease, box-shadow .3s ease, border-color .3s ease;
  }
  .ghp .card:hover {
    transform: translateY(-4px);
    border-color: #58a6ff;
    box-shadow: 0 16px 40px rgba(56,139,253,.18);
  }

  .ghp .type-list {
    list-style: none;
    margin: 0;
    padding: 0;
    text-align: left;
    font-size: 0.95rem;
    color: #c9d1d9;
  }
  .ghp .type-list li {
    padding: 0.35rem 0;
    border-bottom: 1px dashed #21262d;
    transition: color .2s ease, transform .2s ease;
  }
  .ghp .type-list li:last-child { border-bottom: none; }
  .ghp .type-list li:hover {
    color: #79c0ff;
    transform: translateX(6px);
  }

  .ghp .stack {
    text-align: center;
    margin: 1rem 0;
  }

  .ghp .stack img {
    transition: transform .25s ease, filter .25s ease;
    border-radius: 8px;
    margin: 0.2rem;
  }
  .ghp .stack img:hover {
    transform: translateY(-4px) scale(1.05);
    filter: drop-shadow(0 6px 16px rgba(88,166,255,.3));
  }

  .ghp .stat {
    text-align: center;
    margin: 0.75rem 0;
  }
  .ghp .stat img {
    transition: transform .3s ease, box-shadow .3s ease;
    border-radius: 14px;
  }
  .ghp .stat img:hover {
    transform: translateY(-4px);
    box-shadow: 0 16px 40px rgba(56,139,253,.18);
  }

  .ghp .soc { text-align: center; margin-top: 1rem; }
  .ghp .soc a { text-decoration: none; display: inline-block; transition: transform .25s ease, opacity .25s ease; }
  .ghp .soc a:hover { transform: translateY(-3px); opacity: .85; }

  .ghp .foot {
    text-align: center;
    color: #8b949e;
    font-size: 0.85rem;
    margin-top: 3.5rem;
    animation: ghp-fade-in 1.5s ease both;
  }

  .ghp .reveal { animation: ghp-reveal .8s ease both; }
  .ghp .reveal:nth-of-type(1) { animation-delay: .1s; }
  .ghp .reveal:nth-of-type(2) { animation-delay: .25s; }
  .ghp .reveal:nth-of-type(3) { animation-delay: .4s; }

  @keyframes ghp-gradient {
    0% { background-position: 0% 50%; }
    50% { background-position: 100% 50%; }
    100% { background-position: 0% 50%; }
  }

  @keyframes ghp-blink {
    0%, 100% { opacity: 1; }
    50% { opacity: 0; }
  }

  @keyframes ghp-reveal {
    from { opacity: 0; transform: translateY(16px); }
    to { opacity: 1; transform: translateY(0); }
  }

  @keyframes ghp-fade-in {
    from { opacity: 0; }
    to { opacity: 1; }
  }
</style>

<div class="ghp">

  <!-- ============ HERO ============ -->
  <div class="hero">
    <span class="badge">IT Student</span>
    <span class="badge">Student Leader</span>
    <span class="badge">Developer</span>

    <h1>Hey, I'm Lyndon 👋</h1>
    <p class="tagline">Motivated · Hardworking · <span class="typed">Always Learning</span></p>
  </div>

  <!-- ============ ABOUT ============ -->
  <h2>💫 About Me</h2>

  <div class="card reveal">
    <p>I am a motivated and hardworking IT student with a passion for learning, technology, and personal growth. As a student leader who has held various positions, I have developed strong skills in teamwork, communication, leadership, and responsibility. I am eager to apply my knowledge, gain practical experience, take on new challenges, and contribute positively to a professional work environment while building a strong foundation for my future career.</p>
  </div>

  <!-- ============ SOCIALS ============ -->
  <h2>🌐 Socials</h2>

  <div class="soc reveal">
    <a href="https://discord.gg/981812902170349578">
      <img alt="Discord" src="https://img.shields.io/badge/Discord-%237289DA.svg?logo=discord&logoColor=white" />
    </a>
    <a href="https://facebook.com/lyndon.bautista.680329">
      <img alt="Facebook" src="https://img.shields.io/badge/Facebook-%231877F2.svg?logo=Facebook&logoColor=white" />
    </a>
    <a href="https://instagram.com/cheesypuppin_">
      <img alt="Instagram" src="https://img.shields.io/badge/Instagram-%23E4405F.svg?logo=Instagram&logoColor=white" />
    </a>
    <a href="https://linkedin.com/in/lyndon-bautista-abb580395">
      <img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-%230077B5.svg?logo=linkedin&logoColor=white" />
    </a>
    <a href="https://pinterest.com/lyndonbtst">
      <img alt="Pinterest" src="https://img.shields.io/badge/Pinterest-%23E60023.svg?logo=Pinterest&logoColor=white" />
    </a>
    <a href="https://reddit.com/user/Bautista_Lyndon">
      <img alt="Reddit" src="https://img.shields.io/badge/Reddit-%23FF4500.svg?logo=Reddit&logoColor=white" />
    </a>
    <a href="https://tiktok.com/@@wimp_sy">
      <img alt="TikTok" src="https://img.shields.io/badge/TikTok-%23000000.svg?logo=TikTok&logoColor=white" />
    </a>
    <a href="https://x.com/@lyndon_yur">
      <img alt="X" src="https://img.shields.io/badge/X-black.svg?logo=X&logoColor=white" />
    </a>
    <a href="mailto:lyndobtst@gmail.com">
      <img alt="Email" src="https://img.shields.io/badge/Email-D14836?logo=gmail&logoColor=white" />
    </a>
  </div>

  <!-- ============ TECH STACK ============ -->
  <h2>💻 Tech Stack</h2>

  <div class="stack reveal">
    <img alt="CSS3" src="https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white" />
    <img alt="C" src="https://img.shields.io/badge/c-%2300599C.svg?style=for-the-badge&logo=c&logoColor=white" />
    <img alt="C#" src="https://img.shields.io/badge/c%23-%23239120.svg?style=for-the-badge&logo=csharp&logoColor=white" />
    <img alt="C++" src="https://img.shields.io/badge/c++-%2300599C.svg?style=for-the-badge&logo=c%2B%2B&logoColor=white" />
    <img alt="Crystal" src="https://img.shields.io/badge/crystal-%23000000.svg?style=for-the-badge&logo=crystal&logoColor=white" />
    <img alt="HTML5" src="https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white" />
    <img alt="Java" src="https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white" />
    <img alt="JavaScript" src="https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E" />
    <img alt="Julia" src="https://img.shields.io/badge/-Julia-9558B2?style=for-the-badge&logo=julia&logoColor=white" />
    <img alt="PHP" src="https://img.shields.io/badge/php-%23777BB4.svg?style=for-the-badge&logo=php&logoColor=white" />
    <img alt="Rust" src="https://img.shields.io/badge/rust-%23000000.svg?style=for-the-badge&logo=rust&logoColor=white" />
    <img alt="Ruby" src="https://img.shields.io/badge/ruby-%23CC342D.svg?style=for-the-badge&logo=ruby&logoColor=white" />
    <img alt="TypeScript" src="https://img.shields.io/badge/typescript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white" />
    <img alt="Windows Terminal" src="https://img.shields.io/badge/Windows%20Terminal-%234D4D4D.svg?style=for-the-badge&logo=windows-terminal&logoColor=white" />
    <img alt="Python" src="https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54" />
  </div>

  <div class="stack">
    <img alt="Firebase" src="https://img.shields.io/badge/firebase-%23039BE5.svg?style=for-the-badge&logo=firebase" />
    <img alt="Vercel" src="https://img.shields.io/badge/vercel-%23000000.svg?style=for-the-badge&logo=vercel&logoColor=white" />
    <img alt="Netlify" src="https://img.shields.io/badge/netlify-%23000000.svg?style=for-the-badge&logo=netlify&logoColor=%2300C7B7" />
    <img alt=".Net" src="https://img.shields.io/badge/.NET-5C2D91?style=for-the-badge&logo=.net&logoColor=white" />
    <img alt="Bootstrap" src="https://img.shields.io/badge/bootstrap-%238511FA.svg?style=for-the-badge&logo=bootstrap&logoColor=white" />
    <img alt="Django" src="https://img.shields.io/badge/django-%23092E20.svg?style=for-the-badge&logo=django&logoColor=white" />
    <img alt="Flutter" src="https://img.shields.io/badge/Flutter-%2302569B.svg?style=for-the-badge&logo=Flutter&logoColor=white" />
    <img alt="JavaFX" src="https://img.shields.io/badge/javafx-%23FF0000.svg?style=for-the-badge&logo=javafx&logoColor=white" />
    <img alt="JWT" src="https://img.shields.io/badge/JWT-black?style=for-the-badge&logo=JSON%20web%20tokens" />
    <img alt="NodeJS" src="https://img.shields.io/badge/node.js-6DA55F?style=for-the-badge&logo=node.js&logoColor=white" />
    <img alt="React" src="https://img.shields.io/badge/react-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB" />
    <img alt="TailwindCSS" src="https://img.shields.io/badge/tailwindcss-%2338B2AC.svg?style=for-the-badge&logo=tailwind-css&logoColor=white" />
  </div>

  <div class="stack">
    <img alt="Firebase" src="https://img.shields.io/badge/firebase-a08021?style=for-the-badge&logo=firebase&logoColor=ffcd34" />
    <img alt="Postgres" src="https://img.shields.io/badge/postgres-%23316192.svg?style=for-the-badge&logo=postgresql&logoColor=white" />
    <img alt="MySQL" src="https://img.shields.io/badge/mysql-4479A1.svg?style=for-the-badge&logo=mysql&logoColor=white" />
    <img alt="MongoDB" src="https://img.shields.io/badge/MongoDB-%234ea94b.svg?style=for-the-badge&logo=mongodb&logoColor=white" />
    <img alt="MariaDB" src="https://img.shields.io/badge/MariaDB-003545?style=for-the-badge&logo=mariadb&logoColor=white" />
    <img alt="SQLite" src="https://img.shields.io/badge/sqlite-%2307405e.svg?style=for-the-badge&logo=sqlite&logoColor=white" />
    <img alt="Supabase" src="https://img.shields.io/badge/Supabase-3ECF8E?style=for-the-badge&logo=supabase&logoColor=white" />
  </div>

  <div class="stack">
    <img alt="Adobe" src="https://img.shields.io/badge/adobe-%23FF0000.svg?style=for-the-badge&logo=adobe&logoColor=white" />
    <img alt="Adobe After Effects" src="https://img.shields.io/badge/Adobe%20After%20Effects-9999FF.svg?style=for-the-badge&logo=Adobe%20After%20Effects&logoColor=white" />
    <img alt="Adobe Lightroom" src="https://img.shields.io/badge/Adobe%20Lightroom-31A8FF.svg?style=for-the-badge&logo=Adobe%20Lightroom&logoColor=white" />
    <img alt="Figma" src="https://img.shields.io/badge/figma-%23F24E1E.svg?style=for-the-badge&logo=figma&logoColor=white" />
    <img alt="Canva" src="https://img.shields.io/badge/Canva-%2300C4CC.svg?style=for-the-badge&logo=Canva&logoColor=white" />
    <img alt="Storybook" src="https://img.shields.io/badge/-Storybook-FF4785?style=for-the-badge&logo=storybook&logoColor=white" />
    <img alt="Sketch" src="https://img.shields.io/badge/Sketch-FFB387?style=for-the-badge&logo=sketch&logoColor=black" />
    <img alt="GitHub" src="https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white" />
    <img alt="Git" src="https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white" />
    <img alt="Cisco" src="https://img.shields.io/badge/cisco-%23049fd9.svg?style=for-the-badge&logo=cisco&logoColor=black" />
  </div>

  <!-- ============ STATS ============ -->
  <h2>📊 GitHub Stats</h2>

  <div class="stat reveal">
    <img alt="GitHub stats" src="https://github-readme-stats.shion.dev/api?username=lyndon18-star&theme=dark&hide_border=false&include_all_commits=false&count_private=false" />
  </div>

  <div class="stat">
    <img alt="Streak" src="https://streak-stats.demolab.com/?user=lyndon18-star&theme=dark&hide_border=false" />
  </div>

  <div class="stat">
    <img alt="Top languages" src="https://github-readme-stats.shion.dev/api/top-langs/?username=lyndon18-star&theme=dark&hide_border=false&include_all_commits=false&count_private=false&layout=compact" />
  </div>

  <!-- ============ TROPHIES ============ -->
  <h2>🏆 GitHub Trophies</h2>

  <div class="stat reveal">
    <img alt="Trophies" src="https://github-profile-trophy.vercel.app/?username=lyndon18-star&theme=radical&no-frame=false&no-bg=true&margin-w=4" />
  </div>

  <!-- ============ QUOTE ============ -->
  <h2>✍️ Random Dev Quote</h2>

  <div class="stat reveal">
    <img alt="Quote" src="https://quotes-github-readme.vercel.app/api?type=horizontal&theme=radical" />
  </div>

  <!-- ============ TOP CONTRIBUTED ============ -->
  <h2>🔝 Top Contributed Repo</h2>

  <div class="stat reveal">
    <img alt="Top contributed repo" src="https://github-contributor-stats.vercel.app/api?username=lyndon18-star&limit=5&theme=dark&combine_all_yearly_contributions=true" />
  </div>

  <div class="foot">
    <img alt="Profile views" src="https://komarev.com/ghpvc/?username=lyndon18-star&icon=2&color=0" />
    <br /><br />
    Made with 💙 · lyndon18-star
  </div>

</div>
