<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>lukeramos-eli / README.md</title>
<style>
:root{color-scheme:dark;--bg:#0b0e14;--panel:#05060d;--line:#5b63c9;--text:#e6e8ff;--mute:#9aa3e8;--dim:#6b72b8;--ts:#4486cc;--cs:#7a52d9;--html:#e5573a;--css:#9254c8;--js:#f1e05a;box-sizing:border-box;padding-top:env(safe-area-inset-top,0px);padding-bottom:env(safe-area-inset-bottom,0px)}
*{box-sizing:border-box}
html{scroll-padding-top:env(safe-area-inset-top,0px)}
body{margin:0;background:var(--bg);font-family:ui-monospace,"JetBrains Mono",Consolas,monospace;color:var(--text);padding:16px}
.win{max-width:1000px;margin:0 auto;border:1px solid #232838;border-radius:14px;background:var(--panel);overflow:hidden}
.bar{display:flex;justify-content:space-between;align-items:center;padding:14px 20px;border-bottom:1px solid #1d2231;font-size:15px}
.pill{background:#e9edf5;color:#0b0e14;border-radius:99px;padding:4px 12px;font:600 13px system-ui,sans-serif}
.body{padding:20px;display:flex;flex-direction:column;gap:16px}
.card{position:relative;border:1px solid var(--line);border-radius:22px;overflow:hidden;background:radial-gradient(120% 120% at 20% 0%,#10143a 0%,#070816 60%,#05060f 100%)}

.glow{background:radial-gradient(40% 50% at 15% 0%,#4a55c7 0%,transparent 70%),radial-gradient(40% 50% at 85% 100%,#2a8f8f55 0%,transparent 70%),radial-gradient(40% 60% at 75% 10%,#6a3a9a66 0%,transparent 70%),#080a1a}
.galaxy{height:440px}
.galaxy canvas{position:absolute;inset:0;width:100%;height:100%}
.info{position:absolute;left:36px;top:52px;z-index:2;max-width:46%}
.eyebrow{font-size:12px;letter-spacing:.3em;color:#7b83f0;font-weight:700}
h1{margin:14px 0 8px;font:800 36px system-ui,sans-serif}
.sub{color:var(--mute);font:600 17px system-ui,sans-serif}
.note{color:var(--dim);font:14px system-ui,sans-serif;margin-top:10px}
.arms{position:absolute;left:36px;bottom:40px;z-index:2;width:230px}
.arms h4{margin:0 0 10px;font-size:11px;letter-spacing:.25em;color:var(--dim)}
.row{display:flex;align-items:center;gap:10px;margin:8px 0;font:700 15px system-ui,sans-serif}
.dot{width:14px;height:14px;border-radius:50%}
.row span:last-child{margin-left:auto;color:var(--mute);font:13px ui-monospace,monospace}
.plist{padding:36px 40px}
.ph{display:flex;justify-content:space-between;align-items:center;color:var(--dim);font-size:13px;padding-bottom:14px;border-bottom:2px solid #3c4290;margin-bottom:34px}
.ph b{font-weight:400;letter-spacing:.2em;color:var(--mute)}
.grid{display:grid;grid-template-columns:1fr 1fr;gap:24px}
.proj{border:1px solid var(--line);border-radius:16px;background:#0a0c1ccc;overflow:hidden}
.proj .t{display:flex;justify-content:space-between;align-items:center;padding:10px 16px;border-bottom:1px solid var(--line);font-size:12px;color:var(--mute)}
.proj .t i{width:10px;height:10px;border-radius:50%;background:#5a5f8f}
.pb{display:grid;grid-template-columns:1fr auto;gap:12px;padding:20px 20px 14px}
.pb h3{margin:0 0 6px;font:700 22px ui-monospace,monospace}
.cur{display:inline-block;width:14px;height:3px;background:#7b83f0;margin-left:8px;animation:bl 1s steps(2) infinite}
@keyframes bl{50%{opacity:0}}
.pb p{margin:0 0 18px;color:var(--mute);font-size:13px;line-height:1.55}
.tag{display:inline-block;border:1px solid #3c4290;background:#1a1d44;border-radius:99px;padding:4px 14px;font-size:12px;color:var(--mute)}
.meta{grid-column:1/-1;color:var(--dim);font-size:13px}
.meta b{color:#6f8cf0;font-weight:400;margin-right:10px}
.donut{width:88px;height:88px;position:relative;align-self:center}
.donut svg{transform:rotate(-90deg)}
.donut em{position:absolute;inset:0;display:grid;place-items:center;font:700 13px system-ui,sans-serif;font-style:normal}
.stack{padding:32px 40px}
.stack .in{border:1px solid var(--line);border-radius:18px;padding:24px 28px;background:#06081499}
.sh{display:flex;justify-content:space-between;align-items:flex-start}
.sh h2{margin:0;font:800 34px system-ui,sans-serif}
.sh span{color:#7b83f0;font:700 18px system-ui,sans-serif}
.sd{color:var(--mute);font:700 15px system-ui,sans-serif;margin:4px 0 18px}
.lr{display:grid;grid-template-columns:150px 54px 1fr;align-items:center;gap:14px;margin:14px 0;font:700 17px system-ui,sans-serif}
.lr .n{display:flex;align-items:center;gap:12px}
.lr .p{text-align:right}
.trk{height:12px;border-radius:9px;background:#2c2c3c}
.fill{height:100%;border-radius:9px;min-width:28px;width:0;transition:width 1.4s cubic-bezier(.2,.8,.2,1)}
.foot{padding:36px;display:grid;place-items:center}
.foot .in{width:100%;border:1px solid var(--line);border-radius:22px;padding:30px;display:grid;place-items:center}
.gh{display:flex;align-items:center;gap:12px;padding:10px 24px 10px 14px;border-radius:99px;border:2px solid #9aa0e8;background:#0a0c1c;text-decoration:none;color:var(--text);box-shadow:0 0 22px #5b63c944}
.gh .g{width:34px;height:34px;border-radius:50%;background:#2c2f3a;display:grid;place-items:center;font:700 16px system-ui,sans-serif}
.gh small{display:block;color:#8d95f0;font:700 12px system-ui,sans-serif;letter-spacing:.05em}
.gh strong{font:700 16px system-ui,sans-serif}
.city{height:440px;border-color:var(--line);background:radial-gradient(40% 50% at 15% 0%,#4a55c7 0%,transparent 70%),radial-gradient(40% 50% at 85% 100%,#2a8f8f55 0%,transparent 70%),radial-gradient(40% 60% at 75% 10%,#6a3a9a66 0%,transparent 70%),#080a1a}
.city canvas{position:absolute;inset:0;width:100%;height:100%}
.ci{position:absolute;left:36px;top:44px;z-index:2;color:var(--mute)}
.ci .eyebrow{color:#7b83f0}
.ci .big{font:800 46px system-ui,sans-serif;color:var(--text);margin:10px 0 2px}
.ci .lab{font:700 17px system-ui,sans-serif;margin-bottom:18px}
.ci .st{font:700 15px system-ui,sans-serif;margin:8px 0}
.cf{position:absolute;left:36px;bottom:26px;z-index:2;color:var(--mute);font-size:13px}
.cf small{display:block;margin-top:6px;color:var(--dim);font:12px system-ui,sans-serif}
@media(max-width:720px){.city{height:520px}.ci{left:22px;top:28px}.cf{left:22px}.ci .big{font-size:38px}}
@media(max-width:720px){.galaxy{height:520px}.info{max-width:90%;left:22px;top:28px}.arms{bottom:24px;left:22px}.grid{grid-template-columns:1fr}.plist,.stack,.foot{padding:20px}.lr{grid-template-columns:110px 44px 1fr}h1{font-size:28px}}
</style>
</head>
<body>
<div class="win">
  <div class="bar"><span>lukeramos-eli / README.md</span><span class="pill">Pro template</span></div>
  <div class="body">

    <section class="card galaxy">
      <canvas id="gx"></canvas>
      <div class="info">
        <div class="eyebrow">REPO GALAXY</div>
        <h1>@lukeramos-eli</h1>
        <div class="sub">2 stars · 6 repositories</div>
        <div class="note">Each star is a repository, sized by its stars.</div>
      </div>
      <div class="arms">
        <h4>ARMS</h4>
        <div class="row"><span class="dot" style="background:var(--ts)"></span>TypeScript<span>51%</span></div>
        <div class="row"><span class="dot" style="background:var(--cs)"></span>C#<span>39%</span></div>
        <div class="row"><span class="dot" style="background:var(--html)"></span>HTML<span>9%</span></div>
        <div class="row"><span class="dot" style="background:var(--css)"></span>CSS<span>1%</span></div>
      </div>
    </section>

    <section class="card glow plist">
      <div class="ph"><b>PROJECTS.LIST</b><span>./projects.sh --all</span><span>2 projects</span></div>
      <div class="grid">
        <div class="proj">
          <div class="t"><span>• SF-Booking</span><i></i></div>
          <div class="pb">
            <div><h3>SF-Booking<span class="cur"></span></h3><p>No description provided.</p><span class="tag">TypeScript</span></div>
            <div class="donut"><svg width="88" height="88" viewBox="0 0 88 88"><circle cx="44" cy="44" r="36" fill="none" stroke="#7a52d9" stroke-width="10"/><circle cx="44" cy="44" r="36" fill="none" stroke="#4486cc" stroke-width="10" stroke-dasharray="131.2 226.2"/></svg><em>58%</em></div>
            <div class="meta"><b>★ 2</b>updated 3mo ago</div>
          </div>
        </div>
        <div class="proj">
          <div class="t"><span>• BERS-Project</span><i></i></div>
          <div class="pb">
            <div><h3>BERS-Project<span class="cur"></span></h3><p>Barangay Emergency Response System - Windows Forms Desktop Application</p><span class="tag">C#</span></div>
            <div class="donut"><svg width="88" height="88" viewBox="0 0 88 88"><circle cx="44" cy="44" r="36" fill="none" stroke="#e5573a" stroke-width="10"/><circle cx="44" cy="44" r="36" fill="none" stroke="#7a52d9" stroke-width="10" stroke-dasharray="214.9 226.2"/></svg><em>95%</em></div>
            <div class="meta"><b>★ 0</b>updated 4mo ago</div>
          </div>
        </div>
      </div>
    </section>

    <section class="card glow stack">
      <div class="in">
        <div class="sh"><h2>Language Stack</h2><span>&gt; stack.scan<span class="cur"></span></span></div>
        <div class="sd">Repository-weighted technologies</div>
        <div id="langs"></div>
      </div>
    </section>

    <section class="card city">
      <canvas id="city"></canvas>
      <div class="ci">
        <div class="eyebrow">CONTRIBUTION CITY</div>
        <div class="big">258</div>
        <div class="lab">contributions in the last year</div>
        <div class="st">54 active days</div>
        <div class="st">Busiest day: 29</div>
      </div>
      <div class="cf">@lukeramos-eli<small>3D view of the last 53 weeks</small></div>
    </section>

    <section class="card glow foot">
      <div class="in"><a class="gh" href="https://github.com/LukeRamos-Eli"><span class="g">G</span><span><small>GitHub</small><strong>@lukeramos-eli</strong></span></a></div>
    </section>

  </div>
</div>

<script>
const langs=[["TypeScript",51,"#4486cc"],["C#",39,"#7a52d9"],["HTML",9,"#e5573a"],["CSS",1,"#9254c8"],["JavaScript",0,"#f1e05a"]];
const L=document.getElementById("langs");
langs.forEach(([n,p,c])=>{L.insertAdjacentHTML("beforeend",`<div class="lr"><div class="n"><span class="dot" style="background:${c}"></span>${n}</div><div class="p" style="color:${c}">${p}%</div><div class="trk"><div class="fill" data-w="${p}" style="background:${c}"></div></div></div>`)});
requestAnimationFrame(()=>setTimeout(()=>document.querySelectorAll(".fill").forEach(f=>f.style.width=Math.max(+f.dataset.w,3)+"%"),100));

const cv=document.getElementById("gx"),ctx=cv.getContext("2d");
let W,H,dpr;
function size(){dpr=Math.min(devicePixelRatio||1,2);const r=cv.getBoundingClientRect();W=r.width;H=r.height;cv.width=W*dpr;cv.height=H*dpr;ctx.setTransform(dpr,0,0,dpr,0,0)}
size();addEventListener("resize",size);
const arms=[["#4486cc",.51],["#7a52d9",.39],["#e5573a",.09],["#9254c8",.01]];
const pts=[];
for(let i=0;i<900;i++){
  let r=Math.random(),a=0,arm=0;
  for(let k=0;k<arms.length;k++){a+=arms[k][1];if(r<=a){arm=k;break}}
  const t=Math.pow(Math.random(),.75);
  const rad=.08+t*.92;
  const ang=rad*5.2+arm*Math.PI*.5+(Math.random()-.5)*.55;
  pts.push({rad,ang,c:arms[arm][0],s:Math.random()*1.8+.5,al:Math.random()*.6+.3,tw:Math.random()*6});
}
const bg=Array.from({length:140},()=>({x:Math.random(),y:Math.random(),s:Math.random()*1.2+.3,tw:Math.random()*6}));
const repos=[
  {n:"OOPs",st:0,rad:.33,ang:2.9,c:"#4ea0e8",side:"l"},
  {n:"Portfolio",st:0,rad:.3,ang:5.5,c:"#e5573a",side:"r"},
  {n:"BERS-Project",st:0,rad:.5,ang:3.5,c:"#7a52d9",side:"l"},
  {n:"SF-Booking",st:2,rad:.58,ang:.35,c:"#4486cc",side:"r",big:1},
  {n:"LukeRamos-Eli",st:0,rad:.72,ang:2.7,c:"#4ea0e8",side:"l"},
  {n:"",st:0,rad:.9,ang:2.3,c:"#7a52d9",side:"l"}
];
const rm=matchMedia("(prefers-reduced-motion: reduce)").matches;
function pos(rad,ang,rot){
  const R=Math.min(W*.5,H*.62)*rad*1.05,a=ang+rot;
  const narrow=W<720;
  const cx=narrow?W*.5:W*.64, cy=narrow?H*.62:H*.52;
  return [cx+Math.cos(a)*R*(narrow?.9:1.25),cy+Math.sin(a)*R*.78];
}
function frame(ms){
  const t=ms/1000,rot=rm?0:t*.06;
  ctx.clearRect(0,0,W,H);
  bg.forEach(b=>{ctx.globalAlpha=.25+.35*Math.abs(Math.sin(t*.8+b.tw));ctx.fillStyle="#aab";ctx.fillRect(b.x*W,b.y*H,b.s,b.s)});
  pts.forEach(p=>{const[x,y]=pos(p.rad,p.ang,rot*(1.4-p.rad*.8));ctx.globalAlpha=p.al*(.7+.3*Math.sin(t+p.tw));ctx.fillStyle=p.c;ctx.beginPath();ctx.arc(x,y,p.s,0,6.283);ctx.fill()});
  const[cx,cy]=pos(0,0,0);
  ctx.globalAlpha=.14;ctx.fillStyle="#8fa0ff";ctx.beginPath();ctx.ellipse(cx,cy,58,30,0,0,6.283);ctx.fill();
  ctx.globalAlpha=.3;ctx.beginPath();ctx.ellipse(cx,cy,24,13,0,0,6.283);ctx.fill();
  ctx.globalAlpha=1;ctx.fillStyle="#fff";ctx.beginPath();ctx.arc(cx,cy,4.5,0,6.283);ctx.fill();
  const small=W<720;
  repos.forEach(r=>{
    const[x,y]=pos(r.rad,r.ang,rot*(1.4-r.rad*.8));
    const rr=r.big?10:4;
    if(r.big){ctx.globalAlpha=.22;ctx.fillStyle="#4486cc";ctx.beginPath();ctx.arc(x,y,24,0,6.283);ctx.fill()}
    ctx.globalAlpha=.25;ctx.fillStyle=r.c;ctx.beginPath();ctx.arc(x,y,rr+6,0,6.283);ctx.fill();
    ctx.globalAlpha=1;ctx.fillStyle=r.c;ctx.beginPath();ctx.arc(x,y,rr,0,6.283);ctx.fill();
    ctx.fillStyle="#fff";ctx.beginPath();ctx.arc(x,y,rr*.35,0,6.283);ctx.fill();
    if(r.n){
      ctx.font=`700 ${small?11:13}px system-ui,sans-serif`;
      const txt=r.n+" ★ "+r.st,w=ctx.measureText(txt).width,off=rr+10;
      ctx.fillStyle="#eef";ctx.textBaseline="middle";
      ctx.fillText(r.n,r.side==="r"?x+off:x-off-w,y);
      const nw=ctx.measureText(r.n+" ").width;
      ctx.fillStyle="#9aa3ff";ctx.fillText("★ "+r.st,(r.side==="r"?x+off:x-off-w)+nw,y);
    }
  });
  requestAnimationFrame(frame);
}
requestAnimationFrame(frame);

/* Contribution City */
(function(){
  const c=document.getElementById("city"),x=c.getContext("2d");
  let seed=7;const rnd=()=>(seed=(seed*16807)%2147483647)/2147483647;
  const WK=53,DY=7,cells=[];
  for(let w=0;w<WK;w++)for(let d=0;d<DY;d++)cells.push({w,d,n:0});
  const pick=[];
  while(pick.length<54){
    const recent=rnd()<.82;
    const w=recent?Math.floor(WK-1-Math.pow(rnd(),1.7)*16):Math.floor(rnd()*(WK-16));
    const d=Math.floor(rnd()*7),k=w*7+d;
    if(!pick.includes(k))pick.push(k);
  }
  const wts=pick.map((_,i)=>i===0?0:Math.pow(rnd(),2.2)+.04);
  const tot=wts.reduce((a,b)=>a+b,0);
  let vals=wts.map((v,i)=>i===0?29:Math.max(1,Math.min(26,Math.round(v/tot*229))));
  let diff=258-vals.reduce((a,b)=>a+b,0),i=1;
  while(diff!==0){const s=diff>0?1:-1;if(vals[i]+s>=1&&vals[i]+s<=26){vals[i]+=s;diff-=s}i=i%(vals.length-1)+1}
  pick.forEach((k,j)=>cells[k].n=vals[j]);
  cells[pick[0]].n=29;
  let W,H,dpr,t0=performance.now();
  function size(){dpr=Math.min(devicePixelRatio||1,2);const r=c.getBoundingClientRect();W=r.width;H=r.height;c.width=W*dpr;c.height=H*dpr;x.setTransform(dpr,0,0,dpr,0,0)}
  function poly(pts,f){x.fillStyle=f;x.beginPath();pts.forEach(([a,b],i)=>i?x.lineTo(a,b):x.moveTo(a,b));x.closePath();x.fill()}
  function draw(now){
    const p=Math.min(1,(now-t0)/1500),e=1-Math.pow(1-p,3);
    x.clearRect(0,0,W,H);
    const narrow=W<720,span=(WK-1+6)*.866*2;
    const s=narrow?(W-40)/span*1.0:Math.min((W*.62)/(span/2*1.0)/1,(H-60)/((WK+6)*.5+10));
    const sc=narrow?s:Math.min(s,W*.62/((WK+5)*.866));
    const dx=sc*.866,dy=sc*.5;
    const ox=narrow?W*.12+6*dx:W*.3+6*dx,oy=narrow?H*.34:H*.2;
    const zs=sc*.62;
    for(let w=0;w<WK;w++)for(let d=0;d<DY;d++){
      const cell=cells[w*7+d],h=2+(cell.n?(3+cell.n*1.9):0)*e*zs/ sc*sc*.5*1;
      const X=ox+(w-d)*dx,Y=oy+(w+d)*dy;
      const n=cell.n,tier=n===0?0:n<4?1:n<10?2:3;
      const top=["#2a2f78","#4486cc","#7a52d9","#b9a8ff"][tier];
      const lf=["#1f2360","#336aa3","#5f3fb0","#8f7fd0"][tier];
      const rt=["#181b4d","#295585","#4c3290","#7567ab"][tier];
      const yt=Y-h;
      poly([[X-dx,yt],[X,yt+dy],[X,Y+dy],[X-dx,Y]],lf);
      poly([[X+dx,yt],[X,yt+dy],[X,Y+dy],[X+dx,Y]],rt);
      poly([[X,yt-dy],[X+dx,yt],[X,yt+dy],[X-dx,yt]],top);
      x.strokeStyle="#0a0c2a";x.lineWidth=.6;x.beginPath();x.moveTo(X-dx,yt);x.lineTo(X,yt-dy);x.lineTo(X+dx,yt);x.lineTo(X,yt+dy);x.closePath();x.stroke();
    }
    if(p<1)requestAnimationFrame(draw);
  }
  function start(){size();t0=performance.now();requestAnimationFrame(draw)}
  start();addEventListener("resize",()=>{size();requestAnimationFrame(draw);t0=-1e9});
})();
</script>
</body>
</html>
