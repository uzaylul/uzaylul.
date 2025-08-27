<!-- ============================ HEADER (animated wave + gradient) ============================ -->
<p align="center">
<svg width="100%" height="220" viewBox="0 0 1200 220" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="g" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%"  stop-color="#f59e0b">
        <animate attributeName="stop-color" values="#f59e0b;#8b5cf6;#06b6d4;#f59e0b" dur="14s" repeatCount="indefinite"/>
      </stop>
      <stop offset="100%" stop-color="#8b5cf6">
        <animate attributeName="stop-color" values="#8b5cf6;#06b6d4;#f59e0b;#8b5cf6" dur="14s" repeatCount="indefinite"/>
      </stop>
    </linearGradient>
    <clipPath id="wave">
      <path d="M0,120 C200,80 300,160 500,120 C700,80 900,160 1200,120 L1200,220 L0,220 Z">
        <animate attributeName="d" dur="10s" repeatCount="indefinite"
          values="
          M0,120 C200,80 300,160 500,120 C700,80 900,160 1200,120 L1200,220 L0,220 Z;
          M0,130 C200,170 300,90 500,130 C700,170 900,90 1200,130 L1200,220 L0,220 Z;
          M0,120 C200,80 300,160 500,120 C700,80 900,160 1200,120 L1200,220 L0,220 Z"/>
      </path>
    </clipPath>
  </defs>
  <rect width="1200" height="220" fill="url(#g)" clip-path="url(#wave)"/>
  <text x="50%" y="48%" dominant-baseline="middle" text-anchor="middle"
        font-size="44" font-family="Inter,Segoe UI,Ubuntu,Helvetica,Arial"
        fill="#ffffff" font-weight="700" letter-spacing=".5px">
    Onur Çelik • uzaylul
    <animate attributeName="letter-spacing" values=".5px;2px;.5px" dur="6s" repeatCount="indefinite"/>
  </text>
  <!-- tiny stars -->
  <g fill="#ffffff" opacity=".35">
    <circle r="2"><animate attributeName="cx" values="50;1150;50" dur="18s" repeatCount="indefinite"/><animate attributeName="cy" values="30;40;30" dur="18s" repeatCount="indefinite"/></circle>
    <circle r="1.6"><animate attributeName="cx" values="300;100;300" dur="12s" repeatCount="indefinite"/><animate attributeName="cy" values="60;20;60" dur="12s" repeatCount="indefinite"/></circle>
  </g>
</svg>
</p>

<!-- ============================ TYPING (pure SVG mask typing) ============================ -->
<p align="center">
<svg width="740" height="40" viewBox="0 0 740 40" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <mask id="cursorMask">
      <rect x="0" y="0" width="740" height="40" fill="white"/>
      <!-- moving black rectangle works as "eraser" to reveal text progressively -->
      <rect id="reveal" x="0" y="0" width="740" height="40" fill="black">
        <animate attributeName="x" values="740;0" dur="3s" fill="freeze"/>
      </rect>
    </mask>
  </defs>
  <g font-family="Fira Code,Consolas,monospace" font-size="18" fill="#22D3EE">
    <text x="10" y="26" mask="url(#cursorMask)">Kelimeler zihnin anahtarıdır.</text>
  </g>
  <!-- blinking cursor -->
  <rect x="10">
    <animate attributeName="x" values="10;570;570" dur="3s" fill="freeze"/>
  </rect>
  <rect width="12" height="22" y="7" fill="#22D3EE">
    <animate attributeName="x" values="10;580;580" dur="3s" fill="freeze"/>
    <animate attributeName="opacity" values="1;0;1" dur="0.9s" repeatCount="indefinite"/>
  </rect>

  <!-- cycle to next lines -->
  <g>
    <animate id="cycle" attributeName="visibility" values="hidden;hidden" dur="4.2s" begin="0s;cycle2.end" fill="freeze"/>
  </g>
</svg>
</p>

<!-- ikinci satır -->
<p align="center">
<svg width="740" height="40" viewBox="0 0 740 40" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <mask id="m2"><rect width="740" height="40" fill="white"/><rect x="740" width="740" height="40" fill="black"><animate attributeName="x" values="740;0" dur="3s" begin="0.2s" fill="freeze"/></rect></mask>
  </defs>
  <text x="10" y="26" font-family="Fira Code,Consolas,monospace" font-size="18" fill="#22D3EE" mask="url(#m2)">
    Üretici &amp; sunucu, hikâye anlatıcısı.
  </text>
  <rect width="12" height="22" y="7" fill="#22D3EE">
    <animate attributeName="x" values="10;620;620" dur="3s" begin="0.2s" fill="freeze"/>
    <animate attributeName="opacity" values="1;0;1" dur="0.9s" repeatCount="indefinite"/>
  </rect>
</svg>
</p>

