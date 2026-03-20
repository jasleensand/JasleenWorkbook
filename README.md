# JasleenWorkbook
<!DOCTYPE html>

<html lang="en"><head>
<meta charset="utf-8"/>
<meta content="width=device-width, initial-scale=1.0" name="viewport"/>
<title>The Artisanal Patisserie - Whimsical Illustration</title>
<script src="https://cdn.tailwindcss.com?plugins=forms,container-queries"></script>
<link href="https://fonts.googleapis.com/css2?family=Noto+Serif:ital,wght@0,400;0,700;1,400&amp;family=Plus+Jakarta+Sans:wght@400;500;600;700&amp;display=swap" rel="stylesheet"/>
<link href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:wght,FILL@100..700,0..1&amp;display=swap" rel="stylesheet"/>
<script id="tailwind-config">
      tailwind.config = {
        darkMode: "class",
        theme: {
          extend: {
            colors: {
              "secondary-container": "#bceddc",
              "on-primary-fixed-variant": "#704b4b",
              "on-surface": "#312e29",
              "on-background": "#312e29",
              "outline": "#8c857b",
              "primary-fixed": "#fecbcb",
              "tertiary": "#595a6b",
              "surface-container-low": "#f6f0e6",
              "outline-variant": "#b1ada5",
              "on-error": "#ffefec",
              "on-primary": "#ffefee",
              "on-tertiary": "#f3f1ff",
              "secondary-fixed-dim": "#afdecf",
              "secondary-fixed": "#bceddc",
              "on-tertiary-fixed": "#404251",
              "surface-bright": "#fcf6ed",
              "on-surface-variant": "#5e5b54",
              "primary": "#785252",
              "tertiary-fixed": "#e6e6fa",
              "on-tertiary-fixed-variant": "#5c5e6e",
              "background": "#FFD6A5",
              "tertiary-dim": "#4d4f5f",
              "primary-fixed-dim": "#efbdbd",
              "error-dim": "#b92902",
              "surface-variant": "#e2dcd1",
              "surface-dim": "#dad4c8",
              "inverse-on-surface": "#a19c95",
              "surface": "#FFD6A5",
              "on-secondary-container": "#2d5a4e",
              "surface-tint": "#785252",
              "tertiary-fixed-dim": "#d8d8ec",
              "inverse-surface": "#100e09",
              "surface-container-lowest": "#ffffff",
              "on-error-container": "#520c00",
              "inverse-primary": "#fecbcb",
              "tertiary-container": "#e6e6fa",
              "secondary": "#376457",
              "error-container": "#f95630",
              "on-secondary": "#ccfdec",
              "on-secondary-fixed": "#18473b",
              "primary-container": "#fecbcb",
              "primary-dim": "#6a4647",
              "error": "#b02500",
              "surface-container": "#ede7dd",
              "secondary-dim": "#2a584b",
              "surface-container-high": "#e8e2d7",
              "on-secondary-fixed-variant": "#376457",
              "on-tertiary-container": "#525464",
              "on-primary-container": "#654142",
              "surface-container-highest": "#e2dcd1",
              "on-primary-fixed": "#502f30"
            },
            fontFamily: {
              "headline": ["Noto Serif"],
              "body": ["Plus Jakarta Sans"],
              "label": ["Plus Jakarta Sans"]
            },
            borderRadius: {"DEFAULT": "1rem", "lg": "2rem", "xl": "3rem", "full": "9999px"},
          },
        },
      }
    </script>
