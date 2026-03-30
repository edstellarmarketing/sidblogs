# SKILL CARD SVGs: Skills in Demand in India
**Date:** 2026-03-26
**Country:** India
**Skills:** 13
**SVG Viewport:** 820 x 180px

---

## SVG 1: Artificial Intelligence & Machine Learning
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
    <filter id="ai-glow-soft">
      <feGaussianBlur stdDeviation="8" result="blur"/>
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
  <!-- Circuit pattern -->
  <g opacity="0.1" stroke="#60A5FA" stroke-width="0.8" fill="none">
    <path d="M0,45 H80 V25 H160 V45 H240"/>
    <path d="M0,90 H120 V70 H200 V90 H300"/>
    <path d="M0,135 H60 V115 H180 V135 H260"/>
    <path d="M400,30 H500 V50 H580"/>
    <path d="M420,130 H520 V150 H620"/>
    <circle cx="80" cy="45" r="2.5" fill="#60A5FA" stroke="none"/>
    <circle cx="160" cy="25" r="2.5" fill="#60A5FA" stroke="none"/>
    <circle cx="200" cy="70" r="2.5" fill="#60A5FA" stroke="none"/>
    <circle cx="500" cy="50" r="2.5" fill="#60A5FA" stroke="none"/>
  </g>
  <!-- Neural network -->
  <g transform="translate(150,90)">
    <!-- Layer 1 (input) -->
    <circle cx="-60" cy="-40" r="5" fill="#60A5FA" opacity="0.9" class="ai-node"/>
    <circle cx="-60" cy="0" r="5" fill="#60A5FA" opacity="0.9" class="ai-node" style="animation-delay:0.3s"/>
    <circle cx="-60" cy="40" r="5" fill="#60A5FA" opacity="0.9" class="ai-node" style="animation-delay:0.6s"/>
    <!-- Layer 2 (hidden) -->
    <circle cx="0" cy="-50" r="5" fill="#60A5FA" opacity="0.8" class="ai-node" style="animation-delay:0.2s"/>
    <circle cx="0" cy="-15" r="5" fill="#60A5FA" opacity="0.8" class="ai-node" style="animation-delay:0.5s"/>
    <circle cx="0" cy="15" r="5" fill="#60A5FA" opacity="0.8" class="ai-node" style="animation-delay:0.8s"/>
    <circle cx="0" cy="50" r="5" fill="#60A5FA" opacity="0.8" class="ai-node" style="animation-delay:0.4s"/>
    <!-- Layer 3 (output) -->
    <circle cx="60" cy="-25" r="5" fill="#60A5FA" opacity="0.9" class="ai-node" style="animation-delay:0.7s"/>
    <circle cx="60" cy="25" r="5" fill="#60A5FA" opacity="0.9" class="ai-node" style="animation-delay:1s"/>
    <!-- Connections L1->L2 -->
    <line x1="-55" y1="-40" x2="-5" y2="-50" stroke="#60A5FA" stroke-width="0.8" opacity="0.3" class="ai-flow"/>
    <line x1="-55" y1="-40" x2="-5" y2="-15" stroke="#60A5FA" stroke-width="0.8" opacity="0.3" class="ai-flow"/>
    <line x1="-55" y1="0" x2="-5" y2="-15" stroke="#60A5FA" stroke-width="0.8" opacity="0.3" class="ai-flow"/>
    <line x1="-55" y1="0" x2="-5" y2="15" stroke="#60A5FA" stroke-width="0.8" opacity="0.3" class="ai-flow"/>
    <line x1="-55" y1="40" x2="-5" y2="15" stroke="#60A5FA" stroke-width="0.8" opacity="0.3" class="ai-flow"/>
    <line x1="-55" y1="40" x2="-5" y2="50" stroke="#60A5FA" stroke-width="0.8" opacity="0.3" class="ai-flow"/>
    <!-- Connections L2->L3 -->
    <line x1="5" y1="-50" x2="55" y2="-25" stroke="#60A5FA" stroke-width="0.8" opacity="0.3" class="ai-flow"/>
    <line x1="5" y1="-15" x2="55" y2="-25" stroke="#60A5FA" stroke-width="0.8" opacity="0.3" class="ai-flow"/>
    <line x1="5" y1="15" x2="55" y2="25" stroke="#60A5FA" stroke-width="0.8" opacity="0.3" class="ai-flow"/>
    <line x1="5" y1="50" x2="55" y2="25" stroke="#60A5FA" stroke-width="0.8" opacity="0.3" class="ai-flow"/>
  </g>
  <!-- Pulse ring at center -->
  <circle cx="150" cy="90" r="12" fill="none" stroke="#60A5FA" stroke-width="1" opacity="0.4" class="ai-ring"/>
  <circle cx="150" cy="90" r="12" fill="none" stroke="#60A5FA" stroke-width="1" opacity="0.4" class="ai-ring" style="animation-delay:0.8s"/>
  <!-- Decorative orbs (right side) -->
  <circle cx="650" cy="90" r="60" fill="#1E3A8A" opacity="0.2"/>
  <circle cx="650" cy="90" r="38" fill="#1E3A8A" opacity="0.15"/>
  <circle cx="650" cy="90" r="20" fill="#60A5FA" opacity="0.2"/>
  <circle cx="650" cy="90" r="8" fill="#60A5FA" opacity="0.5" filter="url(#ai-glow)"/>
  <circle cx="740" cy="50" r="25" fill="#1E3A8A" opacity="0.15"/>
  <circle cx="740" cy="50" r="10" fill="#60A5FA" opacity="0.2"/>
  <circle cx="740" cy="50" r="4" fill="#60A5FA" opacity="0.4" filter="url(#ai-glow-soft)"/>
  <line x1="650" y1="90" x2="740" y2="50" stroke="#60A5FA" stroke-width="0.5" opacity="0.2"/>
  <circle cx="720" cy="140" r="18" fill="#1E3A8A" opacity="0.12"/>
  <circle cx="720" cy="140" r="6" fill="#60A5FA" opacity="0.3"/>
  <line x1="650" y1="90" x2="720" y2="140" stroke="#60A5FA" stroke-width="0.5" opacity="0.15"/>
</svg>
```

---

## SVG 2: Data Science & Analytics
**Sector:** Analytics
**Palette:** Analytics (#0F1629 / #1E2D6B / #818CF8)
**Pattern:** Dot Grid
**Icon:** Chart
**Animation:** Breathe Nodes
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
      @keyframes ds-breathe { 0%,100% { r: 5; opacity: 1; } 50% { r: 7; opacity: 0.5; } }
      @keyframes ds-rise { 0% { transform: scaleY(0); } 100% { transform: scaleY(1); } }
      .ds-node { animation: ds-breathe 2.2s ease-in-out infinite; }
    </style>
  </defs>
  <rect width="820" height="180" fill="url(#ds-bg)"/>
  <!-- Dot grid pattern -->
  <g opacity="0.07" fill="#818CF8">
    <circle cx="30" cy="30" r="1.5"/><circle cx="90" cy="30" r="1.5"/><circle cx="150" cy="30" r="1.5"/><circle cx="210" cy="30" r="1.5"/><circle cx="270" cy="30" r="1.5"/><circle cx="330" cy="30" r="1.5"/><circle cx="390" cy="30" r="1.5"/><circle cx="450" cy="30" r="1.5"/><circle cx="510" cy="30" r="1.5"/><circle cx="570" cy="30" r="1.5"/><circle cx="630" cy="30" r="1.5"/><circle cx="690" cy="30" r="1.5"/><circle cx="750" cy="30" r="1.5"/>
    <circle cx="30" cy="90" r="1.5"/><circle cx="90" cy="90" r="1.5"/><circle cx="150" cy="90" r="1.5"/><circle cx="210" cy="90" r="1.5"/><circle cx="270" cy="90" r="1.5"/><circle cx="330" cy="90" r="1.5"/><circle cx="390" cy="90" r="1.5"/><circle cx="450" cy="90" r="1.5"/><circle cx="510" cy="90" r="1.5"/><circle cx="570" cy="90" r="1.5"/><circle cx="630" cy="90" r="1.5"/><circle cx="690" cy="90" r="1.5"/><circle cx="750" cy="90" r="1.5"/>
    <circle cx="30" cy="150" r="1.5"/><circle cx="90" cy="150" r="1.5"/><circle cx="150" cy="150" r="1.5"/><circle cx="210" cy="150" r="1.5"/><circle cx="270" cy="150" r="1.5"/><circle cx="330" cy="150" r="1.5"/><circle cx="390" cy="150" r="1.5"/><circle cx="450" cy="150" r="1.5"/><circle cx="510" cy="150" r="1.5"/><circle cx="570" cy="150" r="1.5"/><circle cx="630" cy="150" r="1.5"/><circle cx="690" cy="150" r="1.5"/><circle cx="750" cy="150" r="1.5"/>
  </g>
  <!-- Bar chart icon -->
  <g transform="translate(120,140)">
    <rect x="0" y="-80" width="14" height="80" fill="#818CF8" opacity="0.5" rx="2"/>
    <rect x="22" y="-55" width="14" height="55" fill="#818CF8" opacity="0.4" rx="2"/>
    <rect x="44" y="-95" width="14" height="95" fill="#818CF8" opacity="0.6" rx="2"/>
    <rect x="66" y="-40" width="14" height="40" fill="#818CF8" opacity="0.35" rx="2"/>
    <rect x="88" y="-70" width="14" height="70" fill="#818CF8" opacity="0.5" rx="2"/>
    <!-- Data points on top of bars -->
    <circle cx="7" cy="-85" r="4" fill="#818CF8" opacity="0.9" class="ds-node"/>
    <circle cx="29" cy="-60" r="4" fill="#818CF8" opacity="0.9" class="ds-node" style="animation-delay:0.3s"/>
    <circle cx="51" cy="-100" r="4" fill="#818CF8" opacity="0.9" class="ds-node" style="animation-delay:0.6s"/>
    <circle cx="73" cy="-45" r="4" fill="#818CF8" opacity="0.9" class="ds-node" style="animation-delay:0.9s"/>
    <circle cx="95" cy="-75" r="4" fill="#818CF8" opacity="0.9" class="ds-node" style="animation-delay:1.2s"/>
    <!-- Trend line connecting data points -->
    <polyline points="7,-85 29,-60 51,-100 73,-45 95,-75" fill="none" stroke="#818CF8" stroke-width="1.5" opacity="0.6"/>
  </g>
  <!-- Decorative orbs -->
  <circle cx="680" cy="85" r="55" fill="#1E2D6B" opacity="0.25"/>
  <circle cx="680" cy="85" r="35" fill="#1E2D6B" opacity="0.18"/>
  <circle cx="680" cy="85" r="18" fill="#818CF8" opacity="0.25"/>
  <circle cx="680" cy="85" r="7" fill="#818CF8" opacity="0.5" filter="url(#ds-glow)"/>
  <circle cx="760" cy="45" r="20" fill="#1E2D6B" opacity="0.15"/>
  <circle cx="760" cy="45" r="8" fill="#818CF8" opacity="0.25"/>
  <line x1="680" y1="85" x2="760" y2="45" stroke="#818CF8" stroke-width="0.5" opacity="0.2"/>
  <circle cx="750" cy="140" r="15" fill="#1E2D6B" opacity="0.12"/>
  <circle cx="750" cy="140" r="5" fill="#818CF8" opacity="0.2"/>
  <line x1="680" y1="85" x2="750" y2="140" stroke="#818CF8" stroke-width="0.5" opacity="0.15"/>
</svg>
```