<!-- üçüncü satır -->
<p align="center">
<svg width="740" height="40" viewBox="0 0 740 40" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <mask id="m3"><rect width="740" height="40" fill="white"/><rect x="740" width="740" height="40" fill="black"><animate attributeName="x" values="740;0" dur="3s" begin="0.4s" fill="freeze"/></rect></mask>
  </defs>
  <text x="10" y="26" font-family="Fira Code,Consolas,monospace" font-size="18" fill="#22D3EE" mask="url(#m3)">
    Mini web araçları, video ve yazı.
  </text>
  <rect width="12" height="22" y="7" fill="#22D3EE">
    <animate attributeName="x" values="10;510;510" dur="3s" begin="0.4s" fill="freeze"/>
    <animate attributeName="opacity" values="1;0;1" dur="0.9s" repeatCount="indefinite"/>
  </rect>
</svg>
</p>

<!-- ============================ SOCIALS (inline white SVG icons, pulsing) ============================ -->
<p align="center">
  <!-- icon button template: dark pill + white logo + pulse -->
  <a href="https://youtube.com/@uzaylul" title="YouTube">
    <svg width="44" height="44" viewBox="0 0 44 44" xmlns="http://www.w3.org/2000/svg">
      <rect x="2" y="2" rx="10" ry="10" width="40" height="40" fill="#0f172a">
        <animate attributeName="opacity" values="1;.85;1" dur="1.6s" repeatCount="indefinite"/>
      </rect>
      <path fill="#fff" transform="translate(10,12) scale(0.9)"
        d="M20.8 3.6c-.2-1-1-1.8-2-2-1.8-.5-8.8-.5-8.8-.5s-7 0-8.8.5c-1 .3-1.8 1-2 2C0 5.4 0 8.3 0 8.3s0 2.9.4 4.7c.2 1 1 1.8 2 2 1.8.5 8.8.5 8.8.5s7 0 8.8-.5c1-.3 1.8-1 2-2 .4-1.8.4-4.7.4-4.7s0-2.9-.4-4.7zM8 12V4.6l6 3.7L8 12z"/>
    </svg>
  </a>
  <a href="https://instagram.com/uzaylul" title="Instagram">
    <svg width="44" height="44" viewBox="0 0 44 44" xmlns="http://www.w3.org/2000/svg">
      <rect x="2" y="2" rx="10" ry="10" width="40" height="40" fill="#0f172a">
        <animate attributeName="opacity" values="1;.85;1" dur="1.7s" repeatCount="indefinite"/>
      </rect>
      <path fill="#fff" transform="translate(10,10) scale(0.9)"
        d="M12 0H4A4 4 0 0 0 0 4v8a4 4 0 0 0 4 4h8a4 4 0 0 0 4-4V4a4 4 0 0 0-4-4zm0 2a2 2 0 0 1 2 2v8a2 2 0 0 1-2 2H4a2 2 0 0 1-2-2V4a2 2 0 0 1 2-2zm-4 3.5A3.5 3.5 0 1 0 11.5 9 3.5 3.5 0 0 0 8 5.5zM13.2 3a1 1 0 1 0 0 2 1 1 0 0 0 0-2z"/>
    </svg>
  </a>
  <a href="https://tiktok.com/@uzaylul" title="TikTok">
    <svg width="44" height="44" viewBox="0 0 44 44" xmlns="http://www.w3.org/2000/svg">
      <rect x="2" y="2" rx="10" ry="10" width="40" height="40" fill="#0f172a">
        <animate attributeName="opacity" values="1;.85;1" dur="1.8s" repeatCount="indefinite"/>
      </rect>
      <path fill="#fff" transform="translate(10,10) scale(0.95)"
        d="M16 0h3c.3 2.6 1.7 4.6 4.2 5.9A9.8 9.8 0 0 0 24 4.4v3.2a12.2 12.2 0 0 1-4-1.4V16a8 8 0 1 1-8-8c.3 0 .6 0 1 .1V11a3.8 3.8 0 1 0 3 3.7V0z"/>
    </svg>
  </a>
  <a href="https://x.com/uzaylul" title="X">
    <svg width="44" height="44" viewBox="0 0 44 44" xmlns="http://www.w3.org/2000/svg">
      <rect x="2" y="2" rx="10" ry="10" width="40" height="40" fill="#0f172a">
        <animate attributeName="opacity" values="1;.85;1" dur="1.6s" begin=".2s" repeatCount="indefinite"/>
      </rect>
      <path fill="#fff" transform="translate(11,11) scale(1.1)"
        d="M12.6 0H9.7L6 5.2 2.8 0H0l5 7.6L0 14h2.9l3.8-5.2L10 14h2.8L7.8 6.6 12.6 0z"/>
    </svg>
  </a>
  <a href="https://reddit.com/r/uzaylul" title="Reddit">
    <svg width="44" height="44" viewBox="0 0 44 44" xmlns="http://www.w3.org/2000/svg">
      <rect x="2" y="2" rx="10" ry="10" width="40" height="40" fill="#0f172a">
        <animate attributeName="opacity" values="1;.85;1" dur="1.9s" repeatCount="indefinite"/>
      </rect>
      <path fill="#fff" transform="translate(8,10) scale(1.05)"
        d="M18.7 12.2c.1.4.1.7.1 1.1 0 4.1-4.3 7.5-9.6 7.5S.6 17.4.6 13.3s4.3-7.5 9.6-7.5c1.7 0 3.4.4 4.8 1.1l1.5-3.6 3.6.8-.3 1.4-2.6-.6-1.1 2.6c2 .9 3.5 2.3 4.1 4.1zM6 12a1.8 1.8 0 1 0 0-3.6 1.8 1.8 0 0 0 0 3.6zm9 0a1.8 1.8 0 1 0 0-3.6 1.8 1.8 0 0 0 0 3.6z"/>
    </svg>
  </a>
  <a href="https://discord.gg/R7q9pbBn9p" title="Discord">
    <svg width="44" height="44" viewBox="0 0 44 44" xmlns="http://www.w3.org/2000/svg">
      <rect x="2" y="2" rx="10" ry="10" width="40" height="40" fill="#0f172a">
        <animate attributeName="opacity" values="1;.85;1" dur="1.7s" begin=".1s" repeatCount="indefinite"/>
      </rect>
      <path fill="#fff" transform="translate(9,11) scale(1.05)"
        d="M20 4.7A16.7 16.7 0 0 0 13.3 3c-.2.4-.4.9-.5 1.4-1.5-.2-3-.2-4.5 0-.1-.5-.3-1-.5-1.4C1.2 3.6 0 4.7 0 4.7 2.6 8.3 5 11 8 12.9c-.3.6-.6 1.1-.8 1.7 1.6.6 3.3.9 5 .9s3.4-.3 5-.9c-.2-.6-.5-1.1-.8-1.7 3-1.9 5.5-4.6 8-8.2zM6.7 11.3a1.7 1.7 0 1 1 0-3.3 1.7 1.7 0 0 1 0 3.3zm10.6 0a1.7 1.7 0 1 1 0-3.3 1.7 1.7 0 0 1 0 3.3z"/>
    </svg>
  </a>
