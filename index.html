<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/>
<title>M87* — Collection</title>
<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,300;1,300&family=DM+Mono:wght@300;400&family=DM+Sans:wght@200;300&display=swap" rel="stylesheet"/>
<style>
*{box-sizing:border-box;margin:0;padding:0;}
body{background:#02010a;font-family:'DM Sans',sans-serif;color:#f0ede8;min-height:100vh;overflow-x:hidden;}

/* Star bg */
#star-canvas{position:fixed;inset:0;z-index:0;}

.content{position:relative;z-index:1;padding:80px 48px;}
header{text-align:center;margin-bottom:80px;}
.h-eyebrow{font-family:'DM Mono',monospace;font-size:11px;letter-spacing:.25em;color:rgba(200,168,99,.5);margin-bottom:20px;}
h1{font-family:'Cormorant Garamond',serif;font-size:clamp(60px,10vw,120px);font-weight:300;letter-spacing:-3px;line-height:.95;margin-bottom:20px;}
h1 em{font-style:italic;color:#c8a863;}
.h-sub{font-family:'DM Mono',monospace;font-size:11px;letter-spacing:.15em;color:rgba(240,237,232,.25);}

.grid{display:grid;grid-template-columns:repeat(3,1fr);gap:2px;}
a.site-card{display:block;position:relative;overflow:hidden;text-decoration:none;aspect-ratio:4/3;cursor:pointer;}
a.site-card:hover .preview-canvas{transform:scale(1.06);}
a.site-card:hover .card-overlay{background:rgba(2,1,10,.4);}
.preview-canvas{width:100%;height:100%;transition:transform .6s cubic-bezier(.16,1,.3,1);}
.card-overlay{position:absolute;inset:0;background:rgba(2,1,10,.65);display:flex;flex-direction:column;justify-content:flex-end;padding:28px;transition:background .3s;}
.card-num{font-family:'DM Mono',monospace;font-size:10px;letter-spacing:.12em;color:rgba(200,168,99,.4);margin-bottom:8px;}
.card-title{font-family:'Cormorant Garamond',serif;font-size:28px;font-weight:300;letter-spacing:-.5px;color:#f0ede8;margin-bottom:4px;}
.card-title em{font-style:italic;color:#c8a863;}
.card-sub{font-size:12px;color:rgba(240,237,232,.4);margin-bottom:14px;}
.card-tags{display:flex;gap:6px;flex-wrap:wrap;}
.tag{font-family:'DM Mono',monospace;font-size:9px;padding:3px 8px;border:0.5px solid rgba(200,168,99,.2);border-radius:3px;color:rgba(200,168,99,.5);}
.card-arrow{position:absolute;top:20px;right:20px;width:32px;height:32px;border-radius:50%;border:0.5px solid rgba(200,168,99,.3);display:flex;align-items:center;justify-content:center;font-size:14px;color:rgba(200,168,99,.5);opacity:0;transform:scale(.8);transition:all .3s;}
a.site-card:hover .card-arrow{opacity:1;transform:scale(1);}

footer{text-align:center;padding:60px 48px 40px;font-family:'DM Mono',monospace;font-size:10px;color:rgba(200,168,99,.2);letter-spacing:.1em;}
@media(max-width:768px){.grid{grid-template-columns:1fr;}.content{padding:60px 20px;}}
</style>
</head>
<body>
<canvas id="star-canvas"></canvas>
<div class="content">
  <header>
    <div class="h-eyebrow">Messier 87 · Event Horizon Telescope · 2019</div>
    <h1>First<br><em>Light</em></h1>
    <div class="h-sub">Three perspectives on humanity's greatest photograph</div>
  </header>
  <div class="grid">
    <a class="site-card" href="01-blackhole-main.html">
      <canvas class="preview-canvas" id="prev1"></canvas>
      <div class="card-overlay">
        <div class="card-num">01</div>
        <div class="card-title">The <em>Discovery</em></div>
        <div class="card-sub">Editorial long-read with animated Canvas background</div>
        <div class="card-tags"><span class="tag">Canvas 2D</span><span class="tag">Parallax</span><span class="tag">Scroll reveal</span><span class="tag">Custom cursor</span></div>
      </div>
      <div class="card-arrow">↗</div>
    </a>
    <a class="site-card" href="02-blackhole-webgl.html">
      <canvas class="preview-canvas" id="prev2"></canvas>
      <div class="card-overlay">
        <div class="card-num">02</div>
        <div class="card-title"><em>Singularity</em></div>
        <div class="card-sub">Full-screen WebGL ray-marching with GLSL shader</div>
        <div class="card-tags"><span class="tag">WebGL 2</span><span class="tag">GLSL</span><span class="tag">Ray marching</span><span class="tag">Mouse drag</span></div>
      </div>
      <div class="card-arrow">↗</div>
    </a>
    <a class="site-card" href="03-blackhole-dashboard.html">
      <canvas class="preview-canvas" id="prev3"></canvas>
      <div class="card-overlay">
        <div class="card-num">03</div>
        <div class="card-title">Data <em>Explorer</em></div>
        <div class="card-sub">Live science dashboard with charts, spectrum, logs</div>
        <div class="card-tags"><span class="tag">Dashboard</span><span class="tag">Live data</span><span class="tag">Canvas charts</span><span class="tag">Tooltips</span></div>
      </div>
      <div class="card-arrow">↗</div>
    </a>
  </div>
</div>
<footer>Data: EHT Collaboration · NSF · ESO · NAOJ · 2019–2022</footer>

<script>
const PI2=Math.PI*2;
function rand(a,b){return a+(b-a)*Math.random();}

// Background starfield
(function(){
  const c=document.getElementById('star-canvas');
  const ctx=c.getContext('2d');
  let W,H;
  function resize(){W=c.width=innerWidth;H=c.height=innerHeight;}
  resize();window.addEventListener('resize',resize);
  const stars=Array.from({length:500},()=>({x:Math.random(),y:Math.random(),r:rand(.3,1.5),a:rand(.1,.7),tw:rand(0,PI2)}));
  let t=0;
  function draw(){
    t+=.004;
    ctx.fillStyle='rgba(2,1,10,.08)';ctx.fillRect(0,0,W,H);
    stars.forEach(s=>{
      const tw=.5+.5*Math.sin(t+s.tw);
      ctx.beginPath();ctx.arc(s.x*W,s.y*H,s.r,0,PI2);
      ctx.fillStyle=`rgba(240,237,232,${s.a*tw})`;ctx.fill();
    });
    requestAnimationFrame(draw);
  }
  draw();
})();

// Preview canvas mini-animations
function makePreview(id,hue1,hue2){
  const c=document.getElementById(id);
  const ctx=c.getContext('2d');
  let W,H;
  function resize(){W=c.width=c.offsetWidth;H=c.height=c.offsetHeight;}
  resize();
  const pts=Array.from({length:300},()=>{
    const r=rand(.3,.85);
    return{angle:rand(0,PI2),r,speed:rand(.004,.015)*(1/r),a:rand(.4,.9),sz:rand(.6,2),h:rand(hue1,hue2)};
  });
  let t=0;
  function draw(){
    t+=.01;
    ctx.fillStyle='rgba(2,1,10,.15)';ctx.fillRect(0,0,W,H);
    const cx=W/2,cy=H/2,R=Math.min(cx,cy)*.7;
    pts.forEach(p=>{
      p.angle+=p.speed;
      const beam=.35+.65*Math.cos(p.angle+Math.PI);
      const x=cx+Math.cos(p.angle)*p.r*R*1.7;
      const y=cy+Math.sin(p.angle)*p.r*R*.42;
      ctx.beginPath();ctx.arc(x,y,p.sz,0,PI2);
      ctx.fillStyle=`hsla(${p.h},80%,${30+beam*32}%,${p.a*beam})`;ctx.fill();
    });
    const g=ctx.createRadialGradient(cx,cy,0,cx,cy,R*.35);
    g.addColorStop(0,'#000');g.addColorStop(.8,'#000');
    g.addColorStop(.92,'rgba(0,0,0,.5)');g.addColorStop(1,'rgba(0,0,0,0)');
    ctx.beginPath();ctx.arc(cx,cy,R*.35,0,PI2);ctx.fillStyle=g;ctx.fill();
    requestAnimationFrame(draw);
  }
  draw();
}
makePreview('prev1',12,42);
makePreview('prev2',20,50);
makePreview('prev3',8,35);
</script>
</body>
</html>
