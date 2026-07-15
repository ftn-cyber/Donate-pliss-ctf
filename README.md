<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Donate Pliss // Halaman Donasi</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600;700;800&family=Inter:wght@400;500;600&display=swap" rel="stylesheet">
<style>
  :root{
    --bg:#f4f8ff; --panel:#ffffff; --panel-2:#eaf2ff;
    --line:#d7e6ff; --blue:#2563eb; --blue-deep:#1d4ed8; --sky:#3b9dff;
    --dim:#5b7796; --text:#1c2b3f; --ok:#0ea86b; --warn:#e0a300;
  }
  *{box-sizing:border-box;}
  body{
    margin:0; background:var(--bg); color:var(--text);
    font-family:'Inter', sans-serif;
  }
  .wrap{ max-width: 880px; margin:0 auto; padding: 36px 20px 70px; }

  header{
    border:1px solid var(--line);
    background: linear-gradient(135deg, #ffffff, #eaf2ff);
    border-radius:14px; padding: 30px 28px; margin-bottom: 30px;
    box-shadow: 0 8px 24px rgba(37,99,235,0.08);
  }
  .eyebrow{ font-family:'Inter',sans-serif; color:var(--blue); font-weight:600; font-size:12px; letter-spacing:2px; text-transform:uppercase; }
  h1{ margin:8px 0 8px; font-family:'Poppins',sans-serif; font-weight:800; font-size: clamp(28px,5vw,42px); color:var(--blue-deep); }
  h1 span{ color: var(--sky); }
  .sub{ color:var(--dim); font-size:14px; line-height:1.7; max-width:620px; }

  .stat-row{ display:flex; gap:14px; margin-top:22px; flex-wrap:wrap; }
  .stat{
    flex:1; min-width:150px; background:var(--panel-2); border:1px solid var(--line);
    border-radius:10px; padding:14px 16px;
  }
  .stat .num{ color:var(--blue-deep); font-size:17px; font-weight:700; font-family:'Poppins',sans-serif; }
  .stat .lbl{ color:var(--dim); font-size:11px; letter-spacing:.5px; text-transform:uppercase; margin-top:2px; }

  .section-title{
    font-family:'Poppins',sans-serif; color:var(--blue-deep);
    font-size:16px; font-weight:700;
    margin: 34px 0 16px; display:flex; align-items:center; gap:10px;
  }
  .section-title::after{ content:""; flex:1; height:1px; background:var(--line); }

  .donor-card{
    border:1px solid var(--line); background:var(--panel);
    border-radius:12px; padding:20px 22px; margin-bottom:18px;
    box-shadow: 0 4px 14px rgba(37,99,235,0.06);
    transition: box-shadow .25s, transform .2s;
  }
  .donor-card:hover{ box-shadow: 0 8px 22px rgba(37,99,235,0.14); transform: translateY(-2px); }

  .donor-head{ display:flex; align-items:center; gap:12px; margin-bottom:12px; }
  .avatar{
    width:42px; height:42px; border-radius:50%;
    background: linear-gradient(135deg, var(--blue), var(--sky));
    display:flex; align-items:center; justify-content:center;
    font-weight:800; color:#fff; font-size:16px; flex-shrink:0;
    font-family:'Poppins',sans-serif;
  }
  .donor-name{ color:var(--text); font-size:15.5px; font-weight:700; font-family:'Poppins',sans-serif; }
  .donor-meta{ color:var(--dim); font-size:11.5px; letter-spacing:.3px; }
  .amount{
    margin-left:auto; background:#eafff5; border:1px solid var(--ok);
    color:var(--ok); font-size:12.5px; font-weight:700; padding:5px 14px; border-radius:20px;
    white-space:nowrap;
  }

  .message{
    font-size:13.5px; line-height:1.8; color:var(--text);
    background:var(--panel-2); border-left:3px solid var(--blue);
    padding:12px 14px; border-radius:6px;
  }
  .message a{
    color:var(--blue-deep); word-break:break-all; text-decoration:none; border-bottom:1px dashed var(--blue-deep);
    font-weight:500;
  }
  .message a:hover{ color:var(--sky); border-bottom-color:var(--sky); }

  .clue-badge{
    display:inline-flex; align-items:center; gap:6px;
    margin-top:10px; font-size:11px; letter-spacing:.5px; text-transform:uppercase;
    color:#8a5b00; background:#fff6e0; border:1px solid var(--warn); padding:4px 12px; border-radius:20px;
    font-weight:600;
  }

  .cta-box{
    margin-top: 38px; text-align:center; border:1px dashed var(--line);
    background:var(--panel); border-radius:12px; padding: 28px; color:var(--dim); font-size:13.5px;
  }
  .cta-box button{
    margin-top:14px; background: linear-gradient(135deg, var(--blue), var(--sky)); color:#fff; border:none;
    font-weight:700; font-family:'Poppins',sans-serif; font-size:13.5px;
    padding:11px 26px; border-radius:24px; cursor:pointer; letter-spacing:.5px;
    box-shadow: 0 6px 16px rgba(37,99,235,0.25);
  }
  .cta-box button:hover{ box-shadow: 0 8px 20px rgba(37,99,235,0.35); }

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
