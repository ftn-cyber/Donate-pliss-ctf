<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Donate Pliss // Halaman Donasi</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=JetBrains+Mono:wght@400;500;700;800&family=Share+Tech+Mono&display=swap" rel="stylesheet">
<style>
  :root{
    --bg:#030812; --panel:#071022; --panel-2:#0b1830; --line:#123055;
    --cyan:#35e6ff; --blue:#2f6fff; --dim:#4d7ba8; --text:#cfe8ff;
    --ok:#23ff9d; --warn:#ffcf4d;
  }
  *{box-sizing:border-box;}
  body{
    margin:0; background:var(--bg); color:var(--text);
    font-family:'JetBrains Mono', monospace;
  }
  .wrap{ max-width: 880px; margin:0 auto; padding: 36px 20px 70px; }

  header{
    border:1px solid var(--line);
    background: linear-gradient(180deg, var(--panel), var(--bg));
    border-radius:6px; padding: 26px 26px; margin-bottom: 30px;
    position:relative; overflow:hidden;
  }
  header::before{
    content:""; position:absolute; top:0; left:0; right:0; height:2px;
    background: linear-gradient(90deg, transparent, var(--cyan), transparent);
    animation: sweep 3s linear infinite;
  }
  @keyframes sweep{0%{transform:translateX(-100%);}100%{transform:translateX(100%);}}
  .eyebrow{ font-family:'Share Tech Mono',monospace; color:var(--dim); font-size:12px; letter-spacing:3px; text-transform:uppercase; }
  h1{ margin:6px 0 8px; font-size: clamp(26px,5vw,40px); color:#eaf6ff; text-shadow:0 0 14px rgba(53,230,255,.35); }
  h1 span{ color:var(--cyan); }
  .sub{ color:var(--dim); font-size:13.5px; line-height:1.7; max-width:620px; }

  .stat-row{ display:flex; gap:14px; margin-top:20px; flex-wrap:wrap; }
  .stat{
    flex:1; min-width:140px; background:var(--panel-2); border:1px solid var(--line);
    border-radius:4px; padding:12px 14px;
  }
  .stat .num{ color:var(--ok); font-size:18px; font-weight:700; }
  .stat .lbl{ color:var(--dim); font-size:11px; letter-spacing:1px; text-transform:uppercase; }

  .section-title{
    font-family:'Share Tech Mono',monospace; color:var(--cyan);
    font-size:14px; letter-spacing:2px; text-transform:uppercase;
    margin: 34px 0 14px; display:flex; align-items:center; gap:10px;
  }
  .section-title::after{ content:""; flex:1; height:1px; background:var(--line); }

  .donor-card{
    border:1px solid var(--line); background:var(--panel);
    border-radius:6px; padding:20px 22px; margin-bottom:18px;
    position:relative; transition: border-color .25s, box-shadow .25s;
  }
  .donor-card:hover{ border-color: var(--blue); box-shadow: 0 0 20px rgba(47,111,255,.18); }

  .donor-head{ display:flex; align-items:center; gap:12px; margin-bottom:12px; }
  .avatar{
    width:42px; height:42px; border-radius:50%;
    background: linear-gradient(135deg, var(--blue), var(--cyan));
    display:flex; align-items:center; justify-content:center;
    font-weight:800; color:#001225; font-size:16px; flex-shrink:0;
  }
  .donor-name{ color:#eaf6ff; font-size:15.5px; font-weight:700; }
  .donor-meta{ color:var(--dim); font-size:11.5px; letter-spacing:.5px; }
  .amount{
    margin-left:auto; background:var(--panel-2); border:1px solid var(--ok);
    color:var(--ok); font-size:12.5px; font-weight:700; padding:4px 12px; border-radius:20px;
    white-space:nowrap;
  }

  .message{
    font-size:13.5px; line-height:1.75; color:var(--text);
    background:var(--panel-2); border-left:3px solid var(--blue);
    padding:12px 14px; border-radius:3px;
  }
  .message a{
    color:var(--cyan); word-break:break-all; text-decoration:none; border-bottom:1px dashed var(--cyan);
  }
  .message a:hover{ color:#fff; border-bottom-color:#fff; }

  .clue-badge{
    display:inline-flex; align-items:center; gap:6px;
    margin-top:10px; font-size:11px; letter-spacing:1px; text-transform:uppercase;
    color:var(--warn); border:1px solid var(--warn); padding:3px 10px; border-radius:20px;
    font-family:'Share Tech Mono',monospace;
  }

  .cta-box{
    margin-top: 38px; text-align:center; border:1px dashed var(--line);
    border-radius:6px; padding: 26px; color:var(--dim); font-size:13px;
  }
  .cta-box button{
    margin-top:12px; background:var(--blue); color:#001225; border:none;
    font-weight:700; font-family:'JetBrains Mono',monospace; font-size:13px;
    padding:10px 22px; border-radius:4px; cursor:pointer; letter-spacing:1px;
    text-transform:uppercase;
  }
  .cta-box button:hover{ background:var(--cyan); }

  footer{ text-align:center; color:var(--dim); font-size:11.5px; margin-top:34px; }
</style>
</head>
<body>
<div class="wrap">

  <header>
    <div class="eyebrow">// laman resmi</div>
    <h1>DONATE <span>PLISS</span></h1>
    <div class="sub">
      Terima kasih untuk setiap dukungan yang masuk. Berikut riwayat donasi terbaru beserta
      pesan yang dititipkan oleh para donatur.
    </div>
    <div class="stat-row">
      <div class="stat"><div class="num">3</div><div class="lbl">Donatur Terbaru</div></div>
      <div class="stat"><div class="num">Rp300rb+ / $400 / Rp900jt</div><div class="lbl">Total Nominal Tercatat</div></div>
      <div class="stat"><div class="num">AKTIF</div><div class="lbl">Status Server</div></div>
    </div>
  </header>

  <div class="section-title">Riwayat Donasi</div>

  <!-- DONATUR 1 -->
  <div class="donor-card">
    <div class="donor-head">
      <div class="avatar">S</div>
      <div>
        <div class="donor-name">secufadby</div>
        <div class="donor-meta">Donatur #1</div>
      </div>
      <div class="amount">Rp 300.000</div>
    </div>
    <div class="message">
      Halo, saya memberikan 300k ini untuk menyampaikan pesan ke satpam. Link ini untuk satpam:
      <br>
      <a href="https://ftn-cyber.github.io/Newspaper-SQL-injection/" target="_blank" rel="noopener noreferrer">
        https://ftn-cyber.github.io/Newspaper-SQL-injection/
      </a>
    </div>
    <div class="clue-badge">🔁 petunjuk: balik kata "satpam"</div>
  </div>

  <!-- DONATUR 2 -->
  <div class="donor-card">
    <div class="donor-head">
      <div class="avatar">Z</div>
      <div>
        <div class="donor-name">zero crush</div>
        <div class="donor-meta">Donatur #2</div>
      </div>
      <div class="amount">$400</div>
    </div>
    <div class="message">
      Saya memberikan 400 dolar ini untuk memberitahu pengguna Donate Pliss agar berhati-hati.
      Link ini untuk panduan berhati-hatinya:
      <br>
      <a href="https://ftn-cyber.github.io/Newspaper-mistery-hacker/" target="_blank" rel="noopener noreferrer">
        https://ftn-cyber.github.io/Newspaper-mistery-hacker/
      </a>
    </div>
    <div class="clue-badge">🔁 petunjuk: balik kata "hacker"</div>
  </div>

  <!-- DONATUR 3 -->
  <div class="donor-card">
    <div class="donor-head">
      <div class="avatar">S</div>
      <div>
        <div class="donor-name">sertfis</div>
        <div class="donor-meta">Donatur #3</div>
      </div>
      <div class="amount">Rp 900.000.000</div>
    </div>
    <div class="message">
      Aku mengirim ini untuk temanku Edo di luar sana yang sedang sakit. Aku mengirimkan 900 juta
      ke Edo untuk biaya rumah sakitnya. Edo adalah temanku yang membuat sebuah web bernama Pliss.
      Berikut link web pemberitahuan bahwa Edo yang membuatnya:
      <br>
      <a href="https://ftn-cyber.github.io/Newspaper-Edo-mistery-plisss/" target="_blank" rel="noopener noreferrer">
        https://ftn-cyber.github.io/Newspaper-Edo-mistery-plisss/
      </a>
    </div>
    <div class="clue-badge">🔁 petunjuk: balik kata "Edo"</div>
  </div>

  <div class="cta-box">
    Ingin ikut mendukung Donate Pliss?
    <br>
    <button type="button" onclick="alert('Fitur donasi belum aktif di halaman demo ini.')">Donasi Sekarang</button>
  </div>

  <footer>DONATE PLISS — halaman donasi demo, dibuat untuk keperluan simulasi.</footer>
</div>
</body>
</html>