<style>
        body { 
            font-family: 'Plus Jakarta Sans', sans-serif; 
            background-color: #FFD6A5; 
            background-image: radial-gradient(circle at center, #FFECB3 0%, #FFD6A5 100%);
        }
        
        .gingham-pattern {
            background-color: #ffffff;
            background-image: 
                linear-gradient(90deg, rgba(255, 173, 173, 0.4) 50%, transparent 50%),
                linear-gradient(rgba(255, 173, 173, 0.4) 50%, transparent 50%);
            background-size: 32px 32px;
            filter: contrast(0.9) brightness(1.05);
            position: relative;
        }

        .cloth-drape {
            position: absolute;
            top: 4%;
            left: -4%;
            right: -4%;
            bottom: 4%;
            z-index: 1;
            border-radius: 40px 45px 35px 50px;
            transform: rotate(-0.2deg);
            box-shadow: 0 12px 25px rgba(0,0,0,0.06);
        }

        .grain-texture::after {
            content: "";
            position: absolute;
            top: 0; left: 0; width: 100%; height: 100%;
            opacity: 0.12;
            pointer-events: none;
            background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 200 200' xmlns='http://www.w3.org/2000/svg'%3%3Cfilter id='noiseFilter'%3%3CfeTurbulence type='fractalNoise' baseFrequency='0.65' numOctaves='3' stitchTiles='stitch'/%3%3C/filter%3%3Crect width='100%25' height='100%25' filter='url(%23noiseFilter)'/%3%3C/svg%3E");
        }

        .macaron-pillowy {
            border-radius: 50%;
            transition: transform 0.3s cubic-bezier(0.175, 0.885, 0.32, 1.275), clip-path 0.2s ease;
            box-shadow: inset 0 -6px 12px rgba(0,0,0,0.08), 0 8px 15px rgba(0,0,0,0.04);
        }
        .macaron-pillowy[data-bite-level="1"] { clip-path: polygon(0 0, 100% 0, 100% 80%, 70% 85%, 62% 100%, 0 100%); }
        .macaron-pillowy[data-bite-level="2"] { clip-path: polygon(0 0, 100% 0, 100% 65%, 55% 70%, 47% 100%, 0 100%); }
        .macaron-pillowy[data-bite-level="3"] { clip-path: polygon(0 0, 100% 0, 100% 50%, 40% 55%, 34% 100%, 0 100%); }
        
        .macaron-btn:hover .macaron-pillowy {
            transform: scale(1.08) translateY(-4px);
        }

        .curved-text-svg {
            position: absolute;
            bottom: 5%;
            width: 90%;
            height: 40%;
            pointer-events: none;
        }

        .curved-text-svg text {
            font-family: 'Noto Serif', serif;
            font-weight: 700;
            text-transform: uppercase;
            letter-spacing: 0.05em;
            font-size: 10px;
        }

        .watercolor-tongs {
            position: absolute;
            bottom: 5%;
            width: 500px;
            height: 140px;
            z-index: 20;
            display: flex;
            align-items: center;
            justify-content: center;
            pointer-events: none;
            transform: rotate(-1deg);
        }

        .tongs-arm-long {
            position: absolute;
            height: 24px;
            width: 420px;
            border-radius: 999px;
            background: linear-gradient(90deg, #e5e7eb, #9ca3af);
            border: 2px solid #6b7280;
            box-shadow: 2px 2px 10px rgba(0,0,0,0.03);
        }

        .scalloped-head {
            position: absolute;
            width: 75px;
            height: 65px;
            background: #d1d5db;
            border: 2.5px solid #6b7280;
            border-radius: 40% 60% 60% 40% / 50% 50% 50% 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            box-shadow: inset 0 -4px 8px rgba(0,0,0,0.1);
            clip-path: polygon(0% 20%, 10% 5%, 20% 20%, 30% 5%, 40% 20%, 50% 5%, 60% 20%, 70% 5%, 80% 20%, 90% 5%, 100% 20%, 100% 100%, 0% 100%);
        }

        .tongs-dot-pattern {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 5px;
        }

        .tongs-dot {
            width: 5px;
            height: 5px;
            background: rgba(255,255,255,0.7);
            border-radius: 50%;
        }

        .rectangular-tray {
            width: 100%;
            max-width: 1000px;
            aspect-ratio: 21/10;
            background-color: #e5e7eb;
            border: 4px solid #9ca3af;
            border-radius: 40px;
            position: relative;
            box-shadow: 0 20px 50px rgba(0,0,0,0.08);
            display: flex;
            align-items: center;
            justify-content: center;
        }
    </style>
</head>
<body class="bg-surface min-h-screen flex flex-col items-center justify-center overflow-hidden grain-texture">
<main class="flex items-center justify-center w-full max-w-7xl px-8">
<div class="relative w-full flex items-center justify-center">
<!-- Soft Background Glow -->
<div class="absolute w-[120%] h-[120%] bg-white/30 blur-[100px] rounded-full pointer-events-none"></div>
<!-- The Rectangular Tray - Soft Grey -->
<div class="rectangular-tray">
<!-- Draping Gingham Cloth - Underneath macarons, drapes slightly off -->
<div class="cloth-drape gingham-pattern border-[2px] border-[#ffadad]/40"></div>
<!-- Macaron Row Container -->
<div class="relative z-10 flex flex-row items-center justify-center gap-8 md:gap-16 lg:gap-24 px-4 w-full -mt-4">
<!-- Macaron 1: Pink (Interactivities) -->
<button class="macaron-btn group relative flex flex-col items-center" data-target="/interactivities.html" data-bites="3">
<div class="macaron-pillowy w-24 h-24 md:w-32 md:h-32 lg:w-40 lg:h-40 bg-[#fff1f2] relative flex items-center justify-center border-b-[10px] border-[#f4c2c2] border-[2px] border-[#e5a4a4]" data-bite-level="0">
<div class="absolute inset-x-0 top-1/2 -translate-y-1/2 h-3 bg-white/50 blur-[1px]"></div>
<svg class="curved-text-svg" viewbox="0 0 100 40">
<path d="M 10,10 C 25,35 75,35 90,10" fill="transparent" id="curve-1"></path>
<text fill="#704b4b">
<textpath startoffset="50%" text-anchor="middle" xlink:href="#curve-1">Interactivities</textpath>
</text>
</svg>
</div>
</button>
<!-- Macaron 2: Mint (Experiments) -->
<button class="macaron-btn group relative flex flex-col items-center" data-target="/experiments.html" data-bites="3">
<div class="macaron-pillowy w-24 h-24 md:w-32 md:h-32 lg:w-40 lg:h-40 bg-[#f0fdf4] relative flex items-center justify-center border-b-[10px] border-[#bceddc] border-[2px] border-[#7cbfa9]" data-bite-level="0">
<div class="absolute inset-x-0 top-1/2 -translate-y-1/2 h-3 bg-white/50 blur-[1px]"></div>
<svg class="curved-text-svg" viewbox="0 0 100 40">
<path d="M 10,10 C 25,35 75,35 90,10" fill="transparent" id="curve-2"></path>
<text fill="#18473b">
<textpath startoffset="50%" text-anchor="middle" xlink:href="#curve-2">Experiments</textpath>
</text>
</svg>
</div>
</button>
<!-- Macaron 3: Lemon (Case Studies) -->
<button class="macaron-btn group relative flex flex-col items-center" data-target="/case-studies.html" data-bites="3">
<div class="macaron-pillowy w-24 h-24 md:w-32 md:h-32 lg:w-40 lg:h-40 bg-[#fffbeb] relative flex items-center justify-center border-b-[10px] border-[#fde68a] border-[2px] border-[#d9bf4c]" data-bite-level="0">
<div class="absolute inset-x-0 top-1/2 -translate-y-1/2 h-3 bg-white/50 blur-[1px]"></div>
<svg class="curved-text-svg" viewbox="0 0 100 40">
<path d="M 10,10 C 25,35 75,35 90,10" fill="transparent" id="curve-3"></path>
<text fill="#857000">
<textpath startoffset="50%" text-anchor="middle" xlink:href="#curve-3">Case Studies</textpath>
</text>
</svg>
</div>
</button>
<!-- Macaron 4: Lavender (Glossary) -->
<button class="macaron-btn group relative flex flex-col items-center" data-target="/glossary.html" data-bites="3">
<div class="macaron-pillowy w-24 h-24 md:w-32 md:h-32 lg:w-40 lg:h-40 bg-[#f5f3ff] relative flex items-center justify-center border-b-[10px] border-[#d8d8ec] border-[2px] border-[#9b9bc4]" data-bite-level="0">
<div class="absolute inset-x-0 top-1/2 -translate-y-1/2 h-3 bg-white/50 blur-[1px]"></div>
<svg class="curved-text-svg" viewbox="0 0 100 40">
<path d="M 10,10 C 25,35 75,35 90,10" fill="transparent" id="curve-4"></path>
<text fill="#525464">
<textpath startoffset="50%" text-anchor="middle" xlink:href="#curve-4">Glossary</textpath>
</text>
</svg>
</div>
</button>
</div>
</main>
<script>
  let audioCtx;
  function playMunchSound() {
    if (!audioCtx) {
      audioCtx = new (window.AudioContext || window.webkitAudioContext)();
    }
    if (audioCtx.state === 'suspended') {
      audioCtx.resume();
    }

    const now = audioCtx.currentTime;
    const mainGain = audioCtx.createGain();
    mainGain.gain.setValueAtTime(0.1, now);
    mainGain.connect(audioCtx.destination);

    const noiseBuf = audioCtx.createBuffer(1, audioCtx.sampleRate * 0.14, audioCtx.sampleRate);
    const noiseData = noiseBuf.getChannelData(0);
    for (let i = 0; i < noiseData.length; i++) {
      noiseData[i] = (Math.random() * 2 - 1) * (1 - i / noiseData.length);
    }
    const noise = audioCtx.createBufferSource();
    noise.buffer = noiseBuf;

    const noiseFilter = audioCtx.createBiquadFilter();
    noiseFilter.type = 'bandpass';
    noiseFilter.frequency.setValueAtTime(1900, now);
    noiseFilter.Q.setValueAtTime(1.4, now);

    const crunchOsc = audioCtx.createOscillator();
    crunchOsc.type = 'square';
    crunchOsc.frequency.setValueAtTime(180, now);
    crunchOsc.frequency.exponentialRampToValueAtTime(70, now + 0.12);

    const crunchGain = audioCtx.createGain();
    crunchGain.gain.setValueAtTime(0.06, now);
    crunchGain.gain.exponentialRampToValueAtTime(0.001, now + 0.16);

    noise.connect(noiseFilter);
    noiseFilter.connect(mainGain);
    crunchOsc.connect(crunchGain);
    crunchGain.connect(mainGain);

    mainGain.gain.exponentialRampToValueAtTime(0.001, now + 0.16);

    noise.start(now);
    noise.stop(now + 0.16);
    crunchOsc.start(now);
    crunchOsc.stop(now + 0.16);
  }

  function initializeMacarons() {
    document.querySelectorAll('.macaron-btn').forEach(button => {
      button.dataset.bites = '3';
      const macaron = button.querySelector('.macaron-pillowy');
      if (macaron) macaron.dataset.biteLevel = '0';
    });
  }

  initializeMacarons();

  document.querySelectorAll('.macaron-btn').forEach(button => {
    button.addEventListener('click', (event) => {
      event.preventDefault();
      playMunchSound();

      const macaron = button.querySelector('.macaron-pillowy');
      let remaining = parseInt(button.dataset.bites || '3', 10);
      remaining = Math.max(0, remaining - 1);
      button.dataset.bites = remaining;

      if (macaron) {
        const level = 4 - remaining;
        macaron.dataset.biteLevel = Math.min(level, 3).toString();
      }

      if (remaining <= 0) {
        const target = button.dataset.target || '#';
        setTimeout(() => {
          window.location.href = target;
        }, 120);
      }
    });
  });
</script>
</body></html>
