<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

</head>
<body>
    <svg xmlns="http://www.w3.org/2000/svg" width="1180" height="610" viewBox="0 0 1180 610" role="img" aria-label="Neshik premium GitHub profile banner">
<defs>

  <!-- Animated Accent Gradient -->
  <linearGradient id="accent" x1="0%" y1="0%" x2="100%" y2="100%">
    <stop offset="0%" stop-color="#7C3AED">
      <animate
        attributeName="stop-color"
        values="#7C3AED;#22D3EE;#10B981;#7C3AED"
        dur="9s"
        repeatCount="indefinite"/>
    </stop>

    <stop offset="55%" stop-color="#22D3EE">
      <animate
        attributeName="stop-color"
        values="#22D3EE;#10B981;#7C3AED;#22D3EE"
        dur="9s"
        repeatCount="indefinite"/>
    </stop>

    <stop offset="100%" stop-color="#10B981">
      <animate
        attributeName="stop-color"
        values="#10B981;#7C3AED;#22D3EE;#10B981"
        dur="9s"
        repeatCount="indefinite"/>
    </stop>
  </linearGradient>

  <!-- Background Orbs -->
  <radialGradient id="orb1">
    <stop offset="0%" stop-color="#22D3EE" stop-opacity=".20"/>
    <stop offset="100%" stop-color="#22D3EE" stop-opacity="0"/>
  </radialGradient>

  <radialGradient id="orb2">
    <stop offset="0%" stop-color="#7C3AED" stop-opacity=".18"/>
    <stop offset="100%" stop-color="#7C3AED" stop-opacity="0"/>
  </radialGradient>

  <!-- Glow -->
  <filter id="glow">
    <feGaussianBlur stdDeviation="5" result="blur"/>
    <feMerge>
      <feMergeNode in="blur"/>
      <feMergeNode in="SourceGraphic"/>
    </feMerge>
  </filter>

  <!-- Soft Background Glow -->
  <filter id="soft">
    <feGaussianBlur stdDeviation="18"/>
  </filter>

  <!-- Rounded Canvas -->
  <clipPath id="round">
    <rect
      x="0"
      y="0"
      width="1180"
      height="610"
      rx="30"/>
  </clipPath>

  <!-- Noise Texture -->
  <pattern
    id="noise"
    width="80"
    height="80"
    patternUnits="userSpaceOnUse">

    <circle
      cx="7"
      cy="12"
      r=".7"
      fill="#F8FAFC"
      opacity=".06"/>

    <circle
      cx="51"
      cy="39"
      r=".6"
      fill="#F8FAFC"
      opacity=".05"/>

    <circle
      cx="29"
      cy="68"
      r=".5"
      fill="#F8FAFC"
      opacity=".05"/>
  </pattern>

  <!-- Scanline -->
  <pattern
    id="scan"
    width="8"
    height="8"
    patternUnits="userSpaceOnUse">

    <rect
      width="8"
      height="1"
      fill="#22D3EE"
      opacity=".035"/>
  </pattern>

</defs>


<!-- ========================================================= -->
<!-- MAIN CANVAS -->
<!-- ========================================================= -->

