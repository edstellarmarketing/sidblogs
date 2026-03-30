# SKILL CARD SVGs: Skills in Demand in the USA
**Date:** 2026-03-27
**Country:** USA
**Skills:** 12
**SVG Viewport:** 820 x 180px

---

## SVG 1: AI & Machine Learning
**Sector:** Technology
**Palette:** Technology (#0F172A / #1E3A8A / #60A5FA)
**Pattern:** Circuit Traces
**Icon:** Neural Network
**Animation:** Flow Lines + Breathe Nodes
**Prefix:** ai

```html
<svg viewBox="0 0 820 180" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="xMidYMid slice">
  <defs>
    <linearGradient id="ai-bg" x1="0" y1="0" x2="1" y2="1">
      <stop offset="0%" stop-color="#0F172A"/>
      <stop offset="100%" stop-color="#1E3A8A"/>
    </linearGradient>
    <filter id="ai-glow">
      <feGaussianBlur stdDeviation="5" result="blur"/>
      <feMerge><feMergeNode in="blur"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
    <style>
      @keyframes ai-flow1 { 0% { stroke-dashoffset: 220; } 100% { stroke-dashoffset: 0; } }
      @keyframes ai-breathe { 0%,100% { r: 5; opacity: 1; } 50% { r: 7; opacity: 0.5; } }
      @keyframes ai-pulse { 0% { r: 12; opacity: 0.6; } 100% { r: 40; opacity: 0; } }
      .ai-flow { stroke-dasharray: 220; animation: ai-flow1 2.2s linear infinite; }
      .ai-node { animation: ai-breathe 2s ease-in-out infinite; }
      .ai-ring { animation: ai-pulse 2.5s ease-out infinite; }
    </style>
  </defs>
  <rect width="820" height="180" fill="url(#ai-bg)"/>
  <g opacity="0.08" stroke="#60A5FA" stroke-width="0.8" fill="none">
    <path d="M0,40 H90 V20 H170 V40 H260"/>
    <path d="M0,90 H110 V65 H210 V90 H320"/>
    <path d="M0,140 H70 V120 H190 V140 H280"/>
    <path d="M380,25 H480 V50 H570"/>
    <path d="M400,135 H510 V155 H630"/>
    <circle cx="90" cy="40" r="2.5" fill="#60A5FA" stroke="none"/>
    <circle cx="170" cy="20" r="2.5" fill="#60A5FA" stroke="none"/>
    <circle cx="210" cy="65" r="2.5" fill="#60A5FA" stroke="none"/>
    <circle cx="480" cy="50" r="2.5" fill="#60A5FA" stroke="none"/>
  </g>
  <g transform="translate(155,90)">
    <circle cx="-60" cy="-40" r="5" fill="#60A5FA" opacity="0.9" class="ai-node"/>
    <circle cx="-60" cy="0" r="5" fill="#60A5FA" opacity="0.9" class="ai-node" style="animation-delay:0.3s"/>
    <circle cx="-60" cy="40" r="5" fill="#60A5FA" opacity="0.9" class="ai-node" style="animation-delay:0.6s"/>
    <circle cx="0" cy="-50" r="5" fill="#60A5FA" opacity="0.8" class="ai-node" style="animation-delay:0.2s"/>
    <circle cx="0" cy="-15" r="5" fill="#60A5FA" opacity="0.8" class="ai-node" style="animation-delay:0.5s"/>
    <circle cx="0" cy="15" r="5" fill="#60A5FA" opacity="0.8" class="ai-node" style="animation-delay:0.8s"/>
    <circle cx="0" cy="50" r="5" fill="#60A5FA" opacity="0.8" class="ai-node" style="animation-delay:0.4s"/>
    <circle cx="60" cy="-25" r="5" fill="#60A5FA" opacity="0.9" class="ai-node" style="animation-delay:0.7s"/>
    <circle cx="60" cy="25" r="5" fill="#60A5FA" opacity="0.9" class="ai-node" style="animation-delay:1s"/>
    <line x1="-55" y1="-40" x2="-5" y2="-50" stroke="#60A5FA" stroke-width="0.8" opacity="0.3" class="ai-flow"/>
    <line x1="-55" y1="-40" x2="-5" y2="-15" stroke="#60A5FA" stroke-width="0.8" opacity="0.3" class="ai-flow"/>
    <line x1="-55" y1="0" x2="-5" y2="-15" stroke="#60A5FA" stroke-width="0.8" opacity="0.3" class="ai-flow"/>
    <line x1="-55" y1="0" x2="-5" y2="15" stroke="#60A5FA" stroke-width="0.8" opacity="0.3" class="ai-flow"/>
    <line x1="-55" y1="40" x2="-5" y2="15" stroke="#60A5FA" stroke-width="0.8" opacity="0.3" class="ai-flow"/>
    <line x1="-55" y1="40" x2="-5" y2="50" stroke="#60A5FA" stroke-width="0.8" opacity="0.3" class="ai-flow"/>
    <line x1="5" y1="-50" x2="55" y2="-25" stroke="#60A5FA" stroke-width="0.8" opacity="0.3" class="ai-flow"/>
    <line x1="5" y1="-15" x2="55" y2="-25" stroke="#60A5FA" stroke-width="0.8" opacity="0.3" class="ai-flow"/>
    <line x1="5" y1="15" x2="55" y2="25" stroke="#60A5FA" stroke-width="0.8" opacity="0.3" class="ai-flow"/>
    <line x1="5" y1="50" x2="55" y2="25" stroke="#60A5FA" stroke-width="0.8" opacity="0.3" class="ai-flow"/>
  </g>
  <circle cx="155" cy="90" r="12" fill="none" stroke="#60A5FA" stroke-width="1" opacity="0.4" class="ai-ring"/>
  <circle cx="600" cy="50" r="30" fill="#60A5FA" opacity="0.04"/>
  <circle cx="680" cy="120" r="45" fill="#60A5FA" opacity="0.03"/>
  <circle cx="750" cy="60" r="20" fill="#60A5FA" opacity="0.05"/>
</svg>
```

---

## SVG 2: Cybersecurity
**Sector:** Security
**Palette:** Security (#05050F / #1E1B4B / #818CF8)
**Pattern:** Hexagonal Grid
**Icon:** Shield with Lock
**Animation:** Pulse Rings + Scan Bar
**Prefix:** cs

```html
<svg viewBox="0 0 820 180" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="xMidYMid slice">
  <defs>
    <linearGradient id="cs-bg" x1="0" y1="0" x2="1" y2="1">
      <stop offset="0%" stop-color="#05050F"/>
      <stop offset="100%" stop-color="#1E1B4B"/>
    </linearGradient>
    <filter id="cs-glow">
      <feGaussianBlur stdDeviation="4" result="blur"/>
      <feMerge><feMergeNode in="blur"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
    <style>
      @keyframes cs-pulse { 0% { r: 15; opacity: 0.5; } 100% { r: 45; opacity: 0; } }
      @keyframes cs-scan { 0% { transform: translateX(-100px); } 100% { transform: translateX(920px); } }
      @keyframes cs-breathe { 0%,100% { opacity: 0.7; } 50% { opacity: 1; } }
      .cs-ring { animation: cs-pulse 3s ease-out infinite; }
      .cs-scan { animation: cs-scan 4s linear infinite; }
      .cs-shield { animation: cs-breathe 2.5s ease-in-out infinite; }
    </style>
  </defs>
  <rect width="820" height="180" fill="url(#cs-bg)"/>
  <g opacity="0.07" stroke="#818CF8" stroke-width="0.6" fill="none">
    <path d="M20,30 L45,15 L70,30 L70,55 L45,70 L20,55 Z"/>
    <path d="M70,30 L95,15 L120,30 L120,55 L95,70 L70,55 Z"/>
    <path d="M120,30 L145,15 L170,30 L170,55 L145,70 L120,55 Z"/>
    <path d="M45,70 L70,55 L95,70 L95,95 L70,110 L45,95 Z"/>
    <path d="M95,70 L120,55 L145,70 L145,95 L120,110 L95,95 Z"/>
    <path d="M70,110 L95,95 L120,110 L120,135 L95,150 L70,135 Z"/>
    <path d="M350,10 L375,-5 L400,10 L400,35 L375,50 L350,35 Z"/>
    <path d="M400,10 L425,-5 L450,10 L450,35 L425,50 L400,35 Z"/>
    <path d="M500,100 L525,85 L550,100 L550,125 L525,140 L500,125 Z"/>
    <path d="M550,100 L575,85 L600,100 L600,125 L575,140 L550,125 Z"/>
  </g>
  <g transform="translate(160,90)" filter="url(#cs-glow)" class="cs-shield">
    <path d="M0,-50 L35,-35 L35,10 Q35,40 0,55 Q-35,40 -35,10 L-35,-35 Z" fill="none" stroke="#818CF8" stroke-width="2" opacity="0.8"/>
    <rect x="-10" y="-20" width="20" height="28" rx="3" fill="none" stroke="#818CF8" stroke-width="1.5" opacity="0.7"/>
    <circle cx="0" cy="-4" r="5" fill="none" stroke="#818CF8" stroke-width="1.5" opacity="0.7"/>
    <line x1="0" y1="1" x2="0" y2="10" stroke="#818CF8" stroke-width="1.5" opacity="0.7"/>
    <path d="M-8,-20 Q-8,-30 0,-30 Q8,-30 8,-20" fill="none" stroke="#818CF8" stroke-width="1.5" opacity="0.7"/>
  </g>
  <circle cx="160" cy="90" r="15" fill="none" stroke="#818CF8" stroke-width="0.8" opacity="0.4" class="cs-ring"/>
  <circle cx="160" cy="90" r="15" fill="none" stroke="#818CF8" stroke-width="0.8" opacity="0.4" class="cs-ring" style="animation-delay:1s"/>
  <rect x="-100" y="0" width="3" height="180" fill="#818CF8" opacity="0.06" class="cs-scan"/>
  <circle cx="580" cy="40" r="35" fill="#818CF8" opacity="0.03"/>
  <circle cx="700" cy="130" r="50" fill="#818CF8" opacity="0.03"/>
  <circle cx="760" cy="45" r="22" fill="#818CF8" opacity="0.04"/>
</svg>
```

---

## SVG 3: Cloud Computing & DevOps
**Sector:** Technology
**Palette:** Technology (#0F172A / #1E3A8A / #60A5FA)
**Pattern:** Horizontal Lines
**Icon:** Cloud with Nodes
**Animation:** Flow Lines + Breathe Nodes
**Prefix:** cc

```html
<svg viewBox="0 0 820 180" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="xMidYMid slice">
  <defs>
    <linearGradient id="cc-bg" x1="0" y1="0" x2="1" y2="1">
      <stop offset="0%" stop-color="#0F172A"/>
      <stop offset="100%" stop-color="#1E3A8A"/>
    </linearGradient>
    <filter id="cc-glow">
      <feGaussianBlur stdDeviation="5" result="blur"/>
      <feMerge><feMergeNode in="blur"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
    <style>
      @keyframes cc-flow { 0% { stroke-dashoffset: 180; } 100% { stroke-dashoffset: 0; } }
      @keyframes cc-breathe { 0%,100% { r: 4; opacity: 0.9; } 50% { r: 6; opacity: 0.5; } }
      @keyframes cc-float { 0%,100% { transform: translateY(0); } 50% { transform: translateY(-4px); } }
      .cc-line { stroke-dasharray: 180; animation: cc-flow 2.5s linear infinite; }
      .cc-node { animation: cc-breathe 2s ease-in-out infinite; }
      .cc-cloud { animation: cc-float 3s ease-in-out infinite; }
    </style>
  </defs>
  <rect width="820" height="180" fill="url(#cc-bg)"/>
  <g opacity="0.06" stroke="#60A5FA" stroke-width="0.5">
    <line x1="0" y1="20" x2="820" y2="20"/>
    <line x1="0" y1="45" x2="820" y2="45"/>
    <line x1="0" y1="70" x2="820" y2="70"/>
    <line x1="0" y1="95" x2="820" y2="95"/>
    <line x1="0" y1="120" x2="820" y2="120"/>
    <line x1="0" y1="145" x2="820" y2="145"/>
    <line x1="0" y1="170" x2="820" y2="170"/>
  </g>
  <g transform="translate(155,80)" filter="url(#cc-glow)" class="cc-cloud">
    <path d="M-40,15 Q-40,-15 -15,-15 Q-10,-35 15,-35 Q40,-35 45,-15 Q65,-15 65,10 Q65,25 50,25 L-30,25 Q-40,25 -40,15 Z" fill="none" stroke="#60A5FA" stroke-width="1.8" opacity="0.8"/>
    <circle cx="-10" cy="45" r="4" fill="#60A5FA" opacity="0.7" class="cc-node"/>
    <circle cx="20" cy="55" r="4" fill="#60A5FA" opacity="0.7" class="cc-node" style="animation-delay:0.4s"/>
    <circle cx="50" cy="45" r="4" fill="#60A5FA" opacity="0.7" class="cc-node" style="animation-delay:0.8s"/>
    <line x1="-10" y1="25" x2="-10" y2="41" stroke="#60A5FA" stroke-width="0.8" opacity="0.4" class="cc-line"/>
    <line x1="20" y1="25" x2="20" y2="51" stroke="#60A5FA" stroke-width="0.8" opacity="0.4" class="cc-line"/>
    <line x1="45" y1="25" x2="50" y2="41" stroke="#60A5FA" stroke-width="0.8" opacity="0.4" class="cc-line"/>
    <line x1="-10" y1="45" x2="20" y2="55" stroke="#60A5FA" stroke-width="0.6" opacity="0.3" class="cc-line"/>
    <line x1="20" y1="55" x2="50" y2="45" stroke="#60A5FA" stroke-width="0.6" opacity="0.3" class="cc-line"/>
  </g>
  <circle cx="590" cy="55" r="32" fill="#60A5FA" opacity="0.04"/>
  <circle cx="690" cy="125" r="48" fill="#60A5FA" opacity="0.03"/>
  <circle cx="770" cy="50" r="18" fill="#60A5FA" opacity="0.05"/>
</svg>
```

---

## SVG 4: Data Science & Analytics
**Sector:** Analytics
**Palette:** Analytics (#0F1629 / #1E2D6B / #818CF8)
**Pattern:** Dot Grid
**Icon:** Bar Chart
**Animation:** Pulse Rings + Breathe Nodes
**Prefix:** ds

```html
<svg viewBox="0 0 820 180" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="xMidYMid slice">
  <defs>
    <linearGradient id="ds-bg" x1="0" y1="0" x2="1" y2="1">
      <stop offset="0%" stop-color="#0F1629"/>
      <stop offset="100%" stop-color="#1E2D6B"/>
    </linearGradient>
    <filter id="ds-glow">
      <feGaussianBlur stdDeviation="4" result="blur"/>
      <feMerge><feMergeNode in="blur"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
    <style>
      @keyframes ds-grow { 0% { transform: scaleY(0); } 100% { transform: scaleY(1); } }
      @keyframes ds-pulse { 0% { r: 10; opacity: 0.5; } 100% { r: 35; opacity: 0; } }
      @keyframes ds-breathe { 0%,100% { opacity: 0.8; } 50% { opacity: 1; } }
      .ds-bar { transform-origin: bottom; animation: ds-grow 1.5s ease-out forwards; }
      .ds-ring { animation: ds-pulse 2.8s ease-out infinite; }
      .ds-glow { animation: ds-breathe 2s ease-in-out infinite; }
    </style>
  </defs>
  <rect width="820" height="180" fill="url(#ds-bg)"/>
  <g opacity="0.06" fill="#818CF8">
    <circle cx="30" cy="20" r="1.2"/><circle cx="70" cy="20" r="1.2"/><circle cx="110" cy="20" r="1.2"/><circle cx="150" cy="20" r="1.2"/><circle cx="190" cy="20" r="1.2"/><circle cx="230" cy="20" r="1.2"/>
    <circle cx="30" cy="50" r="1.2"/><circle cx="70" cy="50" r="1.2"/><circle cx="110" cy="50" r="1.2"/><circle cx="150" cy="50" r="1.2"/><circle cx="190" cy="50" r="1.2"/><circle cx="230" cy="50" r="1.2"/>
    <circle cx="30" cy="80" r="1.2"/><circle cx="70" cy="80" r="1.2"/><circle cx="110" cy="80" r="1.2"/><circle cx="150" cy="80" r="1.2"/><circle cx="190" cy="80" r="1.2"/><circle cx="230" cy="80" r="1.2"/>
    <circle cx="30" cy="110" r="1.2"/><circle cx="70" cy="110" r="1.2"/><circle cx="110" cy="110" r="1.2"/><circle cx="150" cy="110" r="1.2"/><circle cx="190" cy="110" r="1.2"/><circle cx="230" cy="110" r="1.2"/>
    <circle cx="30" cy="140" r="1.2"/><circle cx="70" cy="140" r="1.2"/><circle cx="110" cy="140" r="1.2"/><circle cx="150" cy="140" r="1.2"/><circle cx="190" cy="140" r="1.2"/><circle cx="230" cy="140" r="1.2"/>
    <circle cx="30" cy="170" r="1.2"/><circle cx="70" cy="170" r="1.2"/><circle cx="110" cy="170" r="1.2"/><circle cx="150" cy="170" r="1.2"/><circle cx="190" cy="170" r="1.2"/><circle cx="230" cy="170" r="1.2"/>
    <circle cx="500" cy="30" r="1.2"/><circle cx="540" cy="30" r="1.2"/><circle cx="580" cy="30" r="1.2"/>
    <circle cx="500" cy="60" r="1.2"/><circle cx="540" cy="60" r="1.2"/><circle cx="580" cy="60" r="1.2"/>
    <circle cx="500" cy="90" r="1.2"/><circle cx="540" cy="90" r="1.2"/><circle cx="580" cy="90" r="1.2"/>
  </g>
  <g transform="translate(120,140)" filter="url(#ds-glow)" class="ds-glow">
    <line x1="0" y1="0" x2="120" y2="0" stroke="#818CF8" stroke-width="1" opacity="0.4"/>
    <line x1="0" y1="0" x2="0" y2="-100" stroke="#818CF8" stroke-width="1" opacity="0.4"/>
    <rect x="10" y="-60" width="16" height="60" rx="2" fill="#818CF8" opacity="0.5" class="ds-bar"/>
    <rect x="35" y="-85" width="16" height="85" rx="2" fill="#818CF8" opacity="0.6" class="ds-bar" style="animation-delay:0.2s"/>
    <rect x="60" y="-45" width="16" height="45" rx="2" fill="#818CF8" opacity="0.5" class="ds-bar" style="animation-delay:0.4s"/>
    <rect x="85" y="-75" width="16" height="75" rx="2" fill="#818CF8" opacity="0.65" class="ds-bar" style="animation-delay:0.6s"/>
  </g>
  <circle cx="170" cy="90" r="10" fill="none" stroke="#818CF8" stroke-width="0.8" opacity="0.3" class="ds-ring"/>
  <circle cx="610" cy="60" r="35" fill="#818CF8" opacity="0.04"/>
  <circle cx="710" cy="130" r="45" fill="#818CF8" opacity="0.03"/>
  <circle cx="770" cy="55" r="20" fill="#818CF8" opacity="0.05"/>
</svg>
```

---

## SVG 5: Software Engineering / Full-Stack
**Sector:** Technology
**Palette:** Technology (#0F172A / #1E3A8A / #60A5FA)
**Pattern:** Diagonal Lines
**Icon:** Code Brackets
**Animation:** Flow Lines + Pulse Rings
**Prefix:** fs

```html
<svg viewBox="0 0 820 180" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="xMidYMid slice">
  <defs>
    <linearGradient id="fs-bg" x1="0" y1="0" x2="1" y2="1">
      <stop offset="0%" stop-color="#0F172A"/>
      <stop offset="100%" stop-color="#1E3A8A"/>
    </linearGradient>
    <filter id="fs-glow">
      <feGaussianBlur stdDeviation="5" result="blur"/>
      <feMerge><feMergeNode in="blur"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
    <style>
      @keyframes fs-flow { 0% { stroke-dashoffset: 150; } 100% { stroke-dashoffset: 0; } }
      @keyframes fs-pulse { 0% { r: 12; opacity: 0.5; } 100% { r: 38; opacity: 0; } }
      @keyframes fs-blink { 0%,100% { opacity: 1; } 50% { opacity: 0.3; } }
      .fs-code { stroke-dasharray: 150; animation: fs-flow 2s linear infinite; }
      .fs-ring { animation: fs-pulse 2.8s ease-out infinite; }
      .fs-cursor { animation: fs-blink 1s step-end infinite; }
    </style>
  </defs>
  <rect width="820" height="180" fill="url(#fs-bg)"/>
  <g opacity="0.06" stroke="#60A5FA" stroke-width="0.5">
    <line x1="0" y1="0" x2="60" y2="180"/>
    <line x1="40" y1="0" x2="100" y2="180"/>
    <line x1="80" y1="0" x2="140" y2="180"/>
    <line x1="120" y1="0" x2="180" y2="180"/>
    <line x1="160" y1="0" x2="220" y2="180"/>
    <line x1="200" y1="0" x2="260" y2="180"/>
    <line x1="240" y1="0" x2="300" y2="180"/>
    <line x1="450" y1="0" x2="510" y2="180"/>
    <line x1="490" y1="0" x2="550" y2="180"/>
    <line x1="530" y1="0" x2="590" y2="180"/>
  </g>
  <g transform="translate(155,90)" filter="url(#fs-glow)">
    <path d="M-35,-35 L-55,0 L-35,35" fill="none" stroke="#60A5FA" stroke-width="2.5" opacity="0.8" stroke-linecap="round" class="fs-code"/>
    <path d="M35,-35 L55,0 L35,35" fill="none" stroke="#60A5FA" stroke-width="2.5" opacity="0.8" stroke-linecap="round" class="fs-code" style="animation-delay:0.5s"/>
    <line x1="-12" y1="-30" x2="12" y2="30" stroke="#60A5FA" stroke-width="2" opacity="0.6"/>
    <rect x="62" y="-8" width="2" height="16" fill="#60A5FA" opacity="0.7" class="fs-cursor"/>
    <line x1="68" y1="-4" x2="100" y2="-4" stroke="#60A5FA" stroke-width="1.5" opacity="0.3"/>
    <line x1="68" y1="4" x2="90" y2="4" stroke="#60A5FA" stroke-width="1.5" opacity="0.2"/>
  </g>
  <circle cx="155" cy="90" r="12" fill="none" stroke="#60A5FA" stroke-width="0.8" opacity="0.3" class="fs-ring"/>
  <circle cx="600" cy="45" r="30" fill="#60A5FA" opacity="0.04"/>
  <circle cx="700" cy="130" r="42" fill="#60A5FA" opacity="0.03"/>
  <circle cx="760" cy="55" r="22" fill="#60A5FA" opacity="0.05"/>
</svg>
```

---

## SVG 6: Healthcare / Registered Nursing
**Sector:** Healthcare
**Palette:** Healthcare (#051F12 / #064E3B / #34D399)
**Pattern:** Dot Grid
**Icon:** Medical Cross with Pulse
**Animation:** Pulse Rings + Flow Lines
**Prefix:** hc

```html
<svg viewBox="0 0 820 180" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="xMidYMid slice">
  <defs>
    <linearGradient id="hc-bg" x1="0" y1="0" x2="1" y2="1">
      <stop offset="0%" stop-color="#051F12"/>
      <stop offset="100%" stop-color="#064E3B"/>
    </linearGradient>
    <filter id="hc-glow">
      <feGaussianBlur stdDeviation="5" result="blur"/>
      <feMerge><feMergeNode in="blur"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
    <style>
      @keyframes hc-pulse { 0% { r: 14; opacity: 0.5; } 100% { r: 42; opacity: 0; } }
      @keyframes hc-heartbeat { 0%,100% { transform: scale(1); } 15% { transform: scale(1.08); } 30% { transform: scale(1); } 45% { transform: scale(1.05); } }
      @keyframes hc-ecg { 0% { stroke-dashoffset: 300; } 100% { stroke-dashoffset: 0; } }
      .hc-ring { animation: hc-pulse 2.5s ease-out infinite; }
      .hc-cross { transform-origin: center; animation: hc-heartbeat 1.5s ease-in-out infinite; }
      .hc-ecg { stroke-dasharray: 300; animation: hc-ecg 2s linear infinite; }
    </style>
  </defs>
  <rect width="820" height="180" fill="url(#hc-bg)"/>
  <g opacity="0.06" fill="#34D399">
    <circle cx="30" cy="25" r="1.2"/><circle cx="65" cy="25" r="1.2"/><circle cx="100" cy="25" r="1.2"/><circle cx="135" cy="25" r="1.2"/><circle cx="170" cy="25" r="1.2"/><circle cx="205" cy="25" r="1.2"/>
    <circle cx="30" cy="55" r="1.2"/><circle cx="65" cy="55" r="1.2"/><circle cx="100" cy="55" r="1.2"/><circle cx="135" cy="55" r="1.2"/><circle cx="170" cy="55" r="1.2"/><circle cx="205" cy="55" r="1.2"/>
    <circle cx="30" cy="85" r="1.2"/><circle cx="65" cy="85" r="1.2"/><circle cx="100" cy="85" r="1.2"/><circle cx="135" cy="85" r="1.2"/><circle cx="170" cy="85" r="1.2"/><circle cx="205" cy="85" r="1.2"/>
    <circle cx="30" cy="115" r="1.2"/><circle cx="65" cy="115" r="1.2"/><circle cx="100" cy="115" r="1.2"/><circle cx="135" cy="115" r="1.2"/><circle cx="170" cy="115" r="1.2"/><circle cx="205" cy="115" r="1.2"/>
    <circle cx="30" cy="145" r="1.2"/><circle cx="65" cy="145" r="1.2"/><circle cx="100" cy="145" r="1.2"/><circle cx="135" cy="145" r="1.2"/><circle cx="170" cy="145" r="1.2"/><circle cx="205" cy="145" r="1.2"/>
    <circle cx="500" cy="40" r="1.2"/><circle cx="535" cy="40" r="1.2"/><circle cx="570" cy="40" r="1.2"/>
    <circle cx="500" cy="70" r="1.2"/><circle cx="535" cy="70" r="1.2"/><circle cx="570" cy="70" r="1.2"/>
  </g>
  <g transform="translate(150,90)" filter="url(#hc-glow)">
    <g class="hc-cross">
      <rect x="-8" y="-25" width="16" height="50" rx="3" fill="#34D399" opacity="0.7"/>
      <rect x="-25" y="-8" width="50" height="16" rx="3" fill="#34D399" opacity="0.7"/>
    </g>
    <path d="M40,0 L60,0 L68,-20 L76,20 L84,-30 L92,15 L100,0 L120,0" fill="none" stroke="#34D399" stroke-width="1.8" opacity="0.6" stroke-linecap="round" class="hc-ecg"/>
  </g>
  <circle cx="150" cy="90" r="14" fill="none" stroke="#34D399" stroke-width="0.8" opacity="0.3" class="hc-ring"/>
  <circle cx="150" cy="90" r="14" fill="none" stroke="#34D399" stroke-width="0.8" opacity="0.3" class="hc-ring" style="animation-delay:0.8s"/>
  <circle cx="600" cy="50" r="30" fill="#34D399" opacity="0.04"/>
  <circle cx="700" cy="125" r="45" fill="#34D399" opacity="0.03"/>
  <circle cx="760" cy="55" r="20" fill="#34D399" opacity="0.05"/>
</svg>
```

---

## SVG 7: Generative AI & Prompt Engineering
**Sector:** Technology
**Palette:** Technology (#0F172A / #1E3A8A / #60A5FA)
**Pattern:** Circuit Traces
**Icon:** Chip/Processor
**Animation:** Scan Bar + Breathe Nodes
**Prefix:** ga

```html
<svg viewBox="0 0 820 180" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="xMidYMid slice">
  <defs>
    <linearGradient id="ga-bg" x1="0" y1="0" x2="1" y2="1">
      <stop offset="0%" stop-color="#0F172A"/>
      <stop offset="100%" stop-color="#1E3A8A"/>
    </linearGradient>
    <filter id="ga-glow">
      <feGaussianBlur stdDeviation="4" result="blur"/>
      <feMerge><feMergeNode in="blur"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
    <style>
      @keyframes ga-scan { 0% { transform: translateY(-90px); } 100% { transform: translateY(90px); } }
      @keyframes ga-breathe { 0%,100% { opacity: 0.6; } 50% { opacity: 1; } }
      @keyframes ga-flow { 0% { stroke-dashoffset: 100; } 100% { stroke-dashoffset: 0; } }
      .ga-scan { animation: ga-scan 3s ease-in-out infinite alternate; }
      .ga-chip { animation: ga-breathe 2s ease-in-out infinite; }
      .ga-trace { stroke-dasharray: 100; animation: ga-flow 2s linear infinite; }
    </style>
  </defs>
  <rect width="820" height="180" fill="url(#ga-bg)"/>
  <g opacity="0.08" stroke="#60A5FA" stroke-width="0.8" fill="none">
    <path d="M10,35 H75 V20 H150 V35 H230"/>
    <path d="M10,85 H100 V60 H185 V85 H280"/>
    <path d="M10,140 H55 V120 H170 V140 H250"/>
    <path d="M420,25 H510 V45 H590"/>
    <path d="M430,140 H530 V160 H640"/>
    <circle cx="75" cy="35" r="2" fill="#60A5FA" stroke="none"/>
    <circle cx="150" cy="20" r="2" fill="#60A5FA" stroke="none"/>
    <circle cx="185" cy="60" r="2" fill="#60A5FA" stroke="none"/>
  </g>
  <g transform="translate(160,90)" filter="url(#ga-glow)" class="ga-chip">
    <rect x="-28" y="-28" width="56" height="56" rx="6" fill="none" stroke="#60A5FA" stroke-width="2" opacity="0.8"/>
    <rect x="-16" y="-16" width="32" height="32" rx="3" fill="#60A5FA" opacity="0.15"/>
    <circle cx="0" cy="0" r="6" fill="#60A5FA" opacity="0.5"/>
    <line x1="-28" y1="-14" x2="-42" y2="-14" stroke="#60A5FA" stroke-width="1.5" opacity="0.5" class="ga-trace"/>
    <line x1="-28" y1="0" x2="-42" y2="0" stroke="#60A5FA" stroke-width="1.5" opacity="0.5" class="ga-trace"/>
    <line x1="-28" y1="14" x2="-42" y2="14" stroke="#60A5FA" stroke-width="1.5" opacity="0.5" class="ga-trace"/>
    <line x1="28" y1="-14" x2="42" y2="-14" stroke="#60A5FA" stroke-width="1.5" opacity="0.5" class="ga-trace"/>
    <line x1="28" y1="0" x2="42" y2="0" stroke="#60A5FA" stroke-width="1.5" opacity="0.5" class="ga-trace"/>
    <line x1="28" y1="14" x2="42" y2="14" stroke="#60A5FA" stroke-width="1.5" opacity="0.5" class="ga-trace"/>
    <line x1="-14" y1="-28" x2="-14" y2="-42" stroke="#60A5FA" stroke-width="1.5" opacity="0.5" class="ga-trace"/>
    <line x1="0" y1="-28" x2="0" y2="-42" stroke="#60A5FA" stroke-width="1.5" opacity="0.5" class="ga-trace"/>
    <line x1="14" y1="-28" x2="14" y2="-42" stroke="#60A5FA" stroke-width="1.5" opacity="0.5" class="ga-trace"/>
    <line x1="-14" y1="28" x2="-14" y2="42" stroke="#60A5FA" stroke-width="1.5" opacity="0.5" class="ga-trace"/>
    <line x1="0" y1="28" x2="0" y2="42" stroke="#60A5FA" stroke-width="1.5" opacity="0.5" class="ga-trace"/>
    <line x1="14" y1="28" x2="14" y2="42" stroke="#60A5FA" stroke-width="1.5" opacity="0.5" class="ga-trace"/>
  </g>
  <rect x="100" y="0" width="120" height="2" fill="#60A5FA" opacity="0.05" rx="1" class="ga-scan"/>
  <circle cx="590" cy="45" r="28" fill="#60A5FA" opacity="0.04"/>
  <circle cx="690" cy="130" r="50" fill="#60A5FA" opacity="0.03"/>
  <circle cx="770" cy="50" r="18" fill="#60A5FA" opacity="0.05"/>
</svg>
```

---

## SVG 8: Project Management & Agile
**Sector:** Custom
**Palette:** Custom (#0F172A / #2D3A6B / #A78BFA)
**Pattern:** Horizontal Lines
**Icon:** Kanban Board
**Animation:** Flow Lines + Breathe Nodes
**Prefix:** pm

```html
<svg viewBox="0 0 820 180" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="xMidYMid slice">
  <defs>
    <linearGradient id="pm-bg" x1="0" y1="0" x2="1" y2="1">
      <stop offset="0%" stop-color="#0F172A"/>
      <stop offset="100%" stop-color="#2D3A6B"/>
    </linearGradient>
    <filter id="pm-glow">
      <feGaussianBlur stdDeviation="4" result="blur"/>
      <feMerge><feMergeNode in="blur"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
    <style>
      @keyframes pm-slide { 0% { transform: translateX(-5px); opacity: 0.4; } 50% { transform: translateX(5px); opacity: 0.8; } 100% { transform: translateX(-5px); opacity: 0.4; } }
      @keyframes pm-breathe { 0%,100% { opacity: 0.5; } 50% { opacity: 0.9; } }
      @keyframes pm-pulse { 0% { r: 10; opacity: 0.4; } 100% { r: 30; opacity: 0; } }
      .pm-card { animation: pm-slide 3s ease-in-out infinite; }
      .pm-board { animation: pm-breathe 2.5s ease-in-out infinite; }
      .pm-ring { animation: pm-pulse 2.8s ease-out infinite; }
    </style>
  </defs>
  <rect width="820" height="180" fill="url(#pm-bg)"/>
  <g opacity="0.06" stroke="#A78BFA" stroke-width="0.5">
    <line x1="0" y1="18" x2="820" y2="18"/>
    <line x1="0" y1="42" x2="820" y2="42"/>
    <line x1="0" y1="66" x2="820" y2="66"/>
    <line x1="0" y1="90" x2="820" y2="90"/>
    <line x1="0" y1="114" x2="820" y2="114"/>
    <line x1="0" y1="138" x2="820" y2="138"/>
    <line x1="0" y1="162" x2="820" y2="162"/>
  </g>
  <g transform="translate(120,40)" filter="url(#pm-glow)" class="pm-board">
    <rect x="0" y="0" width="100" height="100" rx="4" fill="none" stroke="#A78BFA" stroke-width="1.5" opacity="0.6"/>
    <line x1="34" y1="0" x2="34" y2="100" stroke="#A78BFA" stroke-width="0.8" opacity="0.3"/>
    <line x1="67" y1="0" x2="67" y2="100" stroke="#A78BFA" stroke-width="0.8" opacity="0.3"/>
    <rect x="5" y="12" width="24" height="14" rx="2" fill="#A78BFA" opacity="0.4" class="pm-card"/>
    <rect x="5" y="32" width="24" height="14" rx="2" fill="#A78BFA" opacity="0.3" class="pm-card" style="animation-delay:0.5s"/>
    <rect x="39" y="12" width="24" height="14" rx="2" fill="#A78BFA" opacity="0.5" class="pm-card" style="animation-delay:1s"/>
    <rect x="39" y="32" width="24" height="14" rx="2" fill="#A78BFA" opacity="0.35" class="pm-card" style="animation-delay:1.5s"/>
    <rect x="72" y="12" width="24" height="14" rx="2" fill="#A78BFA" opacity="0.55" class="pm-card" style="animation-delay:0.7s"/>
    <rect x="5" y="55" width="24" height="14" rx="2" fill="#A78BFA" opacity="0.25" class="pm-card" style="animation-delay:2s"/>
    <rect x="72" y="32" width="24" height="14" rx="2" fill="#A78BFA" opacity="0.3" class="pm-card" style="animation-delay:1.2s"/>
  </g>
  <circle cx="170" cy="90" r="10" fill="none" stroke="#A78BFA" stroke-width="0.8" opacity="0.3" class="pm-ring"/>
  <circle cx="590" cy="50" r="32" fill="#A78BFA" opacity="0.04"/>
  <circle cx="690" cy="125" r="48" fill="#A78BFA" opacity="0.03"/>
  <circle cx="770" cy="50" r="20" fill="#A78BFA" opacity="0.05"/>
</svg>
```

---

## SVG 9: Skilled Trades (Electrician/HVAC)
**Sector:** Trades
**Palette:** Trades (#1C0500 / #78350F / #FBBF24)
**Pattern:** Diagonal Lines
**Icon:** Bolt/Lightning
**Animation:** Pulse Rings + Flow Lines
**Prefix:** tr

```html
<svg viewBox="0 0 820 180" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="xMidYMid slice">
  <defs>
    <linearGradient id="tr-bg" x1="0" y1="0" x2="1" y2="1">
      <stop offset="0%" stop-color="#1C0500"/>
      <stop offset="100%" stop-color="#78350F"/>
    </linearGradient>
    <filter id="tr-glow">
      <feGaussianBlur stdDeviation="6" result="blur"/>
      <feMerge><feMergeNode in="blur"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
    <style>
      @keyframes tr-flash { 0%,100% { opacity: 0.7; } 50% { opacity: 1; } 75% { opacity: 0.4; } }
      @keyframes tr-pulse { 0% { r: 12; opacity: 0.5; } 100% { r: 40; opacity: 0; } }
      @keyframes tr-arc { 0% { stroke-dashoffset: 80; } 100% { stroke-dashoffset: 0; } }
      .tr-bolt { animation: tr-flash 1.5s ease-in-out infinite; }
      .tr-ring { animation: tr-pulse 2.5s ease-out infinite; }
      .tr-arc { stroke-dasharray: 80; animation: tr-arc 1.8s linear infinite; }
    </style>
  </defs>
  <rect width="820" height="180" fill="url(#tr-bg)"/>
  <g opacity="0.07" stroke="#FBBF24" stroke-width="0.5">
    <line x1="0" y1="0" x2="60" y2="180"/>
    <line x1="45" y1="0" x2="105" y2="180"/>
    <line x1="90" y1="0" x2="150" y2="180"/>
    <line x1="135" y1="0" x2="195" y2="180"/>
    <line x1="180" y1="0" x2="240" y2="180"/>
    <line x1="225" y1="0" x2="285" y2="180"/>
    <line x1="460" y1="0" x2="520" y2="180"/>
    <line x1="505" y1="0" x2="565" y2="180"/>
    <line x1="550" y1="0" x2="610" y2="180"/>
  </g>
  <g transform="translate(155,90)" filter="url(#tr-glow)" class="tr-bolt">
    <polygon points="-5,-50 10,-8 0,-8 15,50 -10,5 2,5 -15,-50" fill="#FBBF24" opacity="0.8"/>
    <path d="M-30,-20 Q-45,0 -30,20" fill="none" stroke="#FBBF24" stroke-width="1" opacity="0.3" class="tr-arc"/>
    <path d="M30,-20 Q45,0 30,20" fill="none" stroke="#FBBF24" stroke-width="1" opacity="0.3" class="tr-arc" style="animation-delay:0.5s"/>
    <path d="M-40,-30 Q-60,0 -40,30" fill="none" stroke="#FBBF24" stroke-width="0.8" opacity="0.2" class="tr-arc" style="animation-delay:1s"/>
    <path d="M40,-30 Q60,0 40,30" fill="none" stroke="#FBBF24" stroke-width="0.8" opacity="0.2" class="tr-arc" style="animation-delay:1.5s"/>
  </g>
  <circle cx="155" cy="90" r="12" fill="none" stroke="#FBBF24" stroke-width="0.8" opacity="0.3" class="tr-ring"/>
  <circle cx="155" cy="90" r="12" fill="none" stroke="#FBBF24" stroke-width="0.8" opacity="0.3" class="tr-ring" style="animation-delay:0.8s"/>
  <circle cx="580" cy="45" r="30" fill="#FBBF24" opacity="0.04"/>
  <circle cx="700" cy="130" r="50" fill="#FBBF24" opacity="0.03"/>
  <circle cx="770" cy="50" r="18" fill="#FBBF24" opacity="0.05"/>
</svg>
```

---

## SVG 10: Clean Energy & Sustainability
**Sector:** Green Energy
**Palette:** Green Energy (#031A0A / #14532D / #4ADE80)
**Pattern:** Diagonal Lines
**Icon:** Leaf/Turbine
**Animation:** Flow Lines + Breathe Nodes
**Prefix:** ge

```html
<svg viewBox="0 0 820 180" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="xMidYMid slice">
  <defs>
    <linearGradient id="ge-bg" x1="0" y1="0" x2="1" y2="1">
      <stop offset="0%" stop-color="#031A0A"/>
      <stop offset="100%" stop-color="#14532D"/>
    </linearGradient>
    <filter id="ge-glow">
      <feGaussianBlur stdDeviation="5" result="blur"/>
      <feMerge><feMergeNode in="blur"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
    <style>
      @keyframes ge-spin { 0% { transform: rotate(0deg); } 100% { transform: rotate(360deg); } }
      @keyframes ge-breathe { 0%,100% { opacity: 0.6; } 50% { opacity: 1; } }
      @keyframes ge-sway { 0%,100% { transform: rotate(-3deg); } 50% { transform: rotate(3deg); } }
      .ge-turbine { transform-origin: center; animation: ge-spin 6s linear infinite; }
      .ge-leaf { transform-origin: 130px 100px; animation: ge-sway 3s ease-in-out infinite; }
      .ge-glow { animation: ge-breathe 2.5s ease-in-out infinite; }
    </style>
  </defs>
  <rect width="820" height="180" fill="url(#ge-bg)"/>
  <g opacity="0.06" stroke="#4ADE80" stroke-width="0.5">
    <line x1="0" y1="0" x2="55" y2="180"/>
    <line x1="40" y1="0" x2="95" y2="180"/>
    <line x1="80" y1="0" x2="135" y2="180"/>
    <line x1="120" y1="0" x2="175" y2="180"/>
    <line x1="160" y1="0" x2="215" y2="180"/>
    <line x1="200" y1="0" x2="255" y2="180"/>
    <line x1="440" y1="0" x2="495" y2="180"/>
    <line x1="480" y1="0" x2="535" y2="180"/>
    <line x1="520" y1="0" x2="575" y2="180"/>
  </g>
  <g filter="url(#ge-glow)">
    <g class="ge-leaf">
      <path d="M130,55 Q170,45 190,65 Q195,90 165,100 Q140,105 130,100 Q120,90 130,55 Z" fill="#4ADE80" opacity="0.25"/>
      <path d="M130,55 Q150,75 165,100" fill="none" stroke="#4ADE80" stroke-width="1" opacity="0.5"/>
      <path d="M145,65 Q155,80 155,90" fill="none" stroke="#4ADE80" stroke-width="0.6" opacity="0.3"/>
    </g>
    <g transform="translate(170,115)">
      <line x1="0" y1="0" x2="0" y2="40" stroke="#4ADE80" stroke-width="2" opacity="0.5"/>
      <g class="ge-turbine">
        <line x1="0" y1="0" x2="0" y2="-28" stroke="#4ADE80" stroke-width="2" opacity="0.6"/>
        <line x1="0" y1="0" x2="24" y2="14" stroke="#4ADE80" stroke-width="2" opacity="0.6"/>
        <line x1="0" y1="0" x2="-24" y2="14" stroke="#4ADE80" stroke-width="2" opacity="0.6"/>
        <circle cx="0" cy="-28" r="3" fill="#4ADE80" opacity="0.5"/>
        <circle cx="24" cy="14" r="3" fill="#4ADE80" opacity="0.5"/>
        <circle cx="-24" cy="14" r="3" fill="#4ADE80" opacity="0.5"/>
      </g>
      <circle cx="0" cy="0" r="4" fill="#4ADE80" opacity="0.6"/>
    </g>
  </g>
  <circle cx="600" cy="50" r="32" fill="#4ADE80" opacity="0.04"/>
  <circle cx="700" cy="125" r="48" fill="#4ADE80" opacity="0.03"/>
  <circle cx="770" cy="55" r="20" fill="#4ADE80" opacity="0.05"/>
</svg>
```

---

## SVG 11: Financial Analysis & Risk Management
**Sector:** Finance
**Palette:** Finance (#0A0F1E / #1E3A5F / #38BDF8)
**Pattern:** Dot Grid
**Icon:** Chart Trend Line
**Animation:** Flow Lines + Breathe Nodes
**Prefix:** fi

```html
<svg viewBox="0 0 820 180" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="xMidYMid slice">
  <defs>
    <linearGradient id="fi-bg" x1="0" y1="0" x2="1" y2="1">
      <stop offset="0%" stop-color="#0A0F1E"/>
      <stop offset="100%" stop-color="#1E3A5F"/>
    </linearGradient>
    <filter id="fi-glow">
      <feGaussianBlur stdDeviation="4" result="blur"/>
      <feMerge><feMergeNode in="blur"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
    <style>
      @keyframes fi-draw { 0% { stroke-dashoffset: 250; } 100% { stroke-dashoffset: 0; } }
      @keyframes fi-breathe { 0%,100% { r: 3; opacity: 0.8; } 50% { r: 5; opacity: 0.4; } }
      @keyframes fi-pulse { 0% { r: 10; opacity: 0.5; } 100% { r: 35; opacity: 0; } }
      .fi-trend { stroke-dasharray: 250; animation: fi-draw 3s ease-in-out infinite; }
      .fi-dot { animation: fi-breathe 2s ease-in-out infinite; }
      .fi-ring { animation: fi-pulse 2.8s ease-out infinite; }
    </style>
  </defs>
  <rect width="820" height="180" fill="url(#fi-bg)"/>
  <g opacity="0.06" fill="#38BDF8">
    <circle cx="25" cy="20" r="1.2"/><circle cx="60" cy="20" r="1.2"/><circle cx="95" cy="20" r="1.2"/><circle cx="130" cy="20" r="1.2"/><circle cx="165" cy="20" r="1.2"/><circle cx="200" cy="20" r="1.2"/>
    <circle cx="25" cy="50" r="1.2"/><circle cx="60" cy="50" r="1.2"/><circle cx="95" cy="50" r="1.2"/><circle cx="130" cy="50" r="1.2"/><circle cx="165" cy="50" r="1.2"/><circle cx="200" cy="50" r="1.2"/>
    <circle cx="25" cy="80" r="1.2"/><circle cx="60" cy="80" r="1.2"/><circle cx="95" cy="80" r="1.2"/><circle cx="130" cy="80" r="1.2"/><circle cx="165" cy="80" r="1.2"/><circle cx="200" cy="80" r="1.2"/>
    <circle cx="25" cy="110" r="1.2"/><circle cx="60" cy="110" r="1.2"/><circle cx="95" cy="110" r="1.2"/><circle cx="130" cy="110" r="1.2"/><circle cx="165" cy="110" r="1.2"/><circle cx="200" cy="110" r="1.2"/>
    <circle cx="25" cy="140" r="1.2"/><circle cx="60" cy="140" r="1.2"/><circle cx="95" cy="140" r="1.2"/><circle cx="130" cy="140" r="1.2"/><circle cx="165" cy="140" r="1.2"/><circle cx="200" cy="140" r="1.2"/>
    <circle cx="25" cy="170" r="1.2"/><circle cx="60" cy="170" r="1.2"/><circle cx="95" cy="170" r="1.2"/><circle cx="130" cy="170" r="1.2"/><circle cx="165" cy="170" r="1.2"/><circle cx="200" cy="170" r="1.2"/>
    <circle cx="490" cy="35" r="1.2"/><circle cx="525" cy="35" r="1.2"/><circle cx="560" cy="35" r="1.2"/>
    <circle cx="490" cy="65" r="1.2"/><circle cx="525" cy="65" r="1.2"/><circle cx="560" cy="65" r="1.2"/>
  </g>
  <g transform="translate(100,140)" filter="url(#fi-glow)">
    <line x1="0" y1="0" x2="140" y2="0" stroke="#38BDF8" stroke-width="1" opacity="0.3"/>
    <line x1="0" y1="0" x2="0" y2="-100" stroke="#38BDF8" stroke-width="1" opacity="0.3"/>
    <polyline points="10,-20 30,-45 55,-35 75,-70 95,-55 115,-85 135,-75" fill="none" stroke="#38BDF8" stroke-width="2" opacity="0.7" stroke-linecap="round" stroke-linejoin="round" class="fi-trend"/>
    <circle cx="10" cy="-20" r="3" fill="#38BDF8" opacity="0.8" class="fi-dot"/>
    <circle cx="30" cy="-45" r="3" fill="#38BDF8" opacity="0.8" class="fi-dot" style="animation-delay:0.3s"/>
    <circle cx="55" cy="-35" r="3" fill="#38BDF8" opacity="0.8" class="fi-dot" style="animation-delay:0.6s"/>
    <circle cx="75" cy="-70" r="3" fill="#38BDF8" opacity="0.8" class="fi-dot" style="animation-delay:0.9s"/>
    <circle cx="95" cy="-55" r="3" fill="#38BDF8" opacity="0.8" class="fi-dot" style="animation-delay:1.2s"/>
    <circle cx="115" cy="-85" r="3" fill="#38BDF8" opacity="0.8" class="fi-dot" style="animation-delay:1.5s"/>
    <circle cx="135" cy="-75" r="3" fill="#38BDF8" opacity="0.8" class="fi-dot" style="animation-delay:1.8s"/>
  </g>
  <circle cx="170" cy="90" r="10" fill="none" stroke="#38BDF8" stroke-width="0.8" opacity="0.3" class="fi-ring"/>
  <circle cx="600" cy="55" r="30" fill="#38BDF8" opacity="0.04"/>
  <circle cx="700" cy="125" r="45" fill="#38BDF8" opacity="0.03"/>
  <circle cx="770" cy="55" r="22" fill="#38BDF8" opacity="0.05"/>
</svg>
```

---

## SVG 12: UX/UI Design & Product Management
**Sector:** Custom
**Palette:** Custom (#1A0A2E / #4C1D95 / #C084FC)
**Pattern:** Hexagonal Grid
**Icon:** Layout/Grid
**Animation:** Breathe Nodes + Pulse Rings
**Prefix:** ux

```html
<svg viewBox="0 0 820 180" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="xMidYMid slice">
  <defs>
    <linearGradient id="ux-bg" x1="0" y1="0" x2="1" y2="1">
      <stop offset="0%" stop-color="#1A0A2E"/>
      <stop offset="100%" stop-color="#4C1D95"/>
    </linearGradient>
    <filter id="ux-glow">
      <feGaussianBlur stdDeviation="4" result="blur"/>
      <feMerge><feMergeNode in="blur"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
    <style>
      @keyframes ux-breathe { 0%,100% { opacity: 0.5; } 50% { opacity: 0.9; } }
      @keyframes ux-pulse { 0% { r: 12; opacity: 0.5; } 100% { r: 38; opacity: 0; } }
      @keyframes ux-morph { 0%,100% { rx: 3; } 50% { rx: 8; } }
      .ux-panel { animation: ux-breathe 2.5s ease-in-out infinite; }
      .ux-ring { animation: ux-pulse 2.8s ease-out infinite; }
      .ux-shape { animation: ux-morph 3s ease-in-out infinite; }
    </style>
  </defs>
  <rect width="820" height="180" fill="url(#ux-bg)"/>
  <g opacity="0.07" stroke="#C084FC" stroke-width="0.6" fill="none">
    <path d="M15,30 L40,15 L65,30 L65,55 L40,70 L15,55 Z"/>
    <path d="M65,30 L90,15 L115,30 L115,55 L90,70 L65,55 Z"/>
    <path d="M115,30 L140,15 L165,30 L165,55 L140,70 L115,55 Z"/>
    <path d="M40,70 L65,55 L90,70 L90,95 L65,110 L40,95 Z"/>
    <path d="M90,70 L115,55 L140,70 L140,95 L115,110 L90,95 Z"/>
    <path d="M65,110 L90,95 L115,110 L115,135 L90,150 L65,135 Z"/>
    <path d="M360,5 L385,-10 L410,5 L410,30 L385,45 L360,30 Z"/>
    <path d="M510,95 L535,80 L560,95 L560,120 L535,135 L510,120 Z"/>
    <path d="M560,95 L585,80 L610,95 L610,120 L585,135 L560,120 Z"/>
  </g>
  <g transform="translate(125,55)" filter="url(#ux-glow)">
    <rect x="0" y="0" width="80" height="70" rx="5" fill="none" stroke="#C084FC" stroke-width="1.5" opacity="0.6"/>
    <line x1="0" y1="18" x2="80" y2="18" stroke="#C084FC" stroke-width="0.8" opacity="0.3"/>
    <rect x="6" y="24" width="45" height="38" rx="3" fill="#C084FC" opacity="0.15" class="ux-panel"/>
    <rect x="56" y="24" width="18" height="16" rx="2" fill="#C084FC" opacity="0.2" class="ux-panel" style="animation-delay:0.5s"/>
    <rect x="56" y="46" width="18" height="16" rx="2" fill="#C084FC" opacity="0.2" class="ux-shape" style="animation-delay:1s"/>
    <circle cx="10" cy="9" r="2.5" fill="#C084FC" opacity="0.4"/>
    <circle cx="18" cy="9" r="2.5" fill="#C084FC" opacity="0.3"/>
    <circle cx="26" cy="9" r="2.5" fill="#C084FC" opacity="0.2"/>
    <rect x="12" y="32" width="30" height="3" rx="1" fill="#C084FC" opacity="0.25"/>
    <rect x="12" y="40" width="22" height="3" rx="1" fill="#C084FC" opacity="0.2"/>
    <rect x="12" y="48" width="26" height="3" rx="1" fill="#C084FC" opacity="0.2"/>
  </g>
  <circle cx="165" cy="90" r="12" fill="none" stroke="#C084FC" stroke-width="0.8" opacity="0.3" class="ux-ring"/>
  <circle cx="590" cy="45" r="32" fill="#C084FC" opacity="0.04"/>
  <circle cx="700" cy="130" r="48" fill="#C084FC" opacity="0.03"/>
  <circle cx="770" cy="50" r="20" fill="#C084FC" opacity="0.05"/>
</svg>
```
