<!DOCTYPE html>
<html lang="ja">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>呼吸と身体のビジュアルガイド｜吹奏楽</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Zen+Kaku+Gothic+New:wght@400;500;700;900&family=Archivo:wght@600;700&display=swap" rel="stylesheet">
<style>
  :root{
    --bg:#0d2630;
    --bg2:#123540;
    --bg3:#0a1d25;
    --panel:#16424f;
    --brass:#e6a93f;
    --brass-d:#b87d22;
    --breath:#6fd6e6;
    --breath-soft:rgba(111,214,230,.16);
    --coral:#e89178;
    --coral-d:#c46a52;
    --text:#e9f4f4;
    --muted:#8aabb3;
    --line:rgba(255,255,255,.09);
    --good:#7fd6a8;
    --warn:#e8916f;
    --jp:"Zen Kaku Gothic New","Hiragino Kaku Gothic ProN","Yu Gothic",-apple-system,sans-serif;
    --en:"Archivo",var(--jp);
  }
  *{box-sizing:border-box;margin:0;padding:0}
  html{-webkit-text-size-adjust:100%}
  body{
    font-family:var(--jp);
    background:
      radial-gradient(1200px 600px at 78% -10%, rgba(230,169,63,.10), transparent 60%),
      radial-gradient(900px 700px at 10% 110%, rgba(111,214,230,.10), transparent 55%),
      var(--bg);
    color:var(--text);
    line-height:1.7;
    min-height:100vh;
  }
  .wrap{max-width:1080px;margin:0 auto;padding:28px 22px 64px}

  /* header */
  header{margin-bottom:26px}
  .eyebrow{
    font-family:var(--en);font-weight:700;letter-spacing:.32em;
    text-transform:uppercase;font-size:12px;color:var(--brass);
    display:flex;align-items:center;gap:12px;
  }
  .eyebrow::after{content:"";flex:1;height:1px;background:linear-gradient(90deg,var(--brass-d),transparent)}
  h1{
    font-weight:900;font-size:clamp(28px,4.5vw,46px);line-height:1.15;
    margin:14px 0 8px;letter-spacing:.01em;
  }
  h1 .breathe{color:var(--breath)}
  .lead{color:var(--muted);max-width:52ch;font-size:15px}

  /* tabs */
  .tabs{
    display:flex;gap:8px;margin:26px 0 22px;flex-wrap:wrap;
    border-bottom:1px solid var(--line);padding-bottom:0;
  }
  .tab{
    appearance:none;border:0;background:transparent;color:var(--muted);
    font-family:var(--jp);font-weight:700;font-size:15px;cursor:pointer;
    padding:12px 16px 14px;position:relative;border-radius:10px 10px 0 0;
    transition:color .18s, background .18s;display:flex;align-items:center;gap:9px;
  }
  .tab .ic{width:20px;height:20px;display:inline-block;flex:none}
  .tab:hover{color:var(--text);background:rgba(255,255,255,.03)}
  .tab[aria-selected="true"]{color:var(--text)}
  .tab[aria-selected="true"]::after{
    content:"";position:absolute;left:10px;right:10px;bottom:-1px;height:3px;
    background:linear-gradient(90deg,var(--brass),var(--breath));border-radius:3px;
  }
  .tab:focus-visible{outline:2px solid var(--breath);outline-offset:2px}

  /* panels */
  .panel{display:none}
  .panel.active{display:block;animation:fade .35s ease}
  @keyframes fade{from{opacity:0;transform:translateY(6px)}to{opacity:1;transform:none}}

  .stage-grid{display:grid;grid-template-columns:1.45fr 1fr;gap:20px;align-items:stretch}
  @media(max-width:780px){.stage-grid{grid-template-columns:1fr}}

  .stage{
    position:relative;background:linear-gradient(180deg,var(--bg2),var(--bg3));
    border:1px solid var(--line);border-radius:18px;overflow:hidden;
    min-height:360px;display:flex;align-items:center;justify-content:center;
  }
  .stage canvas, .stage svg{display:block;width:100%;height:100%}
  .stage .tag{
    position:absolute;top:14px;left:14px;font-family:var(--en);font-weight:700;
    font-size:11px;letter-spacing:.22em;text-transform:uppercase;
    color:var(--breath);background:rgba(13,38,48,.7);
    padding:5px 10px;border-radius:999px;border:1px solid var(--line);
  }

  .side{display:flex;flex-direction:column;gap:16px}
  .card{
    background:var(--panel);border:1px solid var(--line);border-radius:16px;
    padding:18px 18px 20px;
  }
  .card h3{font-size:16px;font-weight:900;margin-bottom:6px;display:flex;align-items:center;gap:8px}
  .card h3 .dot{width:9px;height:9px;border-radius:50%;background:var(--brass);flex:none}
  .card p{font-size:14px;color:var(--muted)}
  .card p b{color:var(--text);font-weight:700}

  /* controls */
  .ctrl{margin-top:6px}
  .ctrl + .ctrl{margin-top:16px}
  .ctrl label{display:flex;justify-content:space-between;font-size:13px;font-weight:700;margin-bottom:7px}
  .ctrl label span{color:var(--breath);font-family:var(--en)}
  input[type=range]{
    -webkit-appearance:none;appearance:none;width:100%;height:6px;border-radius:6px;
    background:linear-gradient(90deg,var(--brass) 0%,var(--brass) var(--p,50%),rgba(255,255,255,.12) var(--p,50%));
    outline:none;cursor:pointer;
  }
  input[type=range]::-webkit-slider-thumb{
    -webkit-appearance:none;width:20px;height:20px;border-radius:50%;
    background:#fff;border:3px solid var(--brass-d);box-shadow:0 2px 6px rgba(0,0,0,.4);cursor:pointer;
  }
  input[type=range]::-moz-range-thumb{
    width:18px;height:18px;border-radius:50%;background:#fff;border:3px solid var(--brass-d);cursor:pointer;
  }
  input[type=range]:focus-visible{outline:2px solid var(--breath);outline-offset:3px}

  .presets{display:flex;flex-wrap:wrap;gap:8px;margin-top:4px}
  .chip{
    appearance:none;border:1px solid var(--line);background:rgba(255,255,255,.03);
    color:var(--text);font-family:var(--jp);font-weight:700;font-size:13px;
    padding:8px 13px;border-radius:999px;cursor:pointer;transition:.16s;
  }
  .chip:hover{border-color:var(--brass);color:var(--brass)}
  .chip.on{background:var(--brass);color:#1a1206;border-color:var(--brass)}
  .chip:focus-visible{outline:2px solid var(--breath);outline-offset:2px}

  .toggle{display:flex;background:rgba(0,0,0,.25);border-radius:12px;padding:4px;gap:4px}
  .toggle button{
    flex:1;appearance:none;border:0;background:transparent;color:var(--muted);
    font-family:var(--jp);font-weight:700;font-size:14px;padding:9px;border-radius:9px;cursor:pointer;transition:.16s;
  }
  .toggle button.on{background:var(--panel);color:var(--text);box-shadow:0 1px 0 rgba(255,255,255,.06) inset}
  .toggle button:focus-visible{outline:2px solid var(--breath);outline-offset:2px}

  .hint{font-size:13px;color:var(--muted);border-left:3px solid var(--brass);padding:2px 0 2px 12px;margin-top:4px}
  .hint b{color:var(--coral)}

  footer{margin-top:34px;color:var(--muted);font-size:13px;text-align:center;border-top:1px solid var(--line);padding-top:20px}
  footer b{color:var(--brass)}

  @media (prefers-reduced-motion: reduce){
    *{animation-duration:.001s !important}
  }
</style>
</head>
<body>
<div class="wrap">
  <header>
    <div class="eyebrow">Brass Band · Body &amp; Breath</div>
    <h1>目に見えない<span class="breathe">息と身体</span>を、<br>見えるようにする。</h1>
    <p class="lead">「お腹で支えて」「口の中を広げて」——言葉だけだと伝わりにくい身体の使い方を、動かしながらイメージできるガイドです。4つのテーマを切り替えて使ってね。</p>
  </header>

  <div class="tabs" role="tablist" aria-label="テーマ切り替え">
    <button class="tab" role="tab" aria-selected="true" data-mode="breath">
      <svg class="ic" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round"><path d="M4 14c4 0 4-4 8-4s4 4 8 4"/><path d="M4 18c4 0 4-3 8-3s4 3 8 3"/></svg>
      息の流れ
    </button>
    <button class="tab" role="tab" aria-selected="false" data-mode="mouth">
      <svg class="ic" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="12" cy="12" r="9"/><path d="M8 13c1.5 2 6.5 2 8 0" stroke-linecap="round"/></svg>
      口の中の空間
    </button>
    <button class="tab" role="tab" aria-selected="false" data-mode="lungs">
      <svg class="ic" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round"><path d="M12 3v8"/><path d="M12 11c0 6-3 9-5 9s-2-5-2-7 2-5 4-5"/><path d="M12 11c0 6 3 9 5 9s2-5 2-7-2-5-4-5"/></svg>
      肺と呼吸筋
    </button>
    <button class="tab" role="tab" aria-selected="false" data-mode="posture">
      <svg class="ic" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round"><circle cx="12" cy="5" r="2.5"/><path d="M12 8v8m0 0-3 5m3-5 3 5M8 11h8"/></svg>
      姿勢と通り道
    </button>
  </div>

  <!-- ============ BREATH ============ -->
  <section class="panel active" id="p-breath" role="tabpanel">
    <div class="stage-grid">
      <div class="stage">
        <span class="tag">Air Flow</span>
        <canvas id="breathCanvas"></canvas>
      </div>
      <div class="side">
        <div class="card">
          <h3><span class="dot"></span>息は「速さ」と「太さ」でできてる</h3>
          <p>同じ「フー」でも、唇のすき間(アパチュア)と支えで流れが大きく変わるよ。スライダーで粒の動きが変わるのを見てみて。</p>
        </div>
        <div class="card">
          <div class="ctrl">
            <label>唇のすき間（アパチュア）<span id="vAp">ふつう</span></label>
            <input type="range" id="ap" min="1" max="10" value="5">
          </div>
          <div class="ctrl">
            <label>息の速さ<span id="vSp">ふつう</span></label>
            <input type="range" id="sp" min="1" max="10" value="5">
          </div>
          <div class="ctrl">
            <label>お腹の支え（息の量）<span id="vSu">ふつう</span></label>
            <input type="range" id="su" min="1" max="10" value="5">
          </div>
          <div class="presets" style="margin-top:16px" id="breathPresets">
            <button class="chip" data-ap="2" data-sp="8" data-su="6">高音（細く速く）</button>
            <button class="chip" data-ap="8" data-sp="3" data-su="9">低音・ロングトーン</button>
            <button class="chip" data-ap="4" data-sp="9" data-su="5">タンギング</button>
          </div>
        </div>
        <p class="hint">粒が<b>まっすぐ遠くまで</b>飛ぶほど、支えのある息。バラけてすぐ落ちる息は、のどで止まりがちのサインだよ。</p>
      </div>
    </div>
  </section>

  <!-- ============ MOUTH ============ -->
  <section class="panel" id="p-mouth" role="tabpanel">
    <div class="stage-grid">
      <div class="stage">
        <span class="tag">Oral Space</span>
        <svg id="mouthSvg" viewBox="0 0 460 360" preserveAspectRatio="xMidYMid meet"></svg>
      </div>
      <div class="side">
        <div class="card">
          <h3><span class="dot"></span>口の中に「響く部屋」を作る</h3>
          <p>音は口の中の空間で響くよ。あくびの直前みたいに<b>奥を縦に広げる</b>と、部屋が大きくなって響きが増える。スライダーで空間の広さを変えてみて。</p>
        </div>
        <div class="card">
          <div class="ctrl">
            <label>口の中の広さ<span id="vOpen">ふつう</span></label>
            <input type="range" id="open" min="0" max="10" value="4">
          </div>
          <div class="presets" style="margin-top:16px" id="mouthPresets">
            <button class="chip" data-open="1">「イ」せまい</button>
            <button class="chip" data-open="5">「オ」ふつう</button>
            <button class="chip" data-open="9">あくびの喉</button>
          </div>
        </div>
        <p class="hint">広げるのは<b>口先より奥（のどの上）</b>。口先を開きすぎると音が散るので、奥の縦じわをイメージしてね。</p>
      </div>
    </div>
  </section>

  <!-- ============ LUNGS ============ -->
  <section class="panel" id="p-lungs" role="tabpanel">
    <div class="stage-grid">
      <div class="stage">
        <span class="tag">Lungs &amp; Muscles</span>
        <svg id="lungSvg" viewBox="0 0 420 420" preserveAspectRatio="xMidYMid meet"></svg>
      </div>
      <div class="side">
        <div class="card">
          <h3><span class="dot"></span>肺じゃなく「まわりの筋肉」で動かす</h3>
          <p>肺そのものに筋肉はないよ。胴体を<b>360°ぐるっと</b>取り巻く筋肉（横隔膜・お腹・背中・脇腹）で広げたり支えたりするイメージ。リングが全周ふくらむのを見てね。</p>
        </div>
        <div class="card">
          <div class="toggle" id="lungToggle">
            <button class="on" data-auto="1">自動で呼吸</button>
            <button data-auto="0">手で動かす</button>
          </div>
          <div class="ctrl" id="lungManual" style="opacity:.4;pointer-events:none;margin-top:16px">
            <label>息を吸う量<span id="vInh">—</span></label>
            <input type="range" id="inh" min="0" max="10" value="3">
          </div>
        </div>
        <p class="hint">背中側もふくらむのがポイント。<b>前だけ</b>ふくらませると、すぐ息が足りなくなるよ。</p>
      </div>
    </div>
  </section>

  <!-- ============ POSTURE ============ -->
  <section class="panel" id="p-posture" role="tabpanel">
    <div class="stage-grid">
      <div class="stage">
        <span class="tag">Air Path</span>
        <svg id="postureSvg" viewBox="0 0 420 420" preserveAspectRatio="xMidYMid meet"></svg>
      </div>
      <div class="side">
        <div class="card">
          <h3><span class="dot"></span>空気の通り道を、折り曲げない</h3>
          <p>猫背であごが落ちると、のど〜気管が折れて空気が通りにくくなるよ。スライダーを動かして、<b>通り道がまっすぐ</b>になる姿勢をさがしてみて。</p>
        </div>
        <div class="card">
          <div class="ctrl">
            <label>姿勢<span id="vPos">—</span></label>
            <input type="range" id="pos" min="0" max="10" value="2">
          </div>
          <div class="presets" style="margin-top:16px" id="posturePresets">
            <button class="chip" data-pos="9">猫背・あご引き</button>
            <button class="chip" data-pos="2">まっすぐ・通る</button>
            <button class="chip" data-pos="0">あご上げすぎ</button>
          </div>
        </div>
        <p class="hint">頭のてっぺんを<b>糸で軽く吊られる</b>イメージ。あご上げすぎ・下げすぎは<b style="color:var(--warn)">どちらものどに力が入る</b>ので、真ん中が一番ラクに響くよ。</p>
      </div>
    </div>
  </section>

  <footer>
    機能① <b>息・身体の可視化</b> プロトタイプ ／ 吹奏楽部向けWebアプリ ・ 気になるところは遠慮なく言ってね
  </footer>
</div>

<script>
const reduce = window.matchMedia('(prefers-reduced-motion: reduce)').matches;
let mode = 'breath';

/* ---------- tabs ---------- */
const tabs=[...document.querySelectorAll('.tab')];
const panels={breath:'p-breath',mouth:'p-mouth',lungs:'p-lungs',posture:'p-posture'};
tabs.forEach(t=>t.addEventListener('click',()=>{
  tabs.forEach(x=>x.setAttribute('aria-selected', x===t));
  Object.values(panels).forEach(id=>document.getElementById(id).classList.remove('active'));
  mode=t.dataset.mode;
  document.getElementById(panels[mode]).classList.add('active');
  if(mode==='breath') sizeBreath();
}));

/* slider fill helper */
function fill(el){const min=+el.min,max=+el.max;el.style.setProperty('--p',((el.value-min)/(max-min)*100)+'%');}
document.querySelectorAll('input[type=range]').forEach(r=>{fill(r);r.addEventListener('input',()=>fill(r));});

/* ============ BREATH (canvas) ============ */
const bc=document.getElementById('breathCanvas');
const bx=bc.getContext('2d');
let bw,bh,particles=[];
function sizeBreath(){
  const r=bc.parentElement.getBoundingClientRect();
  bw=bc.width=r.width*devicePixelRatio; bh=bc.height=r.height*devicePixelRatio;
  bx.setTransform(devicePixelRatio,0,0,devicePixelRatio,0,0);
  bw=r.width; bh=r.height;
}
window.addEventListener('resize',()=>{if(mode==='breath')sizeBreath();});
const apEl=document.getElementById('ap'),spEl=document.getElementById('sp'),suEl=document.getElementById('su');
const word=v=>v<=3?'せまい':v<=6?'ふつう':'広い';
const wordSp=v=>v<=3?'ゆっくり':v<=6?'ふつう':'速い';
const wordSu=v=>v<=3?'弱い':v<=6?'ふつう':'強い';
function updBreathLabels(){
  document.getElementById('vAp').textContent=word(+apEl.value);
  document.getElementById('vSp').textContent=wordSp(+spEl.value);
  document.getElementById('vSu').textContent=wordSu(+suEl.value);
}
[apEl,spEl,suEl].forEach(e=>e.addEventListener('input',updBreathLabels));updBreathLabels();
document.querySelectorAll('#breathPresets .chip').forEach(c=>c.addEventListener('click',()=>{
  document.querySelectorAll('#breathPresets .chip').forEach(x=>x.classList.remove('on'));
  c.classList.add('on');
  apEl.value=c.dataset.ap;spEl.value=c.dataset.sp;suEl.value=c.dataset.su;
  [apEl,spEl,suEl].forEach(fill);updBreathLabels();
}));
// 口の位置・スケール・唇のすき間(アパチュア連動)をまとめて返す共通関数
function mouthPoint(){
  const s=Math.min(bw,bh)/360;
  const mx=bw*0.22, my=bh*0.52;       // 唇の合わせ目あたり
  const ap=+apEl.value;
  const gap=(2.5+ap*2.1)*s;           // 唇のすき間：アパチュアが大きいほど開く
  return {mx,my,s,gap};
}
function spawn(){
  const sp=+spEl.value, su=+suEl.value;
  const {mx,my,s,gap}=mouthPoint();
  const ox=mx+42*s, oy=my;            // 息の出口＝唇の先端
  const speed=(0.6+sp*0.32);          // 速さ
  const n=Math.round(1+su*0.4);       // 支え→量
  for(let i=0;i<n;i++){
    particles.push({
      x:ox, y:oy+(Math.random()-0.5)*gap*1.05,   // すき間の幅から出る
      vx:speed*(0.8+Math.random()*0.5),
      vy:(Math.random()-0.5)*(0.22+gap*0.012),
      r:1.4+Math.random()*(1+su*0.18),
      a:0, life:0, max:90+Math.random()*60,
      decay:0.55+ (10-su)*0.04        // 支え弱い→早く落ちる
    });
  }
}
function drawFace(){
  const {mx,my,s,gap}=mouthPoint();
  bx.save();
  bx.lineJoin='round';bx.lineCap='round';
  // --- 顔シルエット（右向き横顔・肌グラデ塗り） ---
  bx.beginPath();
  bx.moveTo(mx-18*s, my-120*s);
  bx.bezierCurveTo(mx+20*s,my-133*s, mx+42*s,my-112*s, mx+37*s,my-78*s);
  bx.bezierCurveTo(mx+34*s,my-70*s, mx+33*s,my-60*s, mx+40*s,my-46*s);
  bx.bezierCurveTo(mx+54*s,my-40*s, mx+62*s,my-33*s, mx+59*s,my-25*s);
  bx.bezierCurveTo(mx+56*s,my-19*s, mx+48*s,my-19*s, mx+41*s,my-15*s);
  bx.bezierCurveTo(mx+45*s,my-9*s, mx+45*s,my-6*s, mx+42*s,my-2*s);
  bx.lineTo(mx+41*s, my+13*s);
  bx.bezierCurveTo(mx+46*s,my+27*s, mx+47*s,my+41*s, mx+34*s,my+53*s);
  bx.bezierCurveTo(mx+23*s,my+65*s, mx+15*s,my+80*s, mx+11*s,my+99*s);
  bx.lineTo(mx-32*s, my+99*s);
  bx.bezierCurveTo(mx-60*s,my+72*s, mx-75*s,my+36*s, mx-73*s,my-10*s);
  bx.bezierCurveTo(mx-71*s,my-62*s, mx-50*s,my-105*s, mx-18*s,my-120*s);
  bx.closePath();
  const skin=bx.createLinearGradient(mx,my-120*s,mx,my+99*s);
  skin.addColorStop(0,'#f3cba3');skin.addColorStop(1,'#d99e72');
  bx.fillStyle=skin;bx.fill();
  bx.lineWidth=2.2;bx.strokeStyle='#c98a63';bx.stroke();
  // --- 髪 ---
  bx.beginPath();
  bx.moveTo(mx-73*s,my-12*s);
  bx.bezierCurveTo(mx-74*s,my-82*s, mx-42*s,my-130*s, mx-4*s,my-130*s);
  bx.bezierCurveTo(mx+24*s,my-130*s, mx+40*s,my-108*s, mx+39*s,my-84*s);
  bx.bezierCurveTo(mx+30*s,my-100*s, mx+4*s,my-104*s, mx-8*s,my-92*s);
  bx.bezierCurveTo(mx-32*s,my-72*s, mx-54*s,my-44*s, mx-60*s,my-12*s);
  bx.closePath();
  bx.fillStyle='#3a2c22';bx.fill();
  // --- 頬の赤み ---
  const cg=bx.createRadialGradient(mx+28*s,my-24*s,2,mx+28*s,my-24*s,26*s);
  cg.addColorStop(0,'rgba(231,138,118,.45)');cg.addColorStop(1,'rgba(231,138,118,0)');
  bx.fillStyle=cg;bx.beginPath();bx.ellipse(mx+28*s,my-24*s,24*s,17*s,0,0,Math.PI*2);bx.fill();
  // --- 耳 ---
  bx.beginPath();bx.ellipse(mx-31*s,my-4*s,8*s,12*s,0,0,Math.PI*2);
  bx.fillStyle='#e7b187';bx.fill();bx.lineWidth=1.6;bx.strokeStyle='#c98a63';bx.stroke();
  // --- 眉・目（横顔） ---
  bx.beginPath();bx.moveTo(mx+9*s,my-74*s);bx.quadraticCurveTo(mx+22*s,my-80*s,mx+34*s,my-72*s);
  bx.lineWidth=3.2;bx.strokeStyle='#5a4634';bx.stroke();
  bx.beginPath();bx.ellipse(mx+23*s,my-62*s,8*s,5*s,0,0,Math.PI*2);bx.fillStyle='#fbf7ef';bx.fill();
  bx.beginPath();bx.arc(mx+27*s,my-62*s,3.4*s,0,Math.PI*2);bx.fillStyle='#5a3a24';bx.fill();
  bx.beginPath();bx.arc(mx+27*s,my-62*s,1.6*s,0,Math.PI*2);bx.fillStyle='#1c120a';bx.fill();
  bx.beginPath();bx.moveTo(mx+15*s,my-64*s);bx.quadraticCurveTo(mx+23*s,my-69*s,mx+32*s,my-63*s);
  bx.lineWidth=2;bx.strokeStyle='#3a2c22';bx.stroke();
  // --- 鼻孔の影 ---
  bx.beginPath();bx.ellipse(mx+49*s,my-18*s,3.2*s,2*s,0,0,Math.PI*2);bx.fillStyle='#bd7f57';bx.fill();
  // --- 口の中（すき間の奥）---
  bx.beginPath();bx.ellipse(mx+30*s,my,10*s,Math.max(1,gap*0.55),0,0,Math.PI*2);
  bx.fillStyle='#5c2420';bx.fill();
  // --- 唇（ふっくら・アパチュア連動）---
  const lg=bx.createLinearGradient(mx,my-8*s,mx,my+13*s);
  lg.addColorStop(0,'#e08b78');lg.addColorStop(1,'#c96a5a');
  bx.fillStyle=lg;bx.lineWidth=1;bx.strokeStyle='#b85f50';
  bx.beginPath();                                    // 上唇
  bx.moveTo(mx+9*s,my-3*s);
  bx.quadraticCurveTo(mx+28*s,my-9*s,mx+44*s,my-2*s);
  bx.quadraticCurveTo(mx+30*s,my-gap*0.5,mx+12*s,my-1*s);
  bx.closePath();bx.fill();bx.stroke();
  bx.beginPath();                                    // 下唇
  bx.moveTo(mx+11*s,my+2*s);
  bx.quadraticCurveTo(mx+30*s,my+gap*0.5,mx+43*s,my+2*s);
  bx.quadraticCurveTo(mx+28*s,my+14*s,mx+10*s,my+6*s);
  bx.closePath();bx.fill();bx.stroke();
  bx.restore();
}
let bt=0;
function breathLoop(){
  if(mode==='breath'){
    bx.clearRect(0,0,bw,bh);
    drawFace();
    if(!reduce){ bt++; if(bt%2===0) spawn(); }
    else if(particles.length<40) spawn();
    for(let i=particles.length-1;i>=0;i--){
      const p=particles[i];
      p.life++; p.x+=p.vx; p.y+=p.vy; p.vy+=0.004; p.vx*=0.995;
      p.a = p.life<10 ? p.life/10 : Math.max(0,1-(p.life/p.max)*p.decay);
      if(p.a<=0||p.x>bw+10){particles.splice(i,1);continue;}
      bx.beginPath();
      bx.fillStyle=`rgba(111,214,230,${p.a*0.8})`;
      bx.arc(p.x,p.y,p.r,0,7);bx.fill();
    }
  }
  requestAnimationFrame(breathLoop);
}

/* ============ MOUTH (svg) ============ */
const ms=document.getElementById('mouthSvg');
const openEl=document.getElementById('open');
function buildMouth(){
  ms.innerHTML=`
    <defs>
      <radialGradient id="skinGrad" cx="62%" cy="42%" r="62%">
        <stop offset="0%" stop-color="#f2c8a0"/><stop offset="70%" stop-color="#e7b187"/><stop offset="100%" stop-color="#d79a6e"/>
      </radialGradient>
      <radialGradient id="cheekGrad" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stop-color="rgba(231,140,118,.5)"/><stop offset="100%" stop-color="rgba(231,140,118,0)"/>
      </radialGradient>
      <linearGradient id="lipGrad" x1="0" y1="0" x2="0" y2="1">
        <stop offset="0%" stop-color="#e08b78"/><stop offset="100%" stop-color="#c96a5a"/>
      </linearGradient>
      <radialGradient id="throatGrad" cx="50%" cy="40%" r="70%">
        <stop offset="0%" stop-color="#5c2420"/><stop offset="100%" stop-color="#2c0f0d"/>
      </radialGradient>
    </defs>
    <text x="200" y="26" text-anchor="middle" fill="var(--text)" font-size="14" font-family="var(--jp)" font-weight="700">口の中（横から見た断面）</text>

    <!-- 髪（後ろ） -->
    <path d="M150 60 Q120 130 126 200 L150 210 Q138 130 175 80 Q205 52 240 50 Q280 48 312 70
             Q300 50 250 44 Q190 42 150 60 Z" fill="#3a2c22"/>

    <!-- 顔ベース（肌・人間の横顔） -->
    <path d="M232 48
             C284 44 320 68 327 104 C331 120 321 126 325 137
             C332 147 349 154 362 168 C364 176 354 181 343 183
             C347 191 348 199 345 207 C351 221 353 237 345 253
             C335 269 315 279 297 287 L297 322 L150 322
             C122 272 130 206 127 178 C116 134 150 74 200 52 Z"
          fill="url(#skinGrad)" stroke="#c98a63" stroke-width="2"/>

    <!-- 頬の赤み -->
    <ellipse cx="312" cy="172" rx="26" ry="18" fill="url(#cheekGrad)"/>
    <!-- 耳 -->
    <path d="M168 158 Q156 156 158 172 Q160 186 174 184 Q168 172 172 160 Z" fill="url(#skinGrad)" stroke="#c98a63" stroke-width="1.5"/>
    <!-- 前髪 -->
    <path d="M232 48 C200 54 172 78 162 110 Q186 80 226 72 Q300 64 326 102 C322 70 286 46 232 48 Z" fill="#33271e"/>

    <!-- 眉 -->
    <path d="M286 112 Q300 107 317 114" fill="none" stroke="#5a4634" stroke-width="3.4" stroke-linecap="round"/>
    <!-- 目 -->
    <ellipse cx="302" cy="129" rx="13" ry="6.5" fill="#fbf7ef"/>
    <circle cx="307" cy="129" r="5.2" fill="#6b4a30"/><circle cx="307" cy="129" r="2.3" fill="#241a12"/>
    <path d="M289 127 Q302 121 315 128" fill="none" stroke="#3a2c22" stroke-width="2.2" stroke-linecap="round"/>
    <!-- 鼻孔の影 -->
    <ellipse cx="347" cy="177" rx="4" ry="2.2" fill="#b97f5b"/>

    <!-- ===== 口の中（開口部の奥） ===== -->
    <!-- のど -->
    <path id="throat" d="M214 158 Q204 214 216 276 L246 276 Q238 214 244 166 Z" fill="url(#throatGrad)" stroke="#7a3a30" stroke-width="1.5"/>
    <!-- 響く空間（可変ハイライト） -->
    <ellipse id="cavity" cx="288" cy="188" rx="52" ry="17" fill="rgba(111,214,230,.20)" stroke="var(--breath)" stroke-width="2" stroke-opacity=".7"/>
    <circle id="wave1" cx="288" cy="188" r="14" fill="none" stroke="var(--breath)" stroke-width="2" opacity="0"/>
    <circle id="wave2" cx="288" cy="188" r="14" fill="none" stroke="var(--breath)" stroke-width="2" opacity="0"/>
    <!-- 上あご（硬口蓋） -->
    <path id="palate" d="M240 164 Q294 154 340 166" fill="none" stroke="#e0a48f" stroke-width="7" stroke-linecap="round"/>
    <!-- 軟口蓋（可変） -->
    <path id="soft" d="M240 164 Q226 182 232 196" fill="none" stroke="#d2806c" stroke-width="6" stroke-linecap="round"/>
    <!-- 上の歯 -->
    <rect x="332" y="166" width="11" height="15" rx="2.5" fill="#fbf8ee" stroke="#d8d0bc" stroke-width="1"/>

    <!-- 下あごユニット（可変：広げると下がる） -->
    <g id="lowerJaw">
      <path id="tongue" d="" fill="#cd6e58" stroke="#a94f3a" stroke-width="1.5"/>
      <path d="M250 214 Q294 224 332 212" fill="none" stroke="#b85741" stroke-width="1.5" opacity=".6"/>
      <rect id="lowtooth" x="332" y="200" width="11" height="15" rx="2.5" fill="#fbf8ee" stroke="#d8d0bc" stroke-width="1"/>
    </g>

    <!-- 唇（ふっくら） -->
    <path id="uplip" d="M328 186 Q344 180 354 188 Q347 196 330 195 Z" fill="url(#lipGrad)" stroke="#b85f50" stroke-width="1"/>
    <path id="lowlip" d="M330 206 Q346 202 353 208 Q346 218 329 213 Z" fill="url(#lipGrad)" stroke="#b85f50" stroke-width="1"/>

    <!-- ラベル -->
    <g font-family="var(--jp)" font-size="12">
      <text x="252" y="150" fill="#e0a48f">上あご</text>
      <text x="250" y="258" fill="#e0907a">舌</text>
      <text x="180" y="150" text-anchor="end" fill="var(--breath)">のど</text>
      <line x1="182" y1="146" x2="220" y2="166" stroke="var(--breath)" stroke-width="1" opacity=".5"/>
    </g>
    <text x="288" y="334" text-anchor="middle" font-family="var(--jp)" font-size="12" fill="var(--breath)" font-weight="700">ここが「響く空間」</text>
    <line id="spaceLine" x1="288" y1="322" x2="288" y2="205" stroke="var(--breath)" stroke-width="1" stroke-dasharray="3 3" opacity=".5"/>
  `;
}
buildMouth();
// 舌：open大で平たく（盛り上がりが減る）。上下移動はlowerJawグループで行う
function tonguePath(o){
  const hump=22-o*1.6;
  const tipX=332, rootX=232, top=214-hump, base=232;
  return `M${rootX} 224 Q286 ${top} ${tipX} 216 L${tipX} 224 Q286 ${base} ${rootX+10} ${base-2} Q${rootX} 230 ${rootX} 224 Z`;
}
function softPath(o){
  const lift=o*2.1;
  return `M240 164 Q${226} ${182-lift} ${233} ${197-lift*1.4}`;
}
function updMouth(){
  const v=+openEl.value;
  ms.querySelector('#tongue').setAttribute('d',tonguePath(v));
  ms.querySelector('#soft').setAttribute('d',softPath(v));
  // 下あごユニットを下げる＝口が開く
  ms.querySelector('#lowerJaw').setAttribute('transform',`translate(0 ${v*2.6})`);
  ms.querySelector('#lowlip').setAttribute('transform',`translate(0 ${v*2.6})`);
  const cav=ms.querySelector('#cavity');
  cav.setAttribute('ry',15+v*4.2);
  cav.setAttribute('cy',186+v*1.4);
  cav.setAttribute('rx',50+v*1.3);
  ms.querySelector('#spaceLine').setAttribute('y2',186+v*1.4+(15+v*4.2));
  document.getElementById('vOpen').textContent = v<=2?'せまい':v<=6?'ふつう':'広い';
}
openEl.addEventListener('input',updMouth);updMouth();
document.querySelectorAll('#mouthPresets .chip').forEach(c=>c.addEventListener('click',()=>{
  document.querySelectorAll('#mouthPresets .chip').forEach(x=>x.classList.remove('on'));
  c.classList.add('on');openEl.value=c.dataset.open;fill(openEl);updMouth();
}));
let wt=0;
function mouthLoop(){
  if(mode==='mouth'&&!reduce){
    wt++;
    const v=+openEl.value, base=16+v*5;
    const cav=ms.querySelector('#cavity');
    const cx=+cav.getAttribute('cx'), cy=+cav.getAttribute('cy');
    const w1=ms.querySelector('#wave1'),w2=ms.querySelector('#wave2');
    if(w1&&w2){
      const t1=(wt%120)/120, t2=((wt+60)%120)/120;
      [[w1,t1],[w2,t2]].forEach(([w,t])=>{
        w.setAttribute('cx',cx);w.setAttribute('cy',cy);
        w.setAttribute('r',base*(0.3+t*1.5));
        w.setAttribute('opacity',(1-t)*0.5*(0.4+v/14));
      });
    }
  }
  requestAnimationFrame(mouthLoop);
}

/* ============ LUNGS (svg) ============ */
const ls=document.getElementById('lungSvg');
ls.innerHTML=`
  <defs>
    <radialGradient id="skinL" cx="50%" cy="35%" r="65%"><stop offset="0%" stop-color="#f1c79f"/><stop offset="100%" stop-color="#dba074"/></radialGradient>
    <linearGradient id="lungGrad" x1="0" y1="0" x2="0" y2="1"><stop offset="0%" stop-color="rgba(111,214,230,.34)"/><stop offset="100%" stop-color="rgba(111,214,230,.16)"/></linearGradient>
  </defs>
  <text x="210" y="20" text-anchor="middle" fill="var(--text)" font-size="14" font-family="var(--jp)" font-weight="700">肺と、まわりの呼吸筋</text>

  <!-- 体（首・肩・胴） -->
  <path d="M178 98 L178 122 Q150 130 140 154 L122 396 L298 396 L280 154 Q270 130 242 122 L242 98 Z" fill="#2f5a66" stroke="#22454f" stroke-width="2"/>
  <rect x="190" y="88" width="40" height="30" rx="8" fill="url(#skinL)"/>
  <circle cx="210" cy="64" r="32" fill="url(#skinL)" stroke="#c98a63" stroke-width="1.5"/>
  <path d="M179 56 Q185 26 210 26 Q235 26 241 56 Q235 40 210 39 Q185 40 179 56 Z" fill="#3a2c22"/>
  <ellipse cx="199" cy="64" rx="3.3" ry="2.5" fill="#fbf7ef"/><circle cx="199" cy="64" r="1.7" fill="#3a2418"/>
  <ellipse cx="221" cy="64" rx="3.3" ry="2.5" fill="#fbf7ef"/><circle cx="221" cy="64" r="1.7" fill="#3a2418"/>
  <path d="M203 76 Q210 80 217 76" stroke="#b85f50" stroke-width="2" fill="none" stroke-linecap="round"/>
  <path d="M178 98 Q210 118 242 98" fill="none" stroke="#22454f" stroke-width="3"/>

  <!-- 360°リング（呼吸筋） -->
  <ellipse id="ring" cx="210" cy="252" rx="112" ry="138" fill="rgba(230,169,63,.06)" stroke="var(--brass)" stroke-width="2.5" stroke-dasharray="4 7" stroke-opacity=".8"/>

  <!-- 気管・気管支 -->
  <path d="M210 122 L210 162 M210 162 L186 182 M210 162 L234 182" stroke="#cfcabd" stroke-width="5" fill="none" stroke-linecap="round"/>

  <!-- 肺 -->
  <path id="lungL" d="M198 160 Q156 164 146 214 Q138 268 162 302 Q184 316 200 300 Q204 252 198 160 Z" fill="url(#lungGrad)" stroke="var(--breath)" stroke-width="2.5"/>
  <path id="lungR" d="M222 160 Q264 164 274 214 Q282 268 258 302 Q236 316 220 300 Q216 252 222 160 Z" fill="url(#lungGrad)" stroke="var(--breath)" stroke-width="2.5"/>

  <!-- 横隔膜 -->
  <path id="diaph" d="M142 310 Q210 342 278 310" stroke="var(--coral)" stroke-width="5" fill="none" stroke-linecap="round"/>

  <!-- ラベル -->
  <g font-family="var(--jp)" font-size="12.5">
    <text x="316" y="212" fill="var(--breath)">肺</text>
    <text x="210" y="368" text-anchor="middle" fill="var(--coral)">横隔膜（下がると吸える）</text>
    <text x="210" y="112" text-anchor="middle" fill="var(--brass)" font-size="12" letter-spacing="1">呼吸筋（360°・背中側も）</text>
  </g>
  <text id="lungStatus" x="210" y="412" text-anchor="middle" font-family="var(--jp)" font-size="13.5" font-weight="700"></text>
`;
const inhEl=document.getElementById('inh');
let autoBreath=true, lt=0;
function setLungs(amount){ // amount 0..1
  const a=amount, s=1+a*0.15;
  const L=ls.querySelector('#lungL'),R=ls.querySelector('#lungR');
  L.style.transformOrigin='172px 232px';R.style.transformOrigin='248px 232px';
  L.setAttribute('transform',`translate(${-a*7} ${-a*4}) scale(${s} ${1+a*0.12})`);
  R.setAttribute('transform',`translate(${a*7} ${-a*4}) scale(${s} ${1+a*0.12})`);
  const ring=ls.querySelector('#ring');
  ring.setAttribute('rx',112+a*16);ring.setAttribute('ry',138+a*10);
  ring.setAttribute('stroke-opacity',0.5+a*0.5);ring.setAttribute('stroke-width',2.5+a*1.8);
  ls.querySelector('#diaph').setAttribute('d',`M142 ${310+a*18} Q210 ${342+a*16} 278 ${310+a*18}`);
  const st=ls.querySelector('#lungStatus');
  if(st){
    if(a>0.55){st.textContent='吸う：肺がふくらみ、筋肉が360°広がる';st.setAttribute('fill','var(--breath)');}
    else if(a<0.4){st.textContent='吐く：筋肉でゆっくり支えながら';st.setAttribute('fill','var(--coral)');}
    else{st.textContent='';}
  }
}
document.querySelectorAll('#lungToggle button').forEach(b=>b.addEventListener('click',()=>{
  document.querySelectorAll('#lungToggle button').forEach(x=>x.classList.remove('on'));
  b.classList.add('on');autoBreath=b.dataset.auto==='1';
  const man=document.getElementById('lungManual');
  man.style.opacity=autoBreath?'.4':'1';man.style.pointerEvents=autoBreath?'none':'auto';
}));
inhEl.addEventListener('input',()=>{if(!autoBreath){setLungs(inhEl.value/10);document.getElementById('vInh').textContent=inhEl.value<=3?'浅い':inhEl.value<=7?'ふつう':'深い';}});
function lungLoop(){
  if(mode==='lungs'){
    if(autoBreath){
      if(!reduce){lt++; const cyc=(Math.sin(lt/55)*0.5+0.5); setLungs(cyc);}
      else setLungs(0.6);
    }
  }
  requestAnimationFrame(lungLoop);
}
setLungs(0.3);

/* ============ POSTURE (svg) ============ */
const ps=document.getElementById('postureSvg');
const posEl=document.getElementById('pos');
function buildPosture(){ps.innerHTML=`
  <defs>
    <radialGradient id="skinP" cx="60%" cy="38%" r="65%">
      <stop offset="0%" stop-color="#f1c79f"/><stop offset="100%" stop-color="#dba074"/>
    </radialGradient>
    <linearGradient id="lungP" x1="0" y1="0" x2="0" y2="1">
      <stop offset="0%" stop-color="rgba(111,214,230,.28)"/><stop offset="100%" stop-color="rgba(111,214,230,.12)"/>
    </linearGradient>
  </defs>
  <line x1="70" y1="412" x2="350" y2="412" stroke="var(--line)" stroke-width="2"/>
  <text x="210" y="26" text-anchor="middle" fill="var(--text)" font-size="14" font-family="var(--jp)" font-weight="700">空気の通り道（横から）</text>
  <!-- ミニゲージ：通り＆ラクさ（真ん中がベスト） -->
  <g font-family="var(--jp)" font-size="11">
    <text x="34" y="60" fill="var(--muted)">空気の通り</text>
    <rect x="104" y="52" width="92" height="9" rx="4.5" fill="rgba(255,255,255,.1)"/>
    <rect id="gAir" x="104" y="52" width="0" height="9" rx="4.5"/>
    <text x="34" y="80" fill="var(--muted)">のどのラクさ</text>
    <rect x="104" y="72" width="92" height="9" rx="4.5" fill="rgba(255,255,255,.1)"/>
    <rect id="gEase" x="104" y="72" width="0" height="9" rx="4.5"/>
  </g>

  <!-- 胴 -->
  <path id="torso" fill="#2f5a66" stroke="#22454f" stroke-width="2"/>
  <!-- 首 -->
  <line id="neck" stroke="url(#skinP)" stroke-width="22" stroke-linecap="round"/>
  <!-- 襟 -->
  <path id="collar" fill="none" stroke="#22454f" stroke-width="3" stroke-linecap="round"/>
  <!-- 肺 -->
  <ellipse id="lung" rx="32" ry="42" fill="url(#lungP)" stroke="var(--breath)" stroke-width="2" stroke-opacity=".5"/>

  <!-- 頭（中身は固定・グループごと回転移動） -->
  <g id="head">
    <path d="M-24 -10 C-30 -36 2 -44 24 -32 C 6 -36 -16 -26 -19 2 Z" fill="#3a2c22"/>
    <path d="M-22 -6 C-26 -30 -2 -38 17 -31 C 31 -27 29 -2 25 6 C 27 15 20 23 8 25 C -9 27 -22 17 -22 -6 Z" fill="url(#skinP)" stroke="#c98a63" stroke-width="1.5"/>
    <path d="M23 0 L32 8 L23 11 Z" fill="url(#skinP)" stroke="#c98a63" stroke-width="1"/>
    <ellipse cx="7" cy="-4" rx="3.4" ry="2.6" fill="#fbf7ef"/><circle cx="9" cy="-4" r="1.8" fill="#3a2418"/>
    <path d="M0 -12 Q7 -15 14 -11" stroke="#5a4634" stroke-width="2" fill="none" stroke-linecap="round"/>
    <path d="M15 12 Q20 14 24 11" stroke="#b85f50" stroke-width="2.2" fill="none" stroke-linecap="round"/>
  </g>

  <!-- 空気の通り道 -->
  <path id="tubeOut" fill="none" stroke-linecap="round" stroke-linejoin="round"/>
  <path id="tubeIn" fill="none" stroke-linecap="round" stroke-linejoin="round"/>
  <circle id="p1" r="4.5" fill="#fff"/><circle id="p2" r="4.5" fill="#fff"/>
  <circle id="p3" r="4.5" fill="#fff"/><circle id="p4" r="4.5" fill="#fff"/>

  <!-- ラベル -->
  <g font-family="var(--jp)" font-size="12.5" fill="var(--text)">
    <text id="lbNose" text-anchor="start">鼻・口</text>
    <text x="96" y="206" text-anchor="end">のど</text>
    <text x="96" y="252" text-anchor="end">気管</text>
    <text x="96" y="300" text-anchor="end">肺</text>
  </g>
  <g stroke="var(--muted)" stroke-width="1" opacity=".5">
    <line id="lnNose"/><line id="lnThroat" x1="100" y1="202"/><line id="lnTrach" x1="100" y1="248"/><line id="lnLung" x1="100" y1="296"/>
  </g>

  <text id="ptxt" x="210" y="404" text-anchor="middle" font-size="14" font-family="var(--jp)" font-weight="700"></text>
`;}
buildPosture();
function setPosture(v){ // v:0(あご上げ)..2(理想)..10(猫背あご引き)
  const hipX=215,hipY=400, lean=(v-2)/10;
  const sx=210+lean*28, sy=222;
  const tilt=(v-2)*5.2;                       // 頭の傾き（＋であご引き）
  const tr=tilt*Math.PI/180, c=Math.cos(tr), s=Math.sin(tr);
  const hx=sx+38+lean*58, hy=sy-62+(v>3?(v-3)*4.5:0);
  // 胴
  ps.querySelector('#torso').setAttribute('d',
    `M${sx-22} ${sy} C ${sx-36+lean*36} ${sy+72} ${hipX-32} ${hipY-72} ${hipX-20} ${hipY} L ${hipX+22} ${hipY} C ${hipX+28} ${hipY-90} ${sx+32} ${sy+56} ${sx+24} ${sy} Z`);
  // 首（肩→頭の下）
  const neck=ps.querySelector('#neck');
  neck.setAttribute('x1',sx+2);neck.setAttribute('y1',sy-2);
  neck.setAttribute('x2',hx-18*s);neck.setAttribute('y2',hy+18*c);
  // 襟
  ps.querySelector('#collar').setAttribute('d',`M${sx-20} ${sy-2} Q${sx+2} ${sy+12} ${sx+24} ${sy-2}`);
  // 頭
  ps.querySelector('#head').setAttribute('transform',`translate(${hx} ${hy}) rotate(${tilt})`);
  // 肺
  const lung=ps.querySelector('#lung');
  lung.setAttribute('cx',sx+6);lung.setAttribute('cy',sy+58);
  // 通り道の通過点
  const nose ={x:hx+24*c-8*s, y:hy+24*s+8*c};   // 鼻先（回転追従）
  const throat={x:sx+8, y:sy-16};
  const trMid={x:sx+5, y:sy+18};
  const lungE={x:sx+6, y:sy+46};
  // 折れ具合：のどでの曲がり
  const bend=v>3?(v-3)*5:0;
  const d=`M${nose.x.toFixed(1)} ${nose.y.toFixed(1)} Q${throat.x+8+bend} ${throat.y-6} ${throat.x} ${throat.y} L${trMid.x} ${trMid.y} L${lungE.x} ${lungE.y}`;
  // 評価：気道の通り（猫背で折れる）／ のどの力み（上げ・下げ両方で増える）
  const airway=1-Math.min(1,Math.max(0,v-2)/7);
  const strain=Math.min(1,Math.abs(v-2)/5.5);
  const ease=1-strain;
  const col=airway>0.6?'var(--good)':airway>0.32?'var(--breath)':'var(--warn)';
  const o=ps.querySelector('#tubeOut'), inn=ps.querySelector('#tubeIn');
  o.setAttribute('d',d);o.setAttribute('stroke','rgba(255,255,255,.16)');o.setAttribute('stroke-width',16);
  inn.setAttribute('d',d);inn.setAttribute('stroke',col);inn.setAttribute('stroke-width',(4.5+airway*7).toFixed(1));inn.setAttribute('opacity',(0.55+airway*0.45).toFixed(2));
  // ゲージ更新
  const gcol=x=>x>0.7?'var(--good)':x>0.4?'var(--breath)':'var(--warn)';
  const gA=ps.querySelector('#gAir');gA.setAttribute('width',92*airway);gA.setAttribute('fill',gcol(airway));
  const gE=ps.querySelector('#gEase');gE.setAttribute('width',92*ease);gE.setAttribute('fill',gcol(ease));
  // ラベル＆リーダー線
  ps.querySelector('#lbNose').setAttribute('x',nose.x+14);ps.querySelector('#lbNose').setAttribute('y',nose.y-8);
  ps.querySelector('#lnNose').setAttribute('x1',nose.x+12);ps.querySelector('#lnNose').setAttribute('y1',nose.y-10);
  ps.querySelector('#lnNose').setAttribute('x2',nose.x+2);ps.querySelector('#lnNose').setAttribute('y2',nose.y-2);
  ps.querySelector('#lnThroat').setAttribute('x2',throat.x-6);ps.querySelector('#lnThroat').setAttribute('y2',throat.y);
  ps.querySelector('#lnTrach').setAttribute('x2',trMid.x-6);ps.querySelector('#lnTrach').setAttribute('y2',trMid.y);
  ps.querySelector('#lnLung').setAttribute('x2',sx-6);ps.querySelector('#lnLung').setAttribute('y2',sy+58);
  // 粒・状態
  window._postPts=[nose,throat,trMid,lungE];window._q=airway;
  document.getElementById('vPos').textContent = v<=1?'あご上げすぎ':v<=3?'ニュートラル':v<=5?'やや前かがみ':'猫背';
  const txt=ps.querySelector('#ptxt');
  if(v>=1&&v<=3){txt.textContent='バッチリ！頭が背骨の上にスッと乗ってる';txt.setAttribute('fill','var(--good)');}
  else if(v<1){txt.textContent='あご上げすぎ：空気は通るけど、のどが緊張ぎみ';txt.setAttribute('fill','var(--warn)');}
  else if(v<=5){txt.textContent='やや前かがみ。少し通りにくいよ';txt.setAttribute('fill','var(--breath)');}
  else{txt.textContent='猫背：のどで通り道が折れてるよ';txt.setAttribute('fill','var(--warn)');}
}
posEl.addEventListener('input',()=>setPosture(+posEl.value));
document.querySelectorAll('#posturePresets .chip').forEach(c=>c.addEventListener('click',()=>{
  document.querySelectorAll('#posturePresets .chip').forEach(x=>x.classList.remove('on'));
  c.classList.add('on');posEl.value=c.dataset.pos;fill(posEl);setPosture(+posEl.value);
}));
let pt2=0;
function postureLoop(){
  if(mode==='posture'&&window._postPts&&!reduce){
    const q=window._q||0.5;
    pt2=(pt2+0.004+q*0.012)%1;                 // 通りやすいほど速く流れる
    const pts=window._postPts;
    for(let i=0;i<4;i++){
      const t=(pt2+i/4)%1, seg=Math.min(2,Math.floor(t*3)), u=(t*3)-seg;
      const a=pts[seg], b=pts[seg+1];
      const x=a.x+(b.x-a.x)*u, y=a.y+(b.y-a.y)*u;
      const cc=ps.querySelector('#p'+(i+1));
      cc.setAttribute('cx',x);cc.setAttribute('cy',y);
      cc.setAttribute('opacity',(Math.sin(t*Math.PI)*(0.4+q*0.6)).toFixed(2));
      cc.setAttribute('fill', q>0.32?'#fff':'var(--warn)');
    }
  }
  requestAnimationFrame(postureLoop);
}
setPosture(2);

/* ---------- boot ---------- */
sizeBreath();
breathLoop();mouthLoop();lungLoop();postureLoop();
</script>
</body>
</html>
