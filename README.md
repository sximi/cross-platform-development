---
layout: default
title: Cross-Platform Development
---

<link href="https://fonts.googleapis.com/css2?family=Sarabun:wght@300;400;500&family=Mitr:wght@300;400;500&display=swap" rel="stylesheet">

<style>
* { margin: 0; padding: 0; box-sizing: border-box; }

body {
  font-family: 'Sarabun', sans-serif;
  background: #fff0f5;
  color: #4a1030;
}

body::before {
  content: '';
  position: fixed;
  inset: 0;
  background-image: radial-gradient(circle, #f9a8be 1.5px, transparent 1.5px);
  background-size: 28px 28px;
  opacity: 0.25;
  pointer-events: none;
  z-index: 0;
}

.wrap { position: relative; z-index: 1; }

.ribbon {
  background: #f9a8be;
  text-align: center;
  padding: 5px;
  font-size: 13px;
  letter-spacing: 6px;
  color: white;
  box-shadow: 0 2px 0 #f48aaa;
}

.page-header {
  background: #e8557a;
  padding: 1rem 2rem;
  box-shadow: 0 3px 0 #c03060;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.page-header .logo {
  font-family: 'Mitr', sans-serif;
  font-size: 1.05rem;
  color: white;
}

.page-header a {
  color: white;
  text-decoration: none;
  font-size: 0.88rem;
  background: rgba(255,255,255,0.2);
  padding: 4px 14px;
  border-radius: 20px;
}

main {
  max-width: 720px;
  margin: 2rem auto;
  padding: 0 1.5rem 4rem;
}

.hero-card {
  background: white;
  border-radius: 24px;
  border: 2px solid #f9a8be;
  padding: 2rem 2rem 1.5rem;
  margin-bottom: 1.5rem;
  box-shadow: 0 6px 0 #f4c0ce;
  text-align: center;
}

.kw-num {
  font-size: 11px;
  font-weight: 500;
  letter-spacing: .12em;
  color: #f9a8be;
  margin-bottom: 6px;
  font-family: 'Mitr', sans-serif;
}

.kw-title {
  font-family: 'Mitr', sans-serif;
  font-size: 2rem;
  font-weight: 500;
  color: #c0304a;
  margin-bottom: 8px;
}

.kw-badge {
  display: inline-block;
  background: #e8557a;
  color: white;
  font-size: 12px;
  padding: 3px 14px;
  border-radius: 20px;
  font-family: 'Mitr', sans-serif;
}

.card {
  background: white;
  border-radius: 20px;
  border: 1.5px solid #f9c8d8;
  padding: 1.6rem 1.8rem;
  margin-bottom: 1.2rem;
  box-shadow: 0 4px 0 #f4c0ce;
}

.section-title {
  font-family: 'Mitr', sans-serif;
  font-size: 0.98rem;
  color: #c0304a;
  margin-bottom: 1rem;
  padding-bottom: 0.6rem;
  border-bottom: 2px dashed #f9c8d8;
  display: flex;
  align-items: center;
  gap: 8px;
}

.badge {
  background: #e8557a;
  color: white;
  font-size: 11px;
  padding: 2px 10px;
  border-radius: 20px;
  font-family: 'Mitr', sans-serif;
}

blockquote {
  border-left: 3px solid #e8557a;
  padding: 0.75rem 1rem;
  margin: 0.75rem 0;
  background: #fff5f8;
  border-radius: 0 12px 12px 0;
  color: #6b2840;
  font-size: 0.93rem;
  line-height: 1.8;
}

blockquote em { color: #c0304a; font-style: normal; font-weight: 500; }

.thai-box {
  background: #fff5f8;
  border: 1.5px dashed #f9a8be;
  border-radius: 16px;
  padding: 1rem 1.2rem;
  color: #6b2840;
  font-size: 0.93rem;
  line-height: 1.9;
}

table { width: 100%; border-collapse: collapse; font-size: 0.91rem; }
th {
  background: #e8557a;
  color: white;
  padding: 9px 14px;
  text-align: left;
  font-family: 'Mitr', sans-serif;
  font-weight: 400;
}
th:first-child { border-radius: 10px 0 0 0; }
th:last-child  { border-radius: 0 10px 0 0; }
td { padding: 9px 14px; border-bottom: 1px solid #fce0ea; color: #6b2840; }
tr:last-child td { border-bottom: none; }
tr:nth-child(even) td { background: #fff5f8; }

.ai-block {
  border: 1.5px solid #f9c8d8;
  border-radius: 16px;
  padding: 1rem 1.2rem;
  margin-bottom: 0.8rem;
  background: #fff5f8;
}
.ai-block p { font-size: 0.93rem; line-height: 1.8; color: #6b2840; }
.ai-src { font-size: 11px; color: #e8557a; margin-top: 6px; font-weight: 500; }

.refs-list { list-style: none; display: flex; flex-direction: column; gap: 8px; }
.refs-list li { font-size: 0.91rem; color: #6b2840; }
.refs-list a { color: #c0304a; text-decoration: none; }
.refs-list a:hover { text-decoration: underline; }

.back-link {
  display: inline-block;
  margin-top: 1.5rem;
  background: #e8557a;
  color: white;
  text-decoration: none;
  padding: 8px 22px;
  border-radius: 20px;
  font-family: 'Mitr', sans-serif;
  font-size: 0.9rem;
  box-shadow: 0 3px 0 #c03060;
}

footer {
  background: #e8557a;
  color: white;
  text-align: center;
  padding: 1rem;
  font-size: 0.83rem;
  letter-spacing: 0.06em;
  box-shadow: 0 -3px 0 #c03060;
}
</style>

<div class="wrap">

<div class="page-header">
  <div class="logo">🎀 sximi.github.io</div>
  <a href="https://sximi.github.io">← หน้าหลัก</a>
</div>
<div class="ribbon">🌸 ✿ 🎀 ✿ 🌸 ✿ 🎀 ✿ 🌸 ✿ 🎀 ✿ 🌸</div>

<main>

  <div class="hero-card">
    <div class="kw-num">KEYWORD 05</div>
    <div class="kw-title">📱 Cross-Platform Development</div>
    <span class="kw-badge">Mobile & Desktop</span>
  </div>

  <div class="card">
    <div class="section-title">📖 Definition <span class="badge">English</span></div>
    <blockquote>
      "Cross-platform development is the practice of developing software products or services for multiple platforms or software environments. Engineers and developers use various methods to deploy the same application or product to multiple platforms."
      <br><br><em>— Red Hat</em>
    </blockquote>
    <blockquote>
      "Cross-platform development refers to creating applications that can run on multiple operating systems or platforms — such as Windows, macOS, Linux, iOS, and Android — using a single codebase or shared code."
      <br><br><em>— Microsoft</em>
    </blockquote>
  </div>

  <div class="card">
    <div class="section-title">🇹🇭 คำนิยาม <span class="badge">Thai</span></div>
    <div class="thai-box">
      Cross-Platform Development คือการพัฒนา App <strong>"เขียนโค้ดครั้งเดียว แต่รันได้ทั้งบน iOS, Android, Windows และ Web"</strong> แทนที่จะต้องเขียนแยกสำหรับแต่ละ platform ทำให้ประหยัดเวลาและทีมงานได้มาก 🌸
    </div>
  </div>

  <div class="card">
    <div class="section-title">🔍 Explanation <span class="badge">ขยายความ</span></div>
    <table>
      <tr><th>เกณฑ์</th><th>Cross-Platform</th><th>Native</th></tr>
      <tr><td><strong>โค้ด</strong></td><td>เขียนครั้งเดียว</td><td>แยกแต่ละ platform</td></tr>
      <tr><td><strong>ความเร็ว</strong></td><td>ช้ากว่าเล็กน้อย</td><td>เร็วสุด</td></tr>
      <tr><td><strong>ค่าใช้จ่าย</strong></td><td>ประหยัดกว่า</td><td>แพงกว่า</td></tr>
      <tr><td><strong>เหมาะกับ</strong></td><td>Startup, ทีมเล็ก</td><td>App performance สูง</td></tr>
    </table>
    <br>
    <table>
      <tr><th>Framework</th><th>ภาษา</th><th>รองรับ</th></tr>
      <tr><td><strong>Flutter</strong></td><td>Dart</td><td>iOS, Android, Web, Desktop</td></tr>
      <tr><td><strong>React Native</strong></td><td>JavaScript</td><td>iOS, Android</td></tr>
      <tr><td><strong>.NET MAUI</strong></td><td>C#</td><td>iOS, Android, Windows, macOS</td></tr>
      <tr><td><strong>Ionic</strong></td><td>JavaScript</td><td>iOS, Android, Web</td></tr>
    </table>
  </div>

  <div class="card">
    <div class="section-title">🤖 GenAI Explanation</div>
    <div class="ai-block">
      <p>"Cross-Platform Development เปลี่ยนโลกของการพัฒนา mobile app — startup ที่มีทีมเล็กสามารถสร้าง app รองรับทั้ง iOS และ Android พร้อมกันได้โดยไม่ต้องจ้างทีมแยกสองทีม"</p>
      <div class="ai-src">— ChatGPT (OpenAI)</div>
    </div>
    <div class="ai-block">
      <p>"ด้วยความก้าวหน้าของ Flutter และ React Native ช่องว่างด้าน performance ระหว่าง cross-platform และ native แคบลงมากในช่วงไม่กี่ปีที่ผ่านมา ทำให้เป็นตัวเลือกที่สมเหตุสมผลสำหรับ project ส่วนใหญ่"</p>
      <div class="ai-src">— Gemini (Google)</div>
    </div>
  </div>

  <div class="card">
    <div class="section-title">📚 References</div>
    <ul class="refs-list">
      <li>1. Red Hat. (2024). <a href="https://www.redhat.com/en/topics/mobile/what-is-cross-platform-development"><em>What is cross-platform development?</em></a></li>
      <li>2. Microsoft. (2024). <a href="https://learn.microsoft.com/en-us/dotnet/maui/what-is-maui"><em>What is .NET MAUI?</em></a></li>
      <li>3. Flutter. (2024). <a href="https://flutter.dev/docs"><em>Flutter Documentation</em></a></li>
    </ul>
  </div>

  <a class="back-link" href="https://sximi.github.io">🎀 กลับหน้าหลัก</a>

</main>

<footer>🎀 made with ♡ · จันทรัสม์ เต็มทอง · My Melody Theme 🌸</footer>

</div>