---

## SVG 3: Cybersecurity
**Sector:** Security
**Palette:** Security (#05050F / #1E1B4B / #818CF8)
**Pattern:** Hexagonal Grid
**Icon:** Shield
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
      <feGaussianBlur stdDeviation="5" result="blur"/>
      <feMerge><feMergeNode in="blur"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
    <style>
      @keyframes cs-pulse { 0% { r: 15; opacity: 0.5; } 100% { r: 50; opacity: 0; } }
      @keyframes cs-scan { 0% { transform: translateX(-60px); opacity: 0; } 10% { opacity: 0.6; } 90% { opacity: 0.6; } 100% { transform: translateX(820px); opacity: 0; } }
      .cs-ring { animation: cs-pulse 2.8s ease-out infinite; }
      .cs-scan { animation: cs-scan 4s linear infinite; }
    </style>
  </defs>
  <rect width="820" height="180" fill="url(#cs-bg)"/>
  <!-- Hex grid pattern -->
  <g opacity="0.06" stroke="#818CF8" stroke-width="0.5" fill="none">
    <polygon points="50,20 70,10 90,20 90,40 70,50 50,40"/>
    <polygon points="90,20 110,10 130,20 130,40 110,50 90,40"/>
    <polygon points="70,50 90,40 110,50 110,70 90,80 70,70"/>
    <polygon points="350,80 370,70 390,80 390,100 370,110 350,100"/>
    <polygon points="390,80 410,70 430,80 430,100 410,110 390,100"/>
    <polygon points="450,20 470,10 490,20 490,40 470,50 450,40"/>
    <polygon points="250,120 270,110 290,120 290,140 270,150 250,140"/>
    <polygon points="550,110 570,100 590,110 590,130 570,140 550,130"/>
  </g>
  <!-- Shield icon -->
  <g transform="translate(160,90)">
    <path d="M0,-55 L40,-38 L40,10 C40,35 20,50 0,60 C-20,50 -40,35 -40,10 L-40,-38 Z" fill="none" stroke="#818CF8" stroke-width="2" opacity="0.7"/>
    <path d="M0,-40 L28,-28 L28,5 C28,22 14,34 0,42 C-14,34 -28,22 -28,5 L-28,-28 Z" fill="#818CF8" opacity="0.1"/>
    <!-- Lock element -->
    <rect x="-8" y="-8" width="16" height="14" rx="2" fill="none" stroke="#818CF8" stroke-width="1.5" opacity="0.8"/>
    <path d="M-5,-8 V-15 C-5,-22 5,-22 5,-15 V-8" fill="none" stroke="#818CF8" stroke-width="1.5" opacity="0.8"/>
    <circle cx="0" cy="0" r="2" fill="#818CF8" opacity="0.9" filter="url(#cs-glow)"/>
  </g>
  <!-- Pulse rings from shield center -->
  <circle cx="160" cy="90" r="15" fill="none" stroke="#818CF8" stroke-width="0.8" class="cs-ring"/>
  <circle cx="160" cy="90" r="15" fill="none" stroke="#818CF8" stroke-width="0.8" class="cs-ring" style="animation-delay:0.9s"/>
  <circle cx="160" cy="90" r="15" fill="none" stroke="#818CF8" stroke-width="0.8" class="cs-ring" style="animation-delay:1.8s"/>
  <!-- Scan line -->
  <rect x="0" y="0" width="3" height="180" fill="#818CF8" opacity="0" class="cs-scan"/>
  <!-- Decorative orbs -->
  <circle cx="660" cy="90" r="55" fill="#1E1B4B" opacity="0.25"/>
  <circle cx="660" cy="90" r="32" fill="#1E1B4B" opacity="0.18"/>
  <circle cx="660" cy="90" r="15" fill="#818CF8" opacity="0.2"/>
  <circle cx="660" cy="90" r="6" fill="#818CF8" opacity="0.5" filter="url(#cs-glow)"/>
  <circle cx="750" cy="55" r="22" fill="#1E1B4B" opacity="0.15"/>
  <circle cx="750" cy="55" r="8" fill="#818CF8" opacity="0.2"/>
  <line x1="660" y1="90" x2="750" y2="55" stroke="#818CF8" stroke-width="0.5" opacity="0.2"/>
  <circle cx="740" cy="145" r="16" fill="#1E1B4B" opacity="0.12"/>
  <circle cx="740" cy="145" r="5" fill="#818CF8" opacity="0.2"/>
  <line x1="660" y1="90" x2="740" y2="145" stroke="#818CF8" stroke-width="0.5" opacity="0.15"/>
</svg>
```

---

## SVG 4: Cloud Computing & DevOps
**Sector:** Technology
**Palette:** Technology (#0F172A / #1E3A8A / #60A5FA)
**Pattern:** Horizontal Lines
**Icon:** Cloud
**Animation:** Flow Lines
**Prefix:** cc

```html
<svg viewBox="0 0 820 180" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="xMidYMid slice">
  <defs>
    <linearGradient id="cc-bg" x1="0" y1="0" x2="1" y2="1">
      <stop offset="0%" stop-color="#0F172A"/>
      <stop offset="100%" stop-color="#1E3A8A"/>
    </linearGradient>
    <filter id="cc-glow">
      <feGaussianBlur stdDeviation="4" result="blur"/>
      <feMerge><feMergeNode in="blur"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
    <style>
      @keyframes cc-flow { 0% { stroke-dashoffset: 200; } 100% { stroke-dashoffset: 0; } }
      @keyframes cc-float { 0%,100% { transform: translateY(0); } 50% { transform: translateY(-6px); } }
      .cc-flow { stroke-dasharray: 200; animation: cc-flow 2.5s linear infinite; }
      .cc-cloud { animation: cc-float 3s ease-in-out infinite; }
    </style>
  </defs>
  <rect width="820" height="180" fill="url(#cc-bg)"/>
  <!-- Horizontal lines -->
  <g opacity="0.07" stroke="#60A5FA" stroke-width="0.5">
    <line x1="0" y1="45" x2="820" y2="45"/>
    <line x1="0" y1="90" x2="820" y2="90"/>
    <line x1="0" y1="135" x2="820" y2="135"/>
  </g>
  <!-- Cloud icon -->
  <g transform="translate(160,85)" class="cc-cloud">
    <path d="M-45,15 C-55,15 -60,5 -55,-5 C-55,-20 -40,-30 -25,-28 C-20,-42 -5,-48 10,-42 C25,-48 40,-38 42,-25 C55,-22 60,-10 55,2 C58,15 48,22 35,18 L-45,18 Z" fill="none" stroke="#60A5FA" stroke-width="1.8" opacity="0.7"/>
    <!-- Connection nodes below cloud -->
    <circle cx="-20" cy="25" r="4" fill="#60A5FA" opacity="0.7"/>
    <circle cx="5" cy="25" r="4" fill="#60A5FA" opacity="0.7"/>
    <circle cx="30" cy="25" r="4" fill="#60A5FA" opacity="0.7"/>
    <line x1="-20" y1="18" x2="-20" y2="25" stroke="#60A5FA" stroke-width="1" opacity="0.5"/>
    <line x1="5" y1="18" x2="5" y2="25" stroke="#60A5FA" stroke-width="1" opacity="0.5"/>
    <line x1="30" y1="18" x2="30" y2="25" stroke="#60A5FA" stroke-width="1" opacity="0.5"/>
    <!-- Flow lines from nodes downward -->
    <line x1="-20" y1="29" x2="-20" y2="55" stroke="#60A5FA" stroke-width="0.8" opacity="0.3" class="cc-flow"/>
    <line x1="5" y1="29" x2="5" y2="55" stroke="#60A5FA" stroke-width="0.8" opacity="0.3" class="cc-flow" style="animation-delay:0.4s"/>
    <line x1="30" y1="29" x2="30" y2="55" stroke="#60A5FA" stroke-width="0.8" opacity="0.3" class="cc-flow" style="animation-delay:0.8s"/>
  </g>
  <!-- Decorative orbs -->
  <circle cx="670" cy="90" r="55" fill="#1E3A8A" opacity="0.22"/>
  <circle cx="670" cy="90" r="34" fill="#1E3A8A" opacity="0.15"/>
  <circle cx="670" cy="90" r="16" fill="#60A5FA" opacity="0.2"/>
  <circle cx="670" cy="90" r="6" fill="#60A5FA" opacity="0.5" filter="url(#cc-glow)"/>
  <circle cx="755" cy="50" r="20" fill="#1E3A8A" opacity="0.15"/>
  <circle cx="755" cy="50" r="7" fill="#60A5FA" opacity="0.2"/>
  <line x1="670" y1="90" x2="755" y2="50" stroke="#60A5FA" stroke-width="0.5" opacity="0.2"/>
  <circle cx="745" cy="140" r="18" fill="#1E3A8A" opacity="0.12"/>
  <circle cx="745" cy="140" r="6" fill="#60A5FA" opacity="0.2"/>
  <line x1="670" y1="90" x2="745" y2="140" stroke="#60A5FA" stroke-width="0.5" opacity="0.15"/>
</svg>
```

---

## SVG 5: Full-Stack Development
**Sector:** Technology
**Palette:** Technology (#0F172A / #1E3A8A / #60A5FA)
**Pattern:** Diagonal Lines
**Icon:** Chip (code brackets)
**Animation:** Flow Lines
**Prefix:** fs

```html
<svg viewBox="0 0 820 180" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="xMidYMid slice">
  <defs>
    <linearGradient id="fs-bg" x1="0" y1="0" x2="1" y2="1">
      <stop offset="0%" stop-color="#0F172A"/>
      <stop offset="100%" stop-color="#1E3A8A"/>
    </linearGradient>
    <filter id="fs-glow">
      <feGaussianBlur stdDeviation="4" result="blur"/>
      <feMerge><feMergeNode in="blur"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
    <style>
      @keyframes fs-flow { 0% { stroke-dashoffset: 180; } 100% { stroke-dashoffset: 0; } }
      @keyframes fs-blink { 0%,49% { opacity: 1; } 50%,100% { opacity: 0.3; } }
      .fs-flow { stroke-dasharray: 180; animation: fs-flow 2s linear infinite; }
      .fs-cursor { animation: fs-blink 1.2s step-end infinite; }
    </style>
  </defs>
  <rect width="820" height="180" fill="url(#fs-bg)"/>
  <!-- Diagonal lines -->
  <g opacity="0.05" stroke="#60A5FA" stroke-width="0.5">
    <line x1="0" y1="0" x2="180" y2="180"/><line x1="100" y1="0" x2="280" y2="180"/>
    <line x1="200" y1="0" x2="380" y2="180"/><line x1="300" y1="0" x2="480" y2="180"/>
    <line x1="400" y1="0" x2="580" y2="180"/><line x1="500" y1="0" x2="680" y2="180"/>
    <line x1="600" y1="0" x2="780" y2="180"/><line x1="700" y1="0" x2="820" y2="120"/>
  </g>
  <!-- Code brackets icon -->
  <g transform="translate(155,90)">
    <!-- Left bracket < -->
    <path d="M-30,-35 L-55,0 L-30,35" fill="none" stroke="#60A5FA" stroke-width="2.5" stroke-linecap="round" opacity="0.8"/>
    <!-- Right bracket > -->
    <path d="M30,-35 L55,0 L30,35" fill="none" stroke="#60A5FA" stroke-width="2.5" stroke-linecap="round" opacity="0.8"/>
    <!-- Slash / -->
    <line x1="10" y1="-30" x2="-10" y2="30" stroke="#60A5FA" stroke-width="2" stroke-linecap="round" opacity="0.6"/>
    <!-- Cursor -->
    <rect x="15" y="28" width="2" height="12" fill="#60A5FA" opacity="0.8" class="fs-cursor"/>
    <!-- Connection lines to stack layers -->
    <line x1="-55" y1="0" x2="-80" y2="-20" stroke="#60A5FA" stroke-width="0.8" opacity="0.3" class="fs-flow"/>
    <line x1="-55" y1="0" x2="-80" y2="20" stroke="#60A5FA" stroke-width="0.8" opacity="0.3" class="fs-flow"/>
    <line x1="55" y1="0" x2="80" y2="-20" stroke="#60A5FA" stroke-width="0.8" opacity="0.3" class="fs-flow"/>
    <line x1="55" y1="0" x2="80" y2="20" stroke="#60A5FA" stroke-width="0.8" opacity="0.3" class="fs-flow"/>
    <!-- Stack layer dots -->
    <circle cx="-80" cy="-20" r="3" fill="#60A5FA" opacity="0.6"/>
    <circle cx="-80" cy="20" r="3" fill="#60A5FA" opacity="0.6"/>
    <circle cx="80" cy="-20" r="3" fill="#60A5FA" opacity="0.6"/>
    <circle cx="80" cy="20" r="3" fill="#60A5FA" opacity="0.6"/>
  </g>
  <!-- Decorative orbs -->
  <circle cx="660" cy="85" r="50" fill="#1E3A8A" opacity="0.2"/>
  <circle cx="660" cy="85" r="30" fill="#1E3A8A" opacity="0.15"/>
  <circle cx="660" cy="85" r="14" fill="#60A5FA" opacity="0.2"/>
  <circle cx="660" cy="85" r="5" fill="#60A5FA" opacity="0.5" filter="url(#fs-glow)"/>
  <circle cx="750" cy="55" r="18" fill="#1E3A8A" opacity="0.12"/>
  <circle cx="750" cy="55" r="6" fill="#60A5FA" opacity="0.2"/>
  <line x1="660" y1="85" x2="750" y2="55" stroke="#60A5FA" stroke-width="0.5" opacity="0.18"/>
  <circle cx="740" cy="140" r="15" fill="#1E3A8A" opacity="0.1"/>
  <circle cx="740" cy="140" r="5" fill="#60A5FA" opacity="0.18"/>
  <line x1="660" y1="85" x2="740" y2="140" stroke="#60A5FA" stroke-width="0.5" opacity="0.12"/>
</svg>
```

---

## SVG 6: Generative AI & Prompt Engineering
**Sector:** Technology
**Palette:** Technology (#0F172A / #1E3A8A / #60A5FA)
**Pattern:** Circuit Traces
**Icon:** Chip (processor with radiating traces)
**Animation:** Pulse Rings + Breathe
**Prefix:** ga

```html
<svg viewBox="0 0 820 180" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="xMidYMid slice">
  <defs>
    <linearGradient id="ga-bg" x1="0" y1="0" x2="1" y2="1">
      <stop offset="0%" stop-color="#0F172A"/>
      <stop offset="100%" stop-color="#1E3A8A"/>
    </linearGradient>
    <filter id="ga-glow">
      <feGaussianBlur stdDeviation="6" result="blur"/>
      <feMerge><feMergeNode in="blur"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
    <style>
      @keyframes ga-pulse { 0% { r: 20; opacity: 0.5; } 100% { r: 55; opacity: 0; } }
      @keyframes ga-breathe { 0%,100% { opacity: 0.8; } 50% { opacity: 0.3; } }
      @keyframes ga-spin { 0% { transform: rotate(0deg); } 100% { transform: rotate(360deg); } }
      .ga-ring { animation: ga-pulse 3s ease-out infinite; }
      .ga-trace { animation: ga-breathe 2s ease-in-out infinite; }
    </style>
  </defs>
  <rect width="820" height="180" fill="url(#ga-bg)"/>
  <!-- Circuit pattern -->
  <g opacity="0.08" stroke="#60A5FA" stroke-width="0.7" fill="none">
    <path d="M0,50 H70 V30 H140"/>
    <path d="M0,130 H90 V110 H170"/>
    <path d="M420,40 H520 V60 H600"/>
    <path d="M380,140 H480 V120 H560"/>
    <circle cx="70" cy="50" r="2" fill="#60A5FA" stroke="none"/>
    <circle cx="170" cy="110" r="2" fill="#60A5FA" stroke="none"/>
  </g>
  <!-- Processor chip icon -->
  <g transform="translate(160,90)">
    <!-- Chip body -->
    <rect x="-28" y="-28" width="56" height="56" rx="6" fill="#1E3A8A" opacity="0.4" stroke="#60A5FA" stroke-width="1.5"/>
    <!-- Inner core -->
    <rect x="-15" y="-15" width="30" height="30" rx="3" fill="#60A5FA" opacity="0.15" stroke="#60A5FA" stroke-width="0.8"/>
    <!-- Core glow -->
    <circle cx="0" cy="0" r="8" fill="#60A5FA" opacity="0.4" filter="url(#ga-glow)"/>
    <circle cx="0" cy="0" r="3" fill="#60A5FA" opacity="0.8"/>
    <!-- Radiating traces (pins) -->
    <line x1="-28" y1="-15" x2="-45" y2="-15" stroke="#60A5FA" stroke-width="1" opacity="0.5" class="ga-trace"/>
    <line x1="-28" y1="0" x2="-50" y2="0" stroke="#60A5FA" stroke-width="1" opacity="0.5" class="ga-trace" style="animation-delay:0.2s"/>
    <line x1="-28" y1="15" x2="-45" y2="15" stroke="#60A5FA" stroke-width="1" opacity="0.5" class="ga-trace" style="animation-delay:0.4s"/>
    <line x1="28" y1="-15" x2="45" y2="-15" stroke="#60A5FA" stroke-width="1" opacity="0.5" class="ga-trace" style="animation-delay:0.6s"/>
    <line x1="28" y1="0" x2="50" y2="0" stroke="#60A5FA" stroke-width="1" opacity="0.5" class="ga-trace" style="animation-delay:0.8s"/>
    <line x1="28" y1="15" x2="45" y2="15" stroke="#60A5FA" stroke-width="1" opacity="0.5" class="ga-trace" style="animation-delay:1s"/>
    <line x1="-15" y1="-28" x2="-15" y2="-45" stroke="#60A5FA" stroke-width="1" opacity="0.5" class="ga-trace" style="animation-delay:0.3s"/>
    <line x1="0" y1="-28" x2="0" y2="-48" stroke="#60A5FA" stroke-width="1" opacity="0.5" class="ga-trace" style="animation-delay:0.5s"/>
    <line x1="15" y1="-28" x2="15" y2="-45" stroke="#60A5FA" stroke-width="1" opacity="0.5" class="ga-trace" style="animation-delay:0.7s"/>
    <line x1="-15" y1="28" x2="-15" y2="45" stroke="#60A5FA" stroke-width="1" opacity="0.5" class="ga-trace" style="animation-delay:0.9s"/>
    <line x1="0" y1="28" x2="0" y2="48" stroke="#60A5FA" stroke-width="1" opacity="0.5" class="ga-trace" style="animation-delay:1.1s"/>
    <line x1="15" y1="28" x2="15" y2="45" stroke="#60A5FA" stroke-width="1" opacity="0.5" class="ga-trace" style="animation-delay:1.3s"/>
  </g>
  <!-- Pulse rings -->
  <circle cx="160" cy="90" r="20" fill="none" stroke="#60A5FA" stroke-width="0.8" class="ga-ring"/>
  <circle cx="160" cy="90" r="20" fill="none" stroke="#60A5FA" stroke-width="0.8" class="ga-ring" style="animation-delay:1s"/>
  <circle cx="160" cy="90" r="20" fill="none" stroke="#60A5FA" stroke-width="0.8" class="ga-ring" style="animation-delay:2s"/>
  <!-- Decorative orbs -->
  <circle cx="670" cy="90" r="55" fill="#1E3A8A" opacity="0.22"/>
  <circle cx="670" cy="90" r="35" fill="#1E3A8A" opacity="0.16"/>
  <circle cx="670" cy="90" r="18" fill="#60A5FA" opacity="0.22"/>
  <circle cx="670" cy="90" r="7" fill="#60A5FA" opacity="0.5" filter="url(#ga-glow)"/>
  <circle cx="755" cy="48" r="22" fill="#1E3A8A" opacity="0.14"/>
  <circle cx="755" cy="48" r="8" fill="#60A5FA" opacity="0.2"/>
  <line x1="670" y1="90" x2="755" y2="48" stroke="#60A5FA" stroke-width="0.5" opacity="0.18"/>
  <circle cx="748" cy="142" r="17" fill="#1E3A8A" opacity="0.12"/>
  <circle cx="748" cy="142" r="6" fill="#60A5FA" opacity="0.2"/>
  <line x1="670" y1="90" x2="748" y2="142" stroke="#60A5FA" stroke-width="0.5" opacity="0.14"/>
</svg>
```

---

## SVG 7: Blockchain & Web3
**Sector:** Finance
**Palette:** Finance (#0A0F1E / #1E3A5F / #38BDF8)
**Pattern:** Hexagonal Grid
**Icon:** Chain Links
**Animation:** Flow Lines
**Prefix:** bc

```html
<svg viewBox="0 0 820 180" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="xMidYMid slice">
  <defs>
    <linearGradient id="bc-bg" x1="0" y1="0" x2="1" y2="1">
      <stop offset="0%" stop-color="#0A0F1E"/>
      <stop offset="100%" stop-color="#1E3A5F"/>
    </linearGradient>
    <filter id="bc-glow">
      <feGaussianBlur stdDeviation="4" result="blur"/>
      <feMerge><feMergeNode in="blur"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
    <style>
      @keyframes bc-flow { 0% { stroke-dashoffset: 160; } 100% { stroke-dashoffset: 0; } }
      @keyframes bc-breathe { 0%,100% { r: 4; opacity: 0.9; } 50% { r: 6; opacity: 0.5; } }
      .bc-flow { stroke-dasharray: 160; animation: bc-flow 2s linear infinite; }
      .bc-node { animation: bc-breathe 2s ease-in-out infinite; }
    </style>
  </defs>
  <rect width="820" height="180" fill="url(#bc-bg)"/>
  <!-- Hex grid -->
  <g opacity="0.06" stroke="#38BDF8" stroke-width="0.5" fill="none">
    <polygon points="60,30 78,20 96,30 96,50 78,60 60,50"/>
    <polygon points="96,30 114,20 132,30 132,50 114,60 96,50"/>
    <polygon points="300,90 318,80 336,90 336,110 318,120 300,110"/>
    <polygon points="500,40 518,30 536,40 536,60 518,70 500,60"/>
    <polygon points="420,130 438,120 456,130 456,150 438,160 420,150"/>
  </g>
  <!-- Blockchain chain -->
  <g transform="translate(100,90)">
    <!-- Block 1 -->
    <rect x="-20" y="-18" width="36" height="36" rx="4" fill="none" stroke="#38BDF8" stroke-width="1.5" opacity="0.7"/>
    <circle cx="-2" cy="0" r="4" fill="#38BDF8" opacity="0.8" class="bc-node"/>
    <!-- Chain link 1->2 -->
    <line x1="16" y1="0" x2="50" y2="0" stroke="#38BDF8" stroke-width="1" opacity="0.4" class="bc-flow"/>
    <!-- Block 2 -->
    <rect x="50" y="-18" width="36" height="36" rx="4" fill="none" stroke="#38BDF8" stroke-width="1.5" opacity="0.7"/>
    <circle cx="68" cy="0" r="4" fill="#38BDF8" opacity="0.8" class="bc-node" style="animation-delay:0.3s"/>
    <!-- Chain link 2->3 -->
    <line x1="86" y1="0" x2="120" y2="0" stroke="#38BDF8" stroke-width="1" opacity="0.4" class="bc-flow" style="animation-delay:0.5s"/>
    <!-- Block 3 -->
    <rect x="120" y="-18" width="36" height="36" rx="4" fill="none" stroke="#38BDF8" stroke-width="1.5" opacity="0.7"/>
    <circle cx="138" cy="0" r="4" fill="#38BDF8" opacity="0.8" class="bc-node" style="animation-delay:0.6s"/>
    <!-- Hash lines inside blocks -->
    <line x1="-14" y1="-8" x2="8" y2="-8" stroke="#38BDF8" stroke-width="0.5" opacity="0.3"/>
    <line x1="-14" y1="-2" x2="6" y2="-2" stroke="#38BDF8" stroke-width="0.5" opacity="0.3"/>
    <line x1="56" y1="-8" x2="78" y2="-8" stroke="#38BDF8" stroke-width="0.5" opacity="0.3"/>
    <line x1="56" y1="-2" x2="76" y2="-2" stroke="#38BDF8" stroke-width="0.5" opacity="0.3"/>
    <line x1="126" y1="-8" x2="148" y2="-8" stroke="#38BDF8" stroke-width="0.5" opacity="0.3"/>
    <line x1="126" y1="-2" x2="146" y2="-2" stroke="#38BDF8" stroke-width="0.5" opacity="0.3"/>
  </g>
  <!-- Decorative orbs -->
  <circle cx="660" cy="85" r="52" fill="#1E3A5F" opacity="0.22"/>
  <circle cx="660" cy="85" r="32" fill="#1E3A5F" opacity="0.16"/>
  <circle cx="660" cy="85" r="15" fill="#38BDF8" opacity="0.2"/>
  <circle cx="660" cy="85" r="6" fill="#38BDF8" opacity="0.5" filter="url(#bc-glow)"/>
  <circle cx="750" cy="50" r="20" fill="#1E3A5F" opacity="0.14"/>
  <circle cx="750" cy="50" r="7" fill="#38BDF8" opacity="0.2"/>
  <line x1="660" y1="85" x2="750" y2="50" stroke="#38BDF8" stroke-width="0.5" opacity="0.18"/>
  <circle cx="740" cy="140" r="16" fill="#1E3A5F" opacity="0.1"/>
  <circle cx="740" cy="140" r="5" fill="#38BDF8" opacity="0.18"/>
  <line x1="660" y1="85" x2="740" y2="140" stroke="#38BDF8" stroke-width="0.5" opacity="0.12"/>
</svg>
```

---

## SVG 8: Digital Marketing & SEO
**Sector:** Technology
**Palette:** Custom Marketing (#0F172A / #1E3A5F / #F472B6)
**Pattern:** Dot Grid
**Icon:** Arrow (trending up)
**Animation:** Breathe Nodes
**Prefix:** dm

```html
<svg viewBox="0 0 820 180" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="xMidYMid slice">
  <defs>
    <linearGradient id="dm-bg" x1="0" y1="0" x2="1" y2="1">
      <stop offset="0%" stop-color="#0F172A"/>
      <stop offset="100%" stop-color="#1E3A5F"/>
    </linearGradient>
    <filter id="dm-glow">
      <feGaussianBlur stdDeviation="4" result="blur"/>
      <feMerge><feMergeNode in="blur"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
    <style>
      @keyframes dm-breathe { 0%,100% { r: 4; opacity: 0.9; } 50% { r: 6; opacity: 0.4; } }
      .dm-node { animation: dm-breathe 2s ease-in-out infinite; }
    </style>
  </defs>
  <rect width="820" height="180" fill="url(#dm-bg)"/>
  <!-- Dot grid -->
  <g opacity="0.07" fill="#F472B6">
    <circle cx="40" cy="40" r="1.5"/><circle cx="100" cy="40" r="1.5"/><circle cx="160" cy="40" r="1.5"/><circle cx="220" cy="40" r="1.5"/><circle cx="280" cy="40" r="1.5"/><circle cx="340" cy="40" r="1.5"/><circle cx="400" cy="40" r="1.5"/><circle cx="460" cy="40" r="1.5"/><circle cx="520" cy="40" r="1.5"/><circle cx="580" cy="40" r="1.5"/><circle cx="640" cy="40" r="1.5"/><circle cx="700" cy="40" r="1.5"/><circle cx="760" cy="40" r="1.5"/>
    <circle cx="40" cy="100" r="1.5"/><circle cx="100" cy="100" r="1.5"/><circle cx="160" cy="100" r="1.5"/><circle cx="220" cy="100" r="1.5"/><circle cx="280" cy="100" r="1.5"/><circle cx="340" cy="100" r="1.5"/><circle cx="400" cy="100" r="1.5"/><circle cx="460" cy="100" r="1.5"/><circle cx="520" cy="100" r="1.5"/><circle cx="580" cy="100" r="1.5"/><circle cx="640" cy="100" r="1.5"/><circle cx="700" cy="100" r="1.5"/><circle cx="760" cy="100" r="1.5"/>
    <circle cx="40" cy="160" r="1.5"/><circle cx="100" cy="160" r="1.5"/><circle cx="160" cy="160" r="1.5"/><circle cx="220" cy="160" r="1.5"/><circle cx="280" cy="160" r="1.5"/><circle cx="340" cy="160" r="1.5"/><circle cx="400" cy="160" r="1.5"/><circle cx="460" cy="160" r="1.5"/><circle cx="520" cy="160" r="1.5"/><circle cx="580" cy="160" r="1.5"/><circle cx="640" cy="160" r="1.5"/><circle cx="700" cy="160" r="1.5"/><circle cx="760" cy="160" r="1.5"/>
  </g>
  <!-- Trending arrow icon -->
  <g transform="translate(140,100)">
    <polyline points="-40,30 -10,5 20,-15 50,-40" fill="none" stroke="#F472B6" stroke-width="2.5" stroke-linecap="round" opacity="0.7"/>
    <!-- Arrow head -->
    <polygon points="50,-40 38,-42 48,-30" fill="#F472B6" opacity="0.7"/>
    <!-- Data nodes on line -->
    <circle cx="-40" cy="30" r="4" fill="#F472B6" opacity="0.8" class="dm-node"/>
    <circle cx="-10" cy="5" r="4" fill="#F472B6" opacity="0.8" class="dm-node" style="animation-delay:0.3s"/>
    <circle cx="20" cy="-15" r="4" fill="#F472B6" opacity="0.8" class="dm-node" style="animation-delay:0.6s"/>
    <circle cx="50" cy="-40" r="5" fill="#F472B6" opacity="0.9" class="dm-node" style="animation-delay:0.9s" filter="url(#dm-glow)"/>
    <!-- Vertical reference lines -->
    <line x1="-40" y1="34" x2="-40" y2="50" stroke="#F472B6" stroke-width="0.5" opacity="0.2"/>
    <line x1="-10" y1="9" x2="-10" y2="50" stroke="#F472B6" stroke-width="0.5" opacity="0.2"/>
    <line x1="20" y1="-11" x2="20" y2="50" stroke="#F472B6" stroke-width="0.5" opacity="0.2"/>
    <line x1="50" y1="-36" x2="50" y2="50" stroke="#F472B6" stroke-width="0.5" opacity="0.2"/>
  </g>
  <!-- Decorative orbs -->
  <circle cx="660" cy="85" r="50" fill="#1E3A5F" opacity="0.2"/>
  <circle cx="660" cy="85" r="30" fill="#1E3A5F" opacity="0.14"/>
  <circle cx="660" cy="85" r="14" fill="#F472B6" opacity="0.2"/>
  <circle cx="660" cy="85" r="5" fill="#F472B6" opacity="0.5" filter="url(#dm-glow)"/>
  <circle cx="750" cy="50" r="18" fill="#1E3A5F" opacity="0.12"/>
  <circle cx="750" cy="50" r="6" fill="#F472B6" opacity="0.18"/>
  <line x1="660" y1="85" x2="750" y2="50" stroke="#F472B6" stroke-width="0.5" opacity="0.15"/>
  <circle cx="740" cy="140" r="14" fill="#1E3A5F" opacity="0.1"/>
  <circle cx="740" cy="140" r="4" fill="#F472B6" opacity="0.15"/>
  <line x1="660" y1="85" x2="740" y2="140" stroke="#F472B6" stroke-width="0.5" opacity="0.12"/>
</svg>
```

---

## SVG 9: Project Management & Agile
**Sector:** Technology
**Palette:** Custom PM (#0F172A / #2D3A6B / #A78BFA)
**Pattern:** Horizontal Lines
**Icon:** Arrow (upward with nodes)
**Animation:** Flow Lines
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
      @keyframes pm-flow { 0% { stroke-dashoffset: 200; } 100% { stroke-dashoffset: 0; } }
      @keyframes pm-breathe { 0%,100% { r: 5; opacity: 1; } 50% { r: 7; opacity: 0.5; } }
      .pm-flow { stroke-dasharray: 200; animation: pm-flow 2.5s linear infinite; }
      .pm-node { animation: pm-breathe 2.2s ease-in-out infinite; }
    </style>
  </defs>
  <rect width="820" height="180" fill="url(#pm-bg)"/>
  <!-- Horizontal lines -->
  <g opacity="0.06" stroke="#A78BFA" stroke-width="0.5">
    <line x1="0" y1="36" x2="820" y2="36"/>
    <line x1="0" y1="72" x2="820" y2="72"/>
    <line x1="0" y1="108" x2="820" y2="108"/>
    <line x1="0" y1="144" x2="820" y2="144"/>
  </g>
  <!-- Kanban / sprint board icon -->
  <g transform="translate(130,90)">
    <!-- Columns -->
    <rect x="-50" y="-50" width="35" height="100" rx="3" fill="none" stroke="#A78BFA" stroke-width="1" opacity="0.4"/>
    <rect x="-10" y="-50" width="35" height="100" rx="3" fill="none" stroke="#A78BFA" stroke-width="1" opacity="0.4"/>
    <rect x="30" y="-50" width="35" height="100" rx="3" fill="none" stroke="#A78BFA" stroke-width="1" opacity="0.4"/>
    <!-- Cards in columns -->
    <rect x="-45" y="-42" width="25" height="14" rx="2" fill="#A78BFA" opacity="0.3"/>
    <rect x="-45" y="-24" width="25" height="14" rx="2" fill="#A78BFA" opacity="0.2"/>
    <rect x="-5" y="-42" width="25" height="14" rx="2" fill="#A78BFA" opacity="0.4"/>
    <rect x="35" y="-42" width="25" height="14" rx="2" fill="#A78BFA" opacity="0.5"/>
    <rect x="35" y="-24" width="25" height="14" rx="2" fill="#A78BFA" opacity="0.35"/>
    <rect x="35" y="-6" width="25" height="14" rx="2" fill="#A78BFA" opacity="0.25"/>
    <!-- Flow arrows between columns -->
    <path d="M-15,20 H-5" stroke="#A78BFA" stroke-width="1" opacity="0.5" class="pm-flow" marker-end="none"/>
    <path d="M25,20 H35" stroke="#A78BFA" stroke-width="1" opacity="0.5" class="pm-flow" style="animation-delay:0.5s"/>
    <!-- Sprint cycle arrow -->
    <path d="M70,-20 C85,-20 85,20 70,20" fill="none" stroke="#A78BFA" stroke-width="1" opacity="0.4"/>
    <circle cx="70" cy="-20" r="3" fill="#A78BFA" opacity="0.6" class="pm-node"/>
    <circle cx="70" cy="20" r="3" fill="#A78BFA" opacity="0.6" class="pm-node" style="animation-delay:0.5s"/>
  </g>
  <!-- Decorative orbs -->
  <circle cx="660" cy="90" r="52" fill="#2D3A6B" opacity="0.22"/>
  <circle cx="660" cy="90" r="32" fill="#2D3A6B" opacity="0.15"/>
  <circle cx="660" cy="90" r="15" fill="#A78BFA" opacity="0.2"/>
  <circle cx="660" cy="90" r="6" fill="#A78BFA" opacity="0.5" filter="url(#pm-glow)"/>
  <circle cx="750" cy="52" r="20" fill="#2D3A6B" opacity="0.14"/>
  <circle cx="750" cy="52" r="7" fill="#A78BFA" opacity="0.2"/>
  <line x1="660" y1="90" x2="750" y2="52" stroke="#A78BFA" stroke-width="0.5" opacity="0.18"/>
  <circle cx="742" cy="142" r="16" fill="#2D3A6B" opacity="0.1"/>
  <circle cx="742" cy="142" r="5" fill="#A78BFA" opacity="0.18"/>
  <line x1="660" y1="90" x2="742" y2="142" stroke="#A78BFA" stroke-width="0.5" opacity="0.14"/>
</svg>
```

---

## SVG 10: IoT & Embedded Systems
**Sector:** Technology / Manufacturing
**Palette:** Custom IoT (#0F172A / #1A3A4A / #2DD4BF)
**Pattern:** Circuit Traces
**Icon:** Gear with connection nodes
**Animation:** Breathe + Flow
**Prefix:** io

```html
<svg viewBox="0 0 820 180" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="xMidYMid slice">
  <defs>
    <linearGradient id="io-bg" x1="0" y1="0" x2="1" y2="1">
      <stop offset="0%" stop-color="#0F172A"/>
      <stop offset="100%" stop-color="#1A3A4A"/>
    </linearGradient>
    <filter id="io-glow">
      <feGaussianBlur stdDeviation="4" result="blur"/>
      <feMerge><feMergeNode in="blur"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
    <style>
      @keyframes io-breathe { 0%,100% { r: 4; opacity: 0.9; } 50% { r: 6; opacity: 0.4; } }
      @keyframes io-flow { 0% { stroke-dashoffset: 160; } 100% { stroke-dashoffset: 0; } }
      .io-node { animation: io-breathe 2s ease-in-out infinite; }
      .io-flow { stroke-dasharray: 160; animation: io-flow 2.2s linear infinite; }
    </style>
  </defs>
  <rect width="820" height="180" fill="url(#io-bg)"/>
  <!-- Circuit traces -->
  <g opacity="0.1" stroke="#2DD4BF" stroke-width="0.7" fill="none">
    <path d="M0,40 H60 V20 H130 V40 H200"/>
    <path d="M0,100 H80 V80 H160 V100 H240"/>
    <path d="M0,150 H50 V130 H140 V150 H220"/>
    <path d="M400,50 H490 V70 H560"/>
    <path d="M420,140 H500 V120 H580"/>
    <circle cx="60" cy="40" r="2" fill="#2DD4BF" stroke="none"/>
    <circle cx="130" cy="20" r="2" fill="#2DD4BF" stroke="none"/>
    <circle cx="160" cy="80" r="2" fill="#2DD4BF" stroke="none"/>
  </g>
  <!-- Central hub (gear-like) -->
  <g transform="translate(160,90)">
    <!-- Outer ring -->
    <circle cx="0" cy="0" r="30" fill="none" stroke="#2DD4BF" stroke-width="1.5" opacity="0.5"/>
    <!-- Inner core -->
    <circle cx="0" cy="0" r="15" fill="#1A3A4A" opacity="0.6" stroke="#2DD4BF" stroke-width="1" />
    <circle cx="0" cy="0" r="6" fill="#2DD4BF" opacity="0.5" filter="url(#io-glow)"/>
    <!-- Gear teeth (simplified as radiating lines) -->
    <line x1="0" y1="-30" x2="0" y2="-40" stroke="#2DD4BF" stroke-width="2" opacity="0.5"/>
    <line x1="21" y1="-21" x2="28" y2="-28" stroke="#2DD4BF" stroke-width="2" opacity="0.5"/>
    <line x1="30" y1="0" x2="40" y2="0" stroke="#2DD4BF" stroke-width="2" opacity="0.5"/>
    <line x1="21" y1="21" x2="28" y2="28" stroke="#2DD4BF" stroke-width="2" opacity="0.5"/>
    <line x1="0" y1="30" x2="0" y2="40" stroke="#2DD4BF" stroke-width="2" opacity="0.5"/>
    <line x1="-21" y1="21" x2="-28" y2="28" stroke="#2DD4BF" stroke-width="2" opacity="0.5"/>
    <line x1="-30" y1="0" x2="-40" y2="0" stroke="#2DD4BF" stroke-width="2" opacity="0.5"/>
    <line x1="-21" y1="-21" x2="-28" y2="-28" stroke="#2DD4BF" stroke-width="2" opacity="0.5"/>
    <!-- Connected IoT nodes -->
    <circle cx="0" cy="-48" r="4" fill="#2DD4BF" opacity="0.7" class="io-node"/>
    <circle cx="48" cy="0" r="4" fill="#2DD4BF" opacity="0.7" class="io-node" style="animation-delay:0.3s"/>
    <circle cx="0" cy="48" r="4" fill="#2DD4BF" opacity="0.7" class="io-node" style="animation-delay:0.6s"/>
    <circle cx="-48" cy="0" r="4" fill="#2DD4BF" opacity="0.7" class="io-node" style="animation-delay:0.9s"/>
    <!-- Flow lines to distant nodes -->
    <line x1="0" y1="-52" x2="0" y2="-70" stroke="#2DD4BF" stroke-width="0.8" opacity="0.3" class="io-flow"/>
    <line x1="52" y1="0" x2="75" y2="0" stroke="#2DD4BF" stroke-width="0.8" opacity="0.3" class="io-flow" style="animation-delay:0.4s"/>
  </g>
  <!-- Decorative orbs -->
  <circle cx="660" cy="85" r="50" fill="#1A3A4A" opacity="0.22"/>
  <circle cx="660" cy="85" r="30" fill="#1A3A4A" opacity="0.15"/>
  <circle cx="660" cy="85" r="14" fill="#2DD4BF" opacity="0.2"/>
  <circle cx="660" cy="85" r="5" fill="#2DD4BF" opacity="0.5" filter="url(#io-glow)"/>
  <circle cx="750" cy="50" r="18" fill="#1A3A4A" opacity="0.12"/>
  <circle cx="750" cy="50" r="6" fill="#2DD4BF" opacity="0.18"/>
  <line x1="660" y1="85" x2="750" y2="50" stroke="#2DD4BF" stroke-width="0.5" opacity="0.15"/>
  <circle cx="740" cy="140" r="14" fill="#1A3A4A" opacity="0.1"/>
  <circle cx="740" cy="140" r="5" fill="#2DD4BF" opacity="0.15"/>
  <line x1="660" y1="85" x2="740" y2="140" stroke="#2DD4BF" stroke-width="0.5" opacity="0.12"/>
</svg>
```

---

## SVG 11: Semiconductor & VLSI Design
**Sector:** Technology / Hardware
**Palette:** Custom Semiconductor (#0A0F1E / #1E2D5A / #F59E0B)
**Pattern:** Circuit Traces
**Icon:** Chip (microprocessor)
**Animation:** Pulse + Flow
**Prefix:** sc

```html
<svg viewBox="0 0 820 180" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="xMidYMid slice">
  <defs>
    <linearGradient id="sc-bg" x1="0" y1="0" x2="1" y2="1">
      <stop offset="0%" stop-color="#0A0F1E"/>
      <stop offset="100%" stop-color="#1E2D5A"/>
    </linearGradient>
    <filter id="sc-glow">
      <feGaussianBlur stdDeviation="5" result="blur"/>
      <feMerge><feMergeNode in="blur"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
    <style>
      @keyframes sc-pulse { 0% { r: 10; opacity: 0.5; } 100% { r: 35; opacity: 0; } }
      @keyframes sc-flow { 0% { stroke-dashoffset: 140; } 100% { stroke-dashoffset: 0; } }
      .sc-ring { animation: sc-pulse 2.5s ease-out infinite; }
      .sc-flow { stroke-dasharray: 140; animation: sc-flow 1.8s linear infinite; }
    </style>
  </defs>
  <rect width="820" height="180" fill="url(#sc-bg)"/>
  <!-- Circuit traces -->
  <g opacity="0.08" stroke="#F59E0B" stroke-width="0.7" fill="none">
    <path d="M0,35 H70 V55 H150"/>
    <path d="M0,95 H60 V75 H140 V95 H210"/>
    <path d="M0,145 H80 V125 H160"/>
    <path d="M450,30 H530 V50 H600"/>
    <path d="M430,150 H510 V130 H590"/>
    <circle cx="70" cy="35" r="2" fill="#F59E0B" stroke="none"/>
    <circle cx="140" cy="75" r="2" fill="#F59E0B" stroke="none"/>
  </g>
  <!-- Chip icon (detailed) -->
  <g transform="translate(165,90)">
    <!-- Chip body -->
    <rect x="-32" y="-32" width="64" height="64" rx="4" fill="#1E2D5A" opacity="0.5" stroke="#F59E0B" stroke-width="1.5"/>
    <!-- Die -->
    <rect x="-18" y="-18" width="36" height="36" rx="2" fill="#F59E0B" opacity="0.08" stroke="#F59E0B" stroke-width="0.8"/>
    <!-- Core -->
    <circle cx="0" cy="0" r="8" fill="#F59E0B" opacity="0.3" filter="url(#sc-glow)"/>
    <circle cx="0" cy="0" r="3" fill="#F59E0B" opacity="0.8"/>
    <!-- Pins (top) -->
    <line x1="-18" y1="-32" x2="-18" y2="-45" stroke="#F59E0B" stroke-width="1" opacity="0.5" class="sc-flow"/>
    <line x1="-6" y1="-32" x2="-6" y2="-48" stroke="#F59E0B" stroke-width="1" opacity="0.5" class="sc-flow" style="animation-delay:0.2s"/>
    <line x1="6" y1="-32" x2="6" y2="-48" stroke="#F59E0B" stroke-width="1" opacity="0.5" class="sc-flow" style="animation-delay:0.4s"/>
    <line x1="18" y1="-32" x2="18" y2="-45" stroke="#F59E0B" stroke-width="1" opacity="0.5" class="sc-flow" style="animation-delay:0.6s"/>
    <!-- Pins (bottom) -->
    <line x1="-18" y1="32" x2="-18" y2="45" stroke="#F59E0B" stroke-width="1" opacity="0.5" class="sc-flow" style="animation-delay:0.3s"/>
    <line x1="-6" y1="32" x2="-6" y2="48" stroke="#F59E0B" stroke-width="1" opacity="0.5" class="sc-flow" style="animation-delay:0.5s"/>
    <line x1="6" y1="32" x2="6" y2="48" stroke="#F59E0B" stroke-width="1" opacity="0.5" class="sc-flow" style="animation-delay:0.7s"/>
    <line x1="18" y1="32" x2="18" y2="45" stroke="#F59E0B" stroke-width="1" opacity="0.5" class="sc-flow" style="animation-delay:0.9s"/>
    <!-- Pins (left) -->
    <line x1="-32" y1="-15" x2="-48" y2="-15" stroke="#F59E0B" stroke-width="1" opacity="0.5"/>
    <line x1="-32" y1="0" x2="-50" y2="0" stroke="#F59E0B" stroke-width="1" opacity="0.5"/>
    <line x1="-32" y1="15" x2="-48" y2="15" stroke="#F59E0B" stroke-width="1" opacity="0.5"/>
    <!-- Pins (right) -->
    <line x1="32" y1="-15" x2="48" y2="-15" stroke="#F59E0B" stroke-width="1" opacity="0.5"/>
    <line x1="32" y1="0" x2="50" y2="0" stroke="#F59E0B" stroke-width="1" opacity="0.5"/>
    <line x1="32" y1="15" x2="48" y2="15" stroke="#F59E0B" stroke-width="1" opacity="0.5"/>
  </g>
  <!-- Pulse ring -->
  <circle cx="165" cy="90" r="10" fill="none" stroke="#F59E0B" stroke-width="0.8" class="sc-ring"/>
  <circle cx="165" cy="90" r="10" fill="none" stroke="#F59E0B" stroke-width="0.8" class="sc-ring" style="animation-delay:0.8s"/>
  <!-- Decorative orbs -->
  <circle cx="660" cy="85" r="50" fill="#1E2D5A" opacity="0.2"/>
  <circle cx="660" cy="85" r="30" fill="#1E2D5A" opacity="0.14"/>
  <circle cx="660" cy="85" r="14" fill="#F59E0B" opacity="0.2"/>
  <circle cx="660" cy="85" r="5" fill="#F59E0B" opacity="0.5" filter="url(#sc-glow)"/>
  <circle cx="750" cy="48" r="20" fill="#1E2D5A" opacity="0.12"/>
  <circle cx="750" cy="48" r="7" fill="#F59E0B" opacity="0.18"/>
  <line x1="660" y1="85" x2="750" y2="48" stroke="#F59E0B" stroke-width="0.5" opacity="0.16"/>
  <circle cx="742" cy="142" r="15" fill="#1E2D5A" opacity="0.1"/>
  <circle cx="742" cy="142" r="5" fill="#F59E0B" opacity="0.16"/>
  <line x1="660" y1="85" x2="742" y2="142" stroke="#F59E0B" stroke-width="0.5" opacity="0.12"/>
</svg>
```

---

## SVG 12: Green Energy & Sustainability
**Sector:** Green Energy
**Palette:** Green Energy (#031A0A / #14532D / #4ADE80)
**Pattern:** Diagonal Lines
**Icon:** Leaf / Wind Turbine
**Animation:** Breathe + Flow
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
      @keyframes ge-breathe { 0%,100% { opacity: 0.7; } 50% { opacity: 0.3; } }
      @keyframes ge-spin { 0% { transform: rotate(0deg); } 100% { transform: rotate(360deg); } }
      .ge-leaf { animation: ge-breathe 3s ease-in-out infinite; }
      .ge-turbine { animation: ge-spin 6s linear infinite; transform-origin: 0px 0px; }
    </style>
  </defs>
  <rect width="820" height="180" fill="url(#ge-bg)"/>
  <!-- Diagonal lines -->
  <g opacity="0.05" stroke="#4ADE80" stroke-width="0.5">
    <line x1="0" y1="0" x2="180" y2="180"/><line x1="80" y1="0" x2="260" y2="180"/>
    <line x1="160" y1="0" x2="340" y2="180"/><line x1="240" y1="0" x2="420" y2="180"/>
    <line x1="320" y1="0" x2="500" y2="180"/><line x1="400" y1="0" x2="580" y2="180"/>
    <line x1="480" y1="0" x2="660" y2="180"/><line x1="560" y1="0" x2="740" y2="180"/>
    <line x1="640" y1="0" x2="820" y2="180"/>
  </g>
  <!-- Leaf icon -->
  <g transform="translate(140,85)">
    <!-- Leaf shape -->
    <path d="M0,-45 C30,-40 45,-15 40,15 C35,40 10,50 0,50 C-10,50 -35,40 -40,15 C-45,-15 -30,-40 0,-45Z" fill="#4ADE80" opacity="0.12" stroke="#4ADE80" stroke-width="1.2" class="ge-leaf"/>
    <!-- Leaf veins -->
    <line x1="0" y1="-40" x2="0" y2="45" stroke="#4ADE80" stroke-width="0.8" opacity="0.4"/>
    <path d="M0,-20 C15,-15 25,-5 30,5" fill="none" stroke="#4ADE80" stroke-width="0.6" opacity="0.3"/>
    <path d="M0,-5 C-15,0 -25,10 -28,18" fill="none" stroke="#4ADE80" stroke-width="0.6" opacity="0.3"/>
    <path d="M0,15 C12,18 20,25 22,30" fill="none" stroke="#4ADE80" stroke-width="0.6" opacity="0.3"/>
    <!-- Center glow -->
    <circle cx="0" cy="5" r="6" fill="#4ADE80" opacity="0.4" filter="url(#ge-glow)"/>
  </g>
  <!-- Small wind turbine (right of center) -->
  <g transform="translate(280,90)">
    <!-- Tower -->
    <line x1="0" y1="0" x2="0" y2="50" stroke="#4ADE80" stroke-width="1" opacity="0.4"/>
    <!-- Blades (rotating) -->
    <g class="ge-turbine">
      <line x1="0" y1="0" x2="0" y2="-25" stroke="#4ADE80" stroke-width="1.5" opacity="0.5" stroke-linecap="round"/>
      <line x1="0" y1="0" x2="22" y2="12" stroke="#4ADE80" stroke-width="1.5" opacity="0.5" stroke-linecap="round"/>
      <line x1="0" y1="0" x2="-22" y2="12" stroke="#4ADE80" stroke-width="1.5" opacity="0.5" stroke-linecap="round"/>
    </g>
    <circle cx="0" cy="0" r="3" fill="#4ADE80" opacity="0.7"/>
  </g>
  <!-- Decorative orbs -->
  <circle cx="660" cy="85" r="52" fill="#14532D" opacity="0.22"/>
  <circle cx="660" cy="85" r="32" fill="#14532D" opacity="0.15"/>
  <circle cx="660" cy="85" r="15" fill="#4ADE80" opacity="0.2"/>
  <circle cx="660" cy="85" r="6" fill="#4ADE80" opacity="0.5" filter="url(#ge-glow)"/>
  <circle cx="750" cy="48" r="20" fill="#14532D" opacity="0.14"/>
  <circle cx="750" cy="48" r="7" fill="#4ADE80" opacity="0.2"/>
  <line x1="660" y1="85" x2="750" y2="48" stroke="#4ADE80" stroke-width="0.5" opacity="0.18"/>
  <circle cx="740" cy="142" r="16" fill="#14532D" opacity="0.1"/>
  <circle cx="740" cy="142" r="5" fill="#4ADE80" opacity="0.16"/>
  <line x1="660" y1="85" x2="740" y2="142" stroke="#4ADE80" stroke-width="0.5" opacity="0.12"/>
</svg>
```

---

## SVG 13: RPA & Intelligent Automation
**Sector:** Technology
**Palette:** Custom Automation (#0F172A / #1E2D4A / #FB923C)
**Pattern:** Dot Grid
**Icon:** Gear (interlocking)
**Animation:** Flow + Breathe
**Prefix:** rp

```html
<svg viewBox="0 0 820 180" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="xMidYMid slice">
  <defs>
    <linearGradient id="rp-bg" x1="0" y1="0" x2="1" y2="1">
      <stop offset="0%" stop-color="#0F172A"/>
      <stop offset="100%" stop-color="#1E2D4A"/>
    </linearGradient>
    <filter id="rp-glow">
      <feGaussianBlur stdDeviation="4" result="blur"/>
      <feMerge><feMergeNode in="blur"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
    <style>
      @keyframes rp-flow { 0% { stroke-dashoffset: 180; } 100% { stroke-dashoffset: 0; } }
      @keyframes rp-breathe { 0%,100% { r: 4; opacity: 0.9; } 50% { r: 6; opacity: 0.4; } }
      @keyframes rp-spin-cw { 0% { transform: rotate(0deg); } 100% { transform: rotate(360deg); } }
      @keyframes rp-spin-ccw { 0% { transform: rotate(0deg); } 100% { transform: rotate(-360deg); } }
      .rp-flow { stroke-dasharray: 180; animation: rp-flow 2s linear infinite; }
      .rp-node { animation: rp-breathe 2s ease-in-out infinite; }
      .rp-gear1 { animation: rp-spin-cw 8s linear infinite; transform-origin: -15px -10px; }
      .rp-gear2 { animation: rp-spin-ccw 8s linear infinite; transform-origin: 18px 12px; }
    </style>
  </defs>
  <rect width="820" height="180" fill="url(#rp-bg)"/>
  <!-- Dot grid -->
  <g opacity="0.06" fill="#FB923C">
    <circle cx="40" cy="30" r="1.5"/><circle cx="100" cy="30" r="1.5"/><circle cx="160" cy="30" r="1.5"/><circle cx="220" cy="30" r="1.5"/><circle cx="280" cy="30" r="1.5"/><circle cx="340" cy="30" r="1.5"/><circle cx="400" cy="30" r="1.5"/><circle cx="460" cy="30" r="1.5"/><circle cx="520" cy="30" r="1.5"/><circle cx="580" cy="30" r="1.5"/><circle cx="640" cy="30" r="1.5"/><circle cx="700" cy="30" r="1.5"/><circle cx="760" cy="30" r="1.5"/>
    <circle cx="40" cy="90" r="1.5"/><circle cx="100" cy="90" r="1.5"/><circle cx="160" cy="90" r="1.5"/><circle cx="220" cy="90" r="1.5"/><circle cx="280" cy="90" r="1.5"/><circle cx="340" cy="90" r="1.5"/><circle cx="400" cy="90" r="1.5"/><circle cx="460" cy="90" r="1.5"/><circle cx="520" cy="90" r="1.5"/><circle cx="580" cy="90" r="1.5"/><circle cx="640" cy="90" r="1.5"/><circle cx="700" cy="90" r="1.5"/><circle cx="760" cy="90" r="1.5"/>
    <circle cx="40" cy="150" r="1.5"/><circle cx="100" cy="150" r="1.5"/><circle cx="160" cy="150" r="1.5"/><circle cx="220" cy="150" r="1.5"/><circle cx="280" cy="150" r="1.5"/><circle cx="340" cy="150" r="1.5"/><circle cx="400" cy="150" r="1.5"/><circle cx="460" cy="150" r="1.5"/><circle cx="520" cy="150" r="1.5"/><circle cx="580" cy="150" r="1.5"/><circle cx="640" cy="150" r="1.5"/><circle cx="700" cy="150" r="1.5"/><circle cx="760" cy="150" r="1.5"/>
  </g>
  <!-- Interlocking gears -->
  <g transform="translate(160,90)">
    <!-- Gear 1 (larger) -->
    <g class="rp-gear1">
      <circle cx="-15" cy="-10" r="22" fill="none" stroke="#FB923C" stroke-width="1.5" opacity="0.5"/>
      <circle cx="-15" cy="-10" r="10" fill="#1E2D4A" opacity="0.6" stroke="#FB923C" stroke-width="0.8"/>
      <!-- Teeth -->
      <line x1="-15" y1="-32" x2="-15" y2="-38" stroke="#FB923C" stroke-width="3" opacity="0.4"/>
      <line x1="-37" y1="-10" x2="-43" y2="-10" stroke="#FB923C" stroke-width="3" opacity="0.4"/>
      <line x1="-15" y1="12" x2="-15" y2="18" stroke="#FB923C" stroke-width="3" opacity="0.4"/>
      <line x1="7" y1="-10" x2="13" y2="-10" stroke="#FB923C" stroke-width="3" opacity="0.4"/>
      <line x1="-30" y1="-25" x2="-35" y2="-30" stroke="#FB923C" stroke-width="3" opacity="0.4"/>
      <line x1="0" y1="-25" x2="5" y2="-30" stroke="#FB923C" stroke-width="3" opacity="0.4"/>
      <line x1="-30" y1="5" x2="-35" y2="10" stroke="#FB923C" stroke-width="3" opacity="0.4"/>
      <line x1="0" y1="5" x2="5" y2="10" stroke="#FB923C" stroke-width="3" opacity="0.4"/>
    </g>
    <!-- Gear 2 (smaller) -->
    <g class="rp-gear2">
      <circle cx="18" cy="12" r="16" fill="none" stroke="#FB923C" stroke-width="1.5" opacity="0.5"/>
      <circle cx="18" cy="12" r="7" fill="#1E2D4A" opacity="0.6" stroke="#FB923C" stroke-width="0.8"/>
      <!-- Teeth -->
      <line x1="18" y1="-4" x2="18" y2="-9" stroke="#FB923C" stroke-width="2.5" opacity="0.4"/>
      <line x1="34" y1="12" x2="39" y2="12" stroke="#FB923C" stroke-width="2.5" opacity="0.4"/>
      <line x1="18" y1="28" x2="18" y2="33" stroke="#FB923C" stroke-width="2.5" opacity="0.4"/>
      <line x1="2" y1="12" x2="-3" y2="12" stroke="#FB923C" stroke-width="2.5" opacity="0.4"/>
      <line x1="29" y1="1" x2="33" y2="-3" stroke="#FB923C" stroke-width="2.5" opacity="0.4"/>
      <line x1="29" y1="23" x2="33" y2="27" stroke="#FB923C" stroke-width="2.5" opacity="0.4"/>
    </g>
    <!-- Center dots -->
    <circle cx="-15" cy="-10" r="3" fill="#FB923C" opacity="0.7" filter="url(#rp-glow)"/>
    <circle cx="18" cy="12" r="2.5" fill="#FB923C" opacity="0.6"/>
    <!-- Process flow arrows -->
    <path d="M-60,0 H-45" stroke="#FB923C" stroke-width="1" opacity="0.4" class="rp-flow"/>
    <path d="M40,0 H60" stroke="#FB923C" stroke-width="1" opacity="0.4" class="rp-flow" style="animation-delay:0.5s"/>
    <circle cx="-65" cy="0" r="4" fill="#FB923C" opacity="0.6" class="rp-node"/>
    <circle cx="65" cy="0" r="4" fill="#FB923C" opacity="0.6" class="rp-node" style="animation-delay:0.5s"/>
  </g>
  <!-- Decorative orbs -->
  <circle cx="660" cy="85" r="50" fill="#1E2D4A" opacity="0.2"/>
  <circle cx="660" cy="85" r="30" fill="#1E2D4A" opacity="0.14"/>
  <circle cx="660" cy="85" r="14" fill="#FB923C" opacity="0.2"/>
  <circle cx="660" cy="85" r="5" fill="#FB923C" opacity="0.5" filter="url(#rp-glow)"/>
  <circle cx="750" cy="50" r="18" fill="#1E2D4A" opacity="0.12"/>
  <circle cx="750" cy="50" r="6" fill="#FB923C" opacity="0.18"/>
  <line x1="660" y1="85" x2="750" y2="50" stroke="#FB923C" stroke-width="0.5" opacity="0.15"/>
  <circle cx="740" cy="140" r="14" fill="#1E2D4A" opacity="0.1"/>
  <circle cx="740" cy="140" r="4" fill="#FB923C" opacity="0.15"/>
  <line x1="660" y1="85" x2="740" y2="140" stroke="#FB923C" stroke-width="0.5" opacity="0.12"/>
</svg>
```

---

*End of Skill Card SVGs*
