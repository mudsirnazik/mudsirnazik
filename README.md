<svg width="1200" height="260" viewBox="0 0 1200 260" xmlns="http://www.w3.org/2000/svg">

<defs>

  <linearGradient id="bg" x1="0" y1="0" x2="1" y2="1">
    <stop offset="0%" stop-color="#020617"/>
    <stop offset="50%" stop-color="#071e2d"/>
    <stop offset="100%" stop-color="#020617"/>
  </linearGradient>

  <filter id="glow">
    <feGaussianBlur stdDeviation="4" result="blur"/>
    <feMerge>
      <feMergeNode in="blur"/>
      <feMergeNode in="SourceGraphic"/>
    </feMerge>
  </filter>

  <style>
    .icon {
      font-family: Arial, sans-serif;
      font-size: 32px;
      font-weight: bold;
      fill: #22d3ee;
    }

    .small {
      font-family: Arial, sans-serif;
      font-size: 24px;
      font-weight: bold;
      fill: #67e8f9;
    }

    .line {
      stroke: #0e7490;
      stroke-width: 1;
      opacity: .35;
    }

    .float1 {
      animation: move1 7s ease-in-out infinite;
    }

    .float2 {
      animation: move2 9s ease-in-out infinite;
    }

    .float3 {
      animation: move3 6s ease-in-out infinite;
    }

    @keyframes move1 {
      0%,100% { transform: translateY(0); }
      50% { transform: translateY(-18px); }
    }

    @keyframes move2 {
      0%,100% { transform: translateY(0); }
      50% { transform: translateY(15px); }
    }

    @keyframes move3 {
      0%,100% { transform: translate(0,0); }
      50% { transform: translate(10px,-12px); }
    }
  </style>

</defs>

<!-- Background -->

<rect width="1200" height="260" rx="18" fill="url(#bg)"/>

<!-- Network lines -->

<path class="line" d="M80 80 L260 170 L430 70 L600 170 L790 80 L970 175 L1120 70"/>
<path class="line" d="M120 200 L310 90 L500 205 L700 90 L900 200 L1080 100"/>

<!-- Floating icons -->

<g class="float1" filter="url(#glow)">
  <text x="70" y="75" class="icon">☁</text>
  <text x="45" y="105" class="small">AWS</text>
</g>

<g class="float2" filter="url(#glow)">
  <text x="245" y="175" class="icon">🐳</text>
  <text x="240" y="205" class="small">Docker</text>
</g>

<g class="float3" filter="url(#glow)">
  <text x="410" y="65" class="icon">☸</text>
  <text x="395" y="98" class="small">K8s</text>
</g>

<g class="float1" filter="url(#glow)">
  <text x="580" y="175" class="icon">⚙</text>
  <text x="565" y="208" class="small">CI/CD</text>
</g>

<g class="float2" filter="url(#glow)">
  <text x="765" y="80" class="icon">🏗</text>
  <text x="750" y="112" class="small">Terraform</text>
</g>

<g class="float3" filter="url(#glow)">
  <text x="950" y="175" class="icon">🐧</text>
  <text x="950" y="208" class="small">Linux</text>
</g>

<g class="float1" filter="url(#glow)">
  <text x="1090" y="75" class="icon">🔐</text>
  <text x="1070" y="108" class="small">DevSecOps</text>
</g>

<!-- Central title -->

<text x="600" y="135"
   text-anchor="middle"
   font-family="Arial"
   font-size="25"
   font-weight="bold"
   fill="#ffffff">
AUTOMATE • DEPLOY • SCALE • SECURE </text>

<text x="600" y="160"
   text-anchor="middle"
   font-family="Arial"
   font-size="13"
   fill="#94a3b8">
DevOps • Cloud • Kubernetes • Infrastructure as Code • Automation </text>

</svg>
