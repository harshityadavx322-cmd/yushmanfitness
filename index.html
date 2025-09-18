<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>BDG Games — Demo</title>
  <style>
    :root{
      --bg:#0b0f1a; --card:#0f1724; --accent:#00e6a8; --muted:#94a3b8;
      font-family: Inter, system-ui, Arial, sans-serif;
    }
    body{margin:0;background:linear-gradient(180deg,#061024 0%, #0b0f1a 100%);color:#e6eef8}
    header{padding:24px 28px;display:flex;align-items:center;justify-content:space-between}
    .brand{display:flex;gap:12px;align-items:center}
    .logo{width:44px;height:44px;border-radius:8px;background:linear-gradient(135deg,#0ff,#06f);display:flex;align-items:center;justify-content:center;font-weight:700;color:#042}
    nav a{color:var(--muted);margin-left:18px;text-decoration:none;font-weight:600}
    .hero{padding:28px;display:flex;gap:24px;align-items:center}
    .hero-left{flex:1}
    .hero h1{font-size:32px;margin:0 0 10px}
    .hero p{color:var(--muted);margin:0 0 16px}
    .btn{background:var(--accent);color:#021; padding:10px 16px;border-radius:8px;border:none;font-weight:700;cursor:pointer}
    .grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(220px,1fr));gap:18px;padding:22px;}
    .card{background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));padding:16px;border-radius:12px;box-shadow:0 6px 18px rgba(2,6,23,0.6)}
    .card h3{margin:0 0 8px}
    .footer{padding:16px;color:var(--muted);text-align:center}
    .topbar{display:flex;gap:12px;align-items:center}
    .credits-badge{background:#071827;padding:8px 12px;border-radius:999px;color:var(--accent);font-weight:700}
    .small{font-size:13px;color:var(--muted)}
    .play-btn{background:transparent;border:1px solid rgba(255,255,255,0.06);padding:8px 12px;border-radius:8px;color:var(--accent);cursor:pointer}
  </style>
</head>
<body>
  <header>
    <div class="brand">
      <div class="logo">BDG</div>
      <div>
        <div style="font-weight:800">BDG Games</div>
        <div class="small">Demo portal • Virtual credits only</div>
      </div>
    </div>
    <div class="topbar">
      <div class="credits-badge">Credits: <span id="credits">0</span></div>
      <button class="btn" id="buyBtn">Buy Credits</button>
    </div>
  </header>

  <section class="hero">
    <div class="hero-left">
      <h1>Spin & Win — Demo</h1>
      <p class="small">Yeh demo site sirf virtual credits ke liye hai. Real money se judi functionality ke liye legal licence aur payment integration zaroori hai.</p>
      <div style="margin-top:14px">
        <button class="btn" onclick="startGame('spin')">Start Spin Demo</button>
        <button class="play-btn" onclick="openHow()">How it works</button>
      </div>
    </div>
    <div style="width:320px">
      <div class="card">
        <h3>Featured Game: Lucky Spin</h3>
        <p class="small">Spend 10 credits to spin. Win up to 100 credits. (Demo random)</p>
        <div style="display:flex;gap:8px;margin-top:10px">
          <button class="btn" onclick="playSpin()">Play (10 cr)</button>
          <button class="play-btn" onclick="showHistory()">History</button>
        </div>
      </div>
    </div>
  </section>

  <section>
    <div class="grid">
      <div class="card">
        <h3>Game — Lucky Spin</h3>
        <p class="small">Chance-based demo. Uses virtual credits stored in your browser (localStorage).</p>
      </div>
      <div class="card">
        <h3>Game — Trivia Challenge</h3>
        <p class="small">Skill game demo placeholder — answer questions to win credits.</p>
      </div>
      <div class="card">
        <h3>Game — Tournament</h3>
        <p class="small">Demo bracket for skill-based tournaments (no real money).</p>
      </div>
    </div>
  </section>

  <div style="padding:22px" id="output"></div>

  <div class="footer">
    <div class="small">This is a demo. No real money transactions. For commercial/real-money operation you must obtain licenses and use compliant payment providers.</div>
  </div>

<script>
  // Simple demo credit management (localStorage)
  const creditsKey = 'bdg_demo_credits';
  const historyKey = 'bdg_demo_history';

  function getCredits(){ return parseInt(localStorage.getItem(creditsKey) || '50',10); } // start with 50 demo credits
  function saveCredits(v){ localStorage.setItem(creditsKey,String(v)); document.getElementById('credits').innerText = v; }
  function addHistory(text){ const h = JSON.parse(localStorage.getItem(historyKey) || '[]'); h.unshift({t:Date.now(),msg:text}); localStorage.setItem(historyKey, JSON.stringify(h)); }

  // init
  saveCredits(getCredits());

  document.getElementById('buyBtn').addEventListener('click',function(){
    // MOCK flow: open external payment page or popup. Replace '#' with your real payment checkout link from gateway.
    // IMPORTANT: do NOT accept card details on GitHub Pages. Use a proper backend.
    const checkoutUrl = '#'; // <-- replace with your checkout URL from Razorpay/Stripe/etc after legal checks
    if(checkoutUrl === '#'){
      alert('Demo: buy credits disabled. To accept payments you must integrate a licensed payment gateway and backend.');
      return;
    }
    window.open(checkoutUrl, '_blank');
  });

  function playSpin(){
    let c = getCredits();
    if(c < 10){ alert('Not enough credits. Use Buy Credits (demo).'); return; }
    c -= 10;
    // demo random draw
    const roll = Math.random();
    let win = 0;
    if(roll > 0.995){ win = 100; }      // tiny chance big win
    else if(roll > 0.9){ win = 25; }
    else if(roll > 0.6){ win = 5; }
    else { win = 0; }
    c += win;
    saveCredits(c);
    const msg = Spin result: rolled ${Math.floor(roll*1000)}/1000 — won ${win} credits.;
    addHistory(msg);
    document.getElementById('output').innerText = msg;
  }

  function showHistory(){
    const h = JSON.parse(localStorage.getItem(historyKey) || '[]');
    if(h.length === 0){ alert('No history yet'); return; }
    const html = h.slice(0,10).map(x=> new Date(x.t).toLocaleString() + ' — ' + x.msg).join('\\n');
    alert(html);
  }

  function startGame(type){
    if(type==='spin') playSpin();
  }

  function openHow(){
    alert('Demo site: virtual credits stored locally. For real payments you must: obtain licences, integrate a payment gateway, implement KYC & secure backend.');
  }
</script>
</body>
</html>