</p>

<!-- ============================ QUICK LINKS (email & all links) ============================ -->
<p align="center">
  <a href="mailto:onurcelikmail@proton.me">
    <img alt="Mail" src="data:image/svg+xml;utf8,
      <svg xmlns='http://www.w3.org/2000/svg' width='110' height='32'>
        <rect rx='6' width='110' height='32' fill='%236d28d9'/>
        <text x='55' y='21' text-anchor='middle' font-family='Inter,Segoe UI' font-size='12' fill='white'>CONTACT</text>
      </svg>">
  </a>
  &nbsp;
  <a href="https://linkler.uzaylul.com/">
    <img alt="All Links" src="data:image/svg+xml;utf8,
      <svg xmlns='http://www.w3.org/2000/svg' width='120' height='32'>
        <rect rx='6' width='120' height='32' fill='%230ea5e9'/>
        <text x='60' y='21' text-anchor='middle' font-family='Inter,Segoe UI' font-size='12' fill='white'>ALL LINKS</text>
      </svg>">
  </a>
</p>

---

### Kısaca
- 🎥 Fikirleri **video** ve **yazıyla** anlatıyorum.  
- 🧰 **Mini web araçları** geliştiriyorum (HTML/CSS/JS).

### Seçme işler
<p align="center">
  • <a href="https://github.com/uzaylul/MultiTools">MultiTools</a>
  &nbsp;&nbsp;• <a href="https://github.com/uzaylul/uzaylul.github.io">Kişisel Site</a>
</p>

### Teknoloji
<p align="center">
  <svg width="28" height="28" viewBox="0 0 24 24"><path fill="#fff" d="M1.5 0h21l-1.9 21.6L12 24l-8.1-2.4L1.5 0Zm4 19.3L12 21l6.5-1.7L19.9 2H4.1l1.4 17.3Z"/></svg>
  &nbsp;<svg width="28" height="28" viewBox="0 0 24 24"><path fill="#fff" d="M1.5 0h21L20.6 21.6L12 24l-8.6-2.4L1.5 0Zm16.6 4.1l-6.1 13.9H8.6L14.7 4.1h3.4Z"/></svg>
  &nbsp;<svg width="28" height="28" viewBox="0 0 24 24"><path fill="#fff" d="M3 3h18v18H3z" fill-opacity=".08"/><path fill="#fff" d="M7 17h2v-6H7v6Zm4 0h2V7h-2v10Zm4 0h2V11h-2v6Z"/></svg>
</p>

<!-- ============================ FOOTER (subtle wave) ============================ -->
<p align="center">
<svg width="100%" height="80" viewBox="0 0 1200 80" xmlns="http://www.w3.org/2000/svg">
  <path fill="#0b1220" d="M0,40 C200,70 300,10 500,40 C700,70 900,10 1200,40 L1200,80 L0,80 Z">
    <animate attributeName="d" dur="8s" repeatCount="indefinite"
      values="M0,40 C200,70 300,10 500,40 C700,70 900,10 1200,40 L1200,80 L0,80 Z;
              M0,35 C200,5 300,75 500,35 C700,5 900,75 1200,35 L1200,80 L0,80 Z;
              M0,40 C200,70 300,10 500,40 C700,70 900,10 1200,40 L1200,80 L0,80 Z"/>
  </path>
</svg>
</p>