<g clip-path="url(#round)">

  <!-- Background -->
  <rect
    width="1180"
    height="610"
    fill="#030712"/>


  <!-- ======================================================= -->
  <!-- BACKGROUND GLOW 1 -->
  <!-- ======================================================= -->

  <circle
    cx="180"
    cy="90"
    r="280"
    fill="url(#orb2)"
    filter="url(#soft)">

    <animateTransform
      attributeName="transform"
      type="translate"
      values="0 0;55 30;0 0"
      dur="12s"
      repeatCount="indefinite"/>
  </circle>


  <!-- ======================================================= -->
  <!-- BACKGROUND GLOW 2 -->
  <!-- ======================================================= -->

  <circle
    cx="1010"
    cy="500"
    r="300"
    fill="url(#orb1)"
    filter="url(#soft)">

    <animateTransform
      attributeName="transform"
      type="translate"
      values="0 0;-45 -35;0 0"
      dur="14s"
      repeatCount="indefinite"/>
  </circle>


  <!-- ======================================================= -->
  <!-- GLASS CONTAINER -->
  <!-- ======================================================= -->

  <rect
    x="24"
    y="24"
    width="1132"
    height="562"
    rx="24"
    fill="#0F172A"
    fill-opacity=".72"
    stroke="#F8FAFC"
    stroke-opacity=".08"/>


  <!-- Noise -->
  <rect
    x="24"
    y="24"
    width="1132"
    height="562"
    rx="24"
    fill="url(#noise)"/>


  <!-- ======================================================= -->
  <!-- BORDER SHIMMER -->
  <!-- ======================================================= -->

  <rect
    x="24"
    y="24"
    width="1132"
    height="562"
    rx="24"
    fill="none"
    stroke="url(#accent)"
    stroke-width="1.2"
    stroke-dasharray="18 240">

    <animate
      attributeName="stroke-dashoffset"
      from="0"
      to="-516"
      dur="7s"
      repeatCount="indefinite"/>
  </rect>


  <!-- ======================================================= -->
  <!-- LEFT SIDE -->
  <!-- ======================================================= -->

  <g transform="translate(65 95)">

    <!-- System Label -->

    <text
      x="0"
      y="0"
      font-family="monospace"
      font-size="12"
      fill="#94A3B8"
      letter-spacing="3">

      NESHIK / SYSTEM ONLINE

    </text>


    <!-- ===================================================== -->
    <!-- ASCII PORTRAIT -->
    <!-- ===================================================== -->

    <g
      font-family="monospace"
      font-size="13"
      font-weight="700"
      fill="url(#accent)"
      filter="url(#glow)">

      <!-- Line 1 -->

      <text
        x="0"
        y="62"
        opacity="0">

        ████████

        <animate
          attributeName="opacity"
          values="0;1"
          begin=".2s"
          dur=".45s"
          fill="freeze"/>

      </text>


      <!-- Line 2 -->

      <text
        x="0"
        y="77"
        opacity="0">

        ██████████████

        <animate
          attributeName="opacity"
          values="0;1"
          begin=".45s"
          dur=".45s"
          fill="freeze"/>

      </text>


      <!-- Line 3 -->

      <text
        x="0"
        y="92"
        opacity="0">

        ████  ◉    ◉  ████

        <animate
          attributeName="opacity"
          values="0;1"
          begin=".7s"
          dur=".45s"
          fill="freeze"/>

      </text>


      <!-- Line 4 -->

      <text
        x="0"
        y="107"
        opacity="0">

        █████    ▽    █████

        <animate
          attributeName="opacity"
          values="0;1"
          begin=".95s"
          dur=".45s"
          fill="freeze"/>

      </text>


      <!-- Line 5 -->

      <text
        x="0"
        y="122"
        opacity="0">

        ████████████████████

        <animate
          attributeName="opacity"
          values="0;1"
          begin="1.2s"
          dur=".45s"
          fill="freeze"/>

      </text>


      <!-- Line 6 -->

      <text
        x="0"
        y="137"
        opacity="0">

        ███  ████████  ███

        <animate
          attributeName="opacity"
          values="0;1"
          begin="1.45s"
          dur=".45s"
          fill="freeze"/>

      </text>


      <!-- Line 7 -->

      <text
        x="0"
        y="152"
        opacity="0">

        ████  ██  ████

        <animate
          attributeName="opacity"
          values="0;1"
          begin="1.7s"
          dur=".45s"
          fill="freeze"/>

      </text>


      <!-- Line 8 -->

      <text
        x="0"
        y="167"
        opacity="0">

        ████████

        <animate
          attributeName="opacity"
          values="0;1"
          begin="1.95s"
          dur=".45s"
          fill="freeze"/>

      </text>

    </g>


    <!-- ===================================================== -->
    <!-- SCANLINE -->
    <!-- ===================================================== -->

    <g opacity=".28">

      <rect
        x="-15"
        y="35"
        width="310"
        height="2"
        fill="#22D3EE">

        <animateTransform
          attributeName="transform"
          type="translate"
          values="0 0;0 145;0 0"
          dur="4s"
          repeatCount="indefinite"/>

      </rect>

    </g>


    <!-- Terminal Prompt -->

    <text
      x="0"
      y="225"
      font-family="monospace"
      font-size="12"
      fill="#94A3B8">

      $ whoami

    </text>


    <!-- Name -->

    <text
      x="0"
      y="250"
      font-family="monospace"
      font-size="24"
      font-weight="700"
      fill="#F8FAFC">

      neshik

      <tspan fill="#22D3EE">_</tspan>

    </text>


    <!-- Description -->

    <text
      x="0"
      y="285"
      font-family="sans-serif"
      font-size="13"
      fill="#94A3B8">

      BUILDING DIGITAL WORLDS

    </text>


    <text
      x="0"
      y="310"
      font-family="sans-serif"
      font-size="13"
      fill="#94A3B8">

      AI · WEB · UI/UX · SPACE

    </text>

  </g>


  <!-- ======================================================= -->
  <!-- RIGHT TERMINAL -->
  <!-- ======================================================= -->

  <g transform="translate(405 65)">

    <!-- Terminal Window -->

    <rect
      width="700"
      height="480"
      rx="22"
      fill="#030712"
      fill-opacity=".78"
      stroke="#F8FAFC"
      stroke-opacity=".09"/>


    <!-- Terminal Header -->

    <rect
      width="700"
      height="58"
      rx="22"
      fill="#0F172A"
      fill-opacity=".92"/>


    <rect
      y="35"
      width="700"
      height="23"
      fill="#0F172A"
      fill-opacity=".92"/>


    <!-- Window Controls -->

    <circle
      cx="28"
      cy="29"
      r="6"
      fill="#7C3AED"/>

    <circle
      cx="49"
      cy="29"
      r="6"
      fill="#22D3EE"/>

    <circle
      cx="70"
      cy="29"
      r="6"
      fill="#10B981"/>


    <!-- Terminal Title -->

    <text
      x="105"
      y="34"
      font-family="monospace"
      font-size="12"
      fill="#94A3B8">

      neshik@github: ~/profile

    </text>


    <!-- ===================================================== -->
    <!-- GREETING -->
    <!-- ===================================================== -->

    <text
      x="36"
      y="102"
      font-family="sans-serif"
      font-size="15"
      fill="#94A3B8">

      Hi 👋

    </text>


    <!-- Main Name -->

    <text
      x="36"
      y="143"
      font-family="sans-serif"
      font-size="37"
      font-weight="800"
      fill="#F8FAFC">

      I'm Neshik

    </text>


    <!-- ===================================================== -->
    <!-- TYPING ROLE 1 -->
    <!-- ===================================================== -->

    <text
      x="36"
      y="178"
      font-family="monospace"
      font-size="16"
      fill="#22D3EE">

      <tspan>Software Developer</tspan>

      <animate
        attributeName="opacity"
        values="1;1;0;0;1"
        dur="8s"
        repeatCount="indefinite"/>

    </text>


    <!-- ===================================================== -->
    <!-- TYPING ROLE 2 -->
    <!-- ===================================================== -->

    <text
      x="36"
      y="178"
      font-family="monospace"
      font-size="16"
      fill="#7C3AED"
      opacity="0">

      <tspan>AI &amp; Web Developer</tspan>

      <animate
        attributeName="opacity"
        values="0;0;1;1;0"
        dur="8s"
        repeatCount="indefinite"/>

    </text>


    <!-- Blinking Cursor -->

    <rect
      x="255"
      y="163"
      width="2"
      height="20"
      fill="#22D3EE">

      <animate
        attributeName="opacity"
        values="1;0;1"
        dur="1s"
        repeatCount="indefinite"/>

    </rect>


    <!-- ===================================================== -->
    <!-- PROFILE DETAILS -->
    <!-- ===================================================== -->

    <g
      font-family="monospace"
      font-size="12">

      <!-- Location -->

      <text
        x="36"
        y="222"
        fill="#94A3B8"
        opacity="0">

        📍 Salem, India

        <animate
          attributeName="opacity"
          values="0;1"
          begin="2.2s"
          dur=".5s"
          fill="freeze"/>

      </text>


      <!-- Education -->

      <text
        x="36"
        y="247"
        fill="#94A3B8"
        opacity="0">

        🎓 BCA Student

        <animate
          attributeName="opacity"
          values="0;1"
          begin="2.5s"
          dur=".5s"
          fill="freeze"/>

      </text>


      <!-- Focus -->

      <text
        x="36"
        y="272"
        fill="#94A3B8"
        opacity="0">

        🚀 Building AI + Web Projects

        <animate
          attributeName="opacity"
          values="0;1"
          begin="2.8s"
          dur=".5s"
          fill="freeze"/>

      </text>


      <!-- Interests -->

      <text
        x="36"
        y="297"
        fill="#94A3B8"
        opacity="0">

        🌌 Exploring Space &amp; Creative Technology

        <animate
          attributeName="opacity"
          values="0;1"
          begin="3.1s"
          dur=".5s"
          fill="freeze"/>

      </text>

    </g>


    <!-- ===================================================== -->
    <!-- SKILLS -->
    <!-- ===================================================== -->

    <text
      x="36"
      y="335"
      font-family="sans-serif"
      font-size="12"
      font-weight="700"
      fill="#F8FAFC">

      SKILLS

    </text>


    <g
      font-family="sans-serif"
      font-size="11"
      fill="#F8FAFC">


      <!-- JavaScript -->

      <g transform="translate(36 350)">

        <rect
          width="82"
          height="28"
          rx="14"
          fill="#7C3AED"
          fill-opacity=".16"
          stroke="#7C3AED"
          stroke-opacity=".35"/>

        <text
          x="41"
          y="18"
          text-anchor="middle">

          JavaScript

        </text>

        <animateTransform
          attributeName="transform"
          type="scale"
          values="1;1.03;1"
          dur="3s"
          repeatCount="indefinite"/>

      </g>


      <!-- Python -->

      <g transform="translate(128 350)">

        <rect
          width="72"
          height="28"
          rx="14"
          fill="#22D3EE"
          fill-opacity=".16"
          stroke="#22D3EE"
          stroke-opacity=".35"/>

        <text
          x="36"
          y="18"
          text-anchor="middle">

          Python

        </text>

      </g>


      <!-- React -->

      <g transform="translate(210 350)">

        <rect
          width="72"
          height="28"
          rx="14"
          fill="#10B981"
          fill-opacity=".16"
          stroke="#10B981"
          stroke-opacity=".35"/>

        <text
          x="36"
          y="18"
          text-anchor="middle">

          React

        </text>

      </g>


      <!-- Generative AI -->

      <g transform="translate(292 350)">

        <rect
          width="92"
          height="28"
          rx="14"
          fill="#7C3AED"
          fill-opacity=".16"
          stroke="#7C3AED"
          stroke-opacity=".35"/>

        <text
          x="46"
          y="18"
          text-anchor="middle">

          Generative AI

        </text>

      </g>


      <!-- UI UX -->

      <g transform="translate(394 350)">

        <rect
          width="76"
          height="28"
          rx="14"
          fill="#22D3EE"
          fill-opacity=".16"
          stroke="#22D3EE"
          stroke-opacity=".35"/>

        <text
          x="38"
          y="18"
          text-anchor="middle">

          UI / UX

        </text>

      </g>

    </g>


    <!-- ===================================================== -->
    <!-- SOCIAL LINKS -->
    <!-- ===================================================== -->

    <g
      transform="translate(36 414)"
      fill="#94A3B8"
      font-family="sans-serif"
      font-size="12">

      <text x="0" y="0">
        ⌘ GitHub
      </text>

      <text x="105" y="0">
        in LinkedIn
      </text>

      <text x="225" y="0">
        ◎ Portfolio
      </text>

      <text x="340" y="0">
        ✉ Email
      </text>

    </g>


    <!-- Terminal Footer -->

    <text
      x="36"
      y="452"
      font-family="monospace"
      font-size="11"
      fill="#94A3B8">

      $ learn → build → improve → repeat ♾

    </text>

  </g>


  <!-- ======================================================= -->
  <!-- FLOATING PARTICLES -->
  <!-- ======================================================= -->

  <g fill="#22D3EE">

    <circle
      cx="360"
      cy="80"
      r="2">

      <animate
        attributeName="cy"
        values="80;55;80"
        dur="4s"
        repeatCount="indefinite"/>

    </circle>


    <circle
      cx="1140"
      cy="150"
      r="1.5">

      <animate
        attributeName="cy"
        values="150;125;150"
        dur="3.5s"
        repeatCount="indefinite"/>

    </circle>


    <circle
      cx="375"
      cy="535"
      r="1.5">

      <animate
        attributeName="cy"
        values="535;510;535"
        dur="5s"
        repeatCount="indefinite"/>

    </circle>

  </g>


  <!-- ======================================================= -->
  <!-- MOVING SCANLINE -->
  <!-- ======================================================= -->

  <rect
    x="24"
    y="24"
    width="1132"
    height="562"
    rx="24"
    fill="url(#scan)">

    <animateTransform
      attributeName="transform"
      type="translate"
      values="0 -610;0 610"
      dur="7s"
      repeatCount="indefinite"/>

  </rect>

</g>

</svg>
</body>
</html>
