<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8"/>
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>Alexsander Martins — GitHub Profile</title>
<link rel="preconnect" href="https://fonts.googleapis.com"/>
<link href="https://fonts.googleapis.com/css2?family=Space+Mono:wght@400;700&family=Fira+Code:wght@300;400;500&display=swap" rel="stylesheet"/>
<style>
  *{box-sizing:border-box;margin:0;padding:0}
  body{background:#0d1117;color:#e6edf3;font-family:'Fira Code',monospace;min-height:100vh}
  .readme{padding:2rem;max-width:900px;margin:0 auto;position:relative;overflow:hidden}

  /* Stars */
  .stars{position:fixed;inset:0;pointer-events:none;z-index:0}
  .star{position:absolute;background:white;border-radius:50%;animation:twinkle var(--d,3s) ease-in-out infinite}
  @keyframes twinkle{0%,100%{opacity:.08}50%{opacity:1}}

  .content{position:relative;z-index:1}

  /* Header */
  .header{display:flex;align-items:flex-start;justify-content:space-between;gap:2rem;margin-bottom:2rem;flex-wrap:wrap}
  .title-section{flex:1;min-width:260px}

  .name-badge{display:inline-flex;align-items:center;gap:8px;background:#161b22;border:1px solid #30363d;border-radius:8px;padding:6px 14px;font-size:11px;color:#8b949e;margin-bottom:12px;letter-spacing:1px;text-transform:uppercase}
  .dot{width:6px;height:6px;border-radius:50%;background:#3fb950;animation:pulse 2s ease-in-out infinite}
  @keyframes pulse{0%,100%{opacity:1;transform:scale(1)}50%{opacity:.5;transform:scale(.8)}}

  h1{font-family:'Space Mono',monospace;font-size:2rem;font-weight:700;background:linear-gradient(90deg,#58a6ff,#bc8cff,#ff7b72);-webkit-background-clip:text;-webkit-text-fill-color:transparent;background-clip:text;margin-bottom:6px}
  .role-tag{display:inline-block;background:#161b22;border:1px solid #30363d;color:#58a6ff;font-size:12px;padding:3px 12px;border-radius:20px;margin-bottom:16px}
  .bio{color:#8b949e;font-size:13px;line-height:1.8;max-width:480px}
  .bio strong{color:#e6edf3}

  /* Death Star */
  .ds-wrap{display:flex;justify-content:center;align-items:center;padding:0.5rem}
  canvas{image-rendering:pixelated;image-rendering:crisp-edges}

  /* Divider */
  .divider{height:1px;background:linear-gradient(90deg,transparent,#30363d,transparent);margin:1.5rem 0}

  /* Section title */
  .section-title{font-family:'Space Mono',monospace;font-size:13px;color:#8b949e;text-transform:uppercase;letter-spacing:2px;margin-bottom:1rem;display:flex;align-items:center;gap:8px}
  .section-title::after{content:'';flex:1;height:1px;background:#21262d}

  /* Tech pills */
  .tech-grid{display:flex;flex-wrap:wrap;gap:10px;margin-bottom:1.5rem}
  .tech-pill{display:flex;align-items:center;gap:8px;background:#161b22;border:1px solid #30363d;border-radius:8px;padding:6px 12px;font-size:12px;color:#c9d1d9;transition:border-color .2s,background .2s;cursor:default;text-decoration:none}
  .tech-pill:hover{border-color:#58a6ff;background:#1c2330}
  .tech-pill img{width:18px;height:18px;border-radius:3px}

  /* AI pills */
  .ai-pill{border-color:#3d2b6e}
  .ai-pill:hover{border-color:#bc8cff;background:#1a1230}
  .ai-icon{width:18px;height:18px;border-radius:3px;display:flex;align-items:center;justify-content:center;font-size:11px;font-weight:700;flex-shrink:0;font-family:'Fira Code',monospace}
  .claude-icon{background:linear-gradient(135deg,#c97b4b,#e8956d);color:white}
  .gpt-icon{background:#10a37f;color:white}
  .gemini-icon{background:linear-gradient(135deg,#4285f4,#ea4335,#fbbc04);color:white}

  /* Stats */
  .stats-row{display:grid;grid-template-columns:1fr 1fr;gap:12px;margin-bottom:1.5rem}
  .stats-row img{width:100%;border-radius:8px;border:1px solid #30363d}

  /* Footer */
  .footer-line{margin-top:1.5rem;text-align:center;font-size:11px;color:#484f58;letter-spacing:1px;padding-bottom:1rem}

  @media(max-width:600px){
    .header{flex-direction:column-reverse;align-items:center}
    h1{font-size:1.5rem}
    .stats-row{grid-template-columns:1fr}
  }
</style>
</head>
<body>

<div class="stars" id="stars"></div>

<div class="readme">
  <div class="content">

    <div class="header">
      <div class="title-section">
        <div class="name-badge"><span class="dot"></span> open to work</div>
        <h1>Alexsander Martins</h1>
        <div class="role-tag">&lt; Front-End Developer /&gt;</div>
        <p class="bio">
          Olá! Sou do <strong>Rio Grande do Sul</strong>, apaixonado por tecnologia
          e desenvolvimento web. Cursando <strong>ADS na Uniaselvi</strong>, trabalho
          remotamente criando interfaces e soluções digitais. Compartilho conhecimento
          e código nessa galáxia chamada GitHub.
        </p>
      </div>
      <div class="ds-wrap">
        <canvas id="ds" width="220" height="220"></canvas>
      </div>
    </div>

    <div class="divider"></div>

    <div class="section-title">// linguagens &amp; tecnologias</div>
    <div class="tech-grid">
      <span class="tech-pill"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/html5/html5-original.svg" alt="HTML5"/>HTML5</span>
      <span class="tech-pill"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/css3/css3-original.svg" alt="CSS3"/>CSS3</span>
      <span class="tech-pill"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/javascript/javascript-original.svg" alt="JavaScript"/>JavaScript</span>
      <span class="tech-pill"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/react/react-original.svg" alt="React"/>React</span>
      <span class="tech-pill"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/python/python-original.svg" alt="Python"/>Python</span>
    </div>

    <div class="section-title">// inteligências artificiais</div>
    <div class="tech-grid">
      <span class="tech-pill ai-pill"><span class="ai-icon claude-icon">C</span>Claude (Anthropic)</span>
      <span class="tech-pill ai-pill"><span class="ai-icon gpt-icon">G</span>ChatGPT (OpenAI)</span>
      <span class="tech-pill ai-pill"><span class="ai-icon gemini-icon">✦</span>Gemini (Google)</span>
    </div>

    <div class="section-title">// estatísticas</div>
    <div class="stats-row">
      <img src="https://github-readme-stats.vercel.app/api?username=SkotAlexsander&show_icons=true&theme=tokyonight&include_all_commits=true&locale=pt-br&hide_border=true&bg_color=0d1117" alt="GitHub Stats"/>
      <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=SkotAlexsander&theme=tokyonight&layout=compact&custom_title=Tecnologias&langs_count=9&hide_border=true&bg_color=0d1117" alt="Linguagens mais usadas"/>
    </div>

    <div class="footer-line">May the code be with you &mdash; Rio Grande do Sul, Brasil</div>
  </div>
</div>

<script>
/* ---- STARS ---- */
(function(){
  const c=document.getElementById('stars');
  for(let i=0;i<100;i++){
    const s=document.createElement('div');
    s.className='star';
    const sz=Math.random()<0.25?2:1;
    s.style.cssText=`width:${sz}px;height:${sz}px;left:${Math.random()*100}%;top:${Math.random()*100}%;--d:${2+Math.random()*6}s;animation-delay:${Math.random()*6}s`;
    c.appendChild(s);
  }
})();

/* ---- DEATH STAR ---- */
(function(){
  const canvas=document.getElementById('ds');
  const ctx=canvas.getContext('2d');
  const W=220,H=220,CX=110,CY=110;
  let t=0;

  function draw(){
    ctx.clearRect(0,0,W,H);

    const rot=t*0.004;
    const pulse=Math.sin(t*0.05);
    const beamCycle=Math.floor(t/200)%6;
    const beamActive=beamCycle===5;
    const beamProgress=(t%200)/200;

    ctx.save();
    ctx.translate(CX,CY);
    ctx.rotate(rot);

    const R=88;

    /* --- sphere base --- */
    ctx.beginPath();
    ctx.arc(0,0,R,0,Math.PI*2);
    ctx.fillStyle='#181c22';
    ctx.fill();
    ctx.strokeStyle='#3a4050';
    ctx.lineWidth=1.5;
    ctx.stroke();

    /* --- latitude/longitude grid --- */
    const numLat=12;
    for(let i=0;i<numLat;i++){
      const a=(i/numLat)*Math.PI*2;
      ctx.beginPath();
      ctx.moveTo(0,0);
      ctx.lineTo(Math.cos(a)*R,Math.sin(a)*R);
      ctx.strokeStyle='rgba(55,65,80,0.45)';
      ctx.lineWidth=0.5;
      ctx.stroke();
    }
    for(let r=18;r<R;r+=18){
      ctx.beginPath();
      ctx.arc(0,0,r,0,Math.PI*2);
      ctx.strokeStyle='rgba(55,65,80,0.4)';
      ctx.lineWidth=0.5;
      ctx.stroke();
    }

    /* --- surface panel shading --- */
    for(let i=0;i<numLat;i++){
      const a1=(i/numLat)*Math.PI*2;
      const a2=((i+1)/numLat)*Math.PI*2;
      for(let r=9;r<R-6;r+=18){
        const brightness=0.12+Math.sin(t*0.018+i*0.7+r*0.09)*0.07;
        ctx.beginPath();
        ctx.arc(0,0,r,a1,a2);
        ctx.strokeStyle=`rgba(75,100,135,${brightness})`;
        ctx.lineWidth=10;
        ctx.stroke();
      }
    }

    /* --- equatorial trench --- */
    ctx.beginPath();
    ctx.arc(0,0,R,Math.PI*1.08,Math.PI*1.92);
    ctx.strokeStyle='rgba(90,110,140,0.7)';
    ctx.lineWidth=5;
    ctx.stroke();
    ctx.beginPath();
    ctx.arc(0,0,R-3,Math.PI*1.1,Math.PI*1.9);
    ctx.strokeStyle='rgba(50,65,85,0.9)';
    ctx.lineWidth=3;
    ctx.stroke();

    /* --- detail dots scattered --- */
    [[60,0],[60,72],[60,144],[60,216],[60,288],[38,36],[38,108],[38,180],[38,252]].forEach(([r,deg])=>{
      const a=deg*(Math.PI/180);
      ctx.beginPath();
      ctx.arc(Math.cos(a)*r,Math.sin(a)*r,2,0,Math.PI*2);
      ctx.fillStyle='rgba(85,110,145,0.8)';
      ctx.fill();
    });

    /* --- superlaser dish --- */
    ctx.beginPath();
    ctx.arc(-30,-30,24,0,Math.PI*2);
    ctx.fillStyle='#1e2530';
    ctx.fill();
    ctx.strokeStyle='#3d4d60';
    ctx.lineWidth=1.5;
    ctx.stroke();

    /* dish rings */
    [16,10,5].forEach(r=>{
      ctx.beginPath();
      ctx.arc(-30,-30,r,0,Math.PI*2);
      ctx.strokeStyle='rgba(70,95,130,0.6)';
      ctx.lineWidth=1;
      ctx.stroke();
    });

    /* dish glow core */
    const glowAlpha=0.55+pulse*0.45;
    const gr=ctx.createRadialGradient(-30,-30,0,-30,-30,20);
    gr.addColorStop(0,`rgba(120,210,255,${glowAlpha})`);
    gr.addColorStop(0.35,`rgba(60,140,220,${glowAlpha*0.7})`);
    gr.addColorStop(1,'rgba(20,60,120,0)');
    ctx.beginPath();
    ctx.arc(-30,-30,20,0,Math.PI*2);
    ctx.fillStyle=gr;
    ctx.fill();

    ctx.beginPath();
    ctx.arc(-30,-30,5,0,Math.PI*2);
    ctx.fillStyle=`rgba(200,240,255,${0.75+pulse*0.25})`;
    ctx.fill();

    /* dish spokes */
    for(let d=0;d<4;d++){
      const a=d*Math.PI/2;
      ctx.beginPath();
      ctx.moveTo(-30+Math.cos(a)*5,-30+Math.sin(a)*5);
      ctx.lineTo(-30+Math.cos(a)*20,-30+Math.sin(a)*20);
      ctx.strokeStyle='rgba(90,130,170,0.6)';
      ctx.lineWidth=1;
      ctx.stroke();
    }

    ctx.restore();

    /* ---- SUPERLASER BEAM ---- */
    if(beamActive && beamProgress<0.75){
      const bAlpha=Math.sin(beamProgress*Math.PI)*0.95;
      const bLen=beamProgress*320;

      const dishWorldX=CX+(Math.cos(rot)*(-30)-Math.sin(rot)*(-30));
      const dishWorldY=CY+(Math.sin(rot)*(-30)+Math.cos(rot)*(-30));
      const beamDir=rot-Math.PI/4;

      ctx.save();
      ctx.globalAlpha=bAlpha;
      ctx.shadowColor='rgba(100,210,255,0.9)';
      ctx.shadowBlur=20;

      /* core beam */
      const bg=ctx.createLinearGradient(
        dishWorldX,dishWorldY,
        dishWorldX+Math.cos(beamDir)*bLen,
        dishWorldY+Math.sin(beamDir)*bLen
      );
      bg.addColorStop(0,'rgba(220,245,255,1)');
      bg.addColorStop(0.15,'rgba(120,200,255,0.9)');
      bg.addColorStop(0.7,'rgba(60,140,230,0.5)');
      bg.addColorStop(1,'rgba(20,80,180,0)');

      ctx.strokeStyle=bg;
      ctx.lineWidth=5;
      ctx.lineCap='round';
      ctx.beginPath();
      ctx.moveTo(dishWorldX,dishWorldY);
      ctx.lineTo(dishWorldX+Math.cos(beamDir)*bLen,dishWorldY+Math.sin(beamDir)*bLen);
      ctx.stroke();

      /* outer glow */
      ctx.globalAlpha=bAlpha*0.3;
      ctx.lineWidth=14;
      ctx.stroke();

      ctx.restore();
    }

    /* ---- ORBITING SHIPS ---- */
    const orbitR=88+16;
    [[0.014,0],[0.009,Math.PI],[0.018,Math.PI*0.6]].forEach(([speed,offset],i)=>{
      const a=t*speed+offset;
      const sx=CX+Math.cos(a)*orbitR;
      const sy=CY+Math.sin(a)*orbitR;
      const size=i===0?5:4;

      ctx.save();
      ctx.translate(sx,sy);
      ctx.rotate(a+Math.PI/2);
      ctx.beginPath();
      ctx.moveTo(0,-size);
      ctx.lineTo(size*0.6,size*0.8);
      ctx.lineTo(0,size*0.4);
      ctx.lineTo(-size*0.6,size*0.8);
      ctx.closePath();
      ctx.fillStyle=`rgba(160,185,210,${0.7+i*0.1})`;
      ctx.fill();
      ctx.restore();
    });

    t++;
    requestAnimationFrame(draw);
  }

  draw();
})();
</script>
</body>
</html>
