<!DOCTYPE html>

<html class="dark" lang="es"><head>
<meta charset="utf-8"/>
<meta content="width=device-width, initial-scale=1.0" name="viewport"/>
<title>MAGENTA | Sublimación Digital y Confección</title>
<script src="https://cdn.tailwindcss.com?plugins=forms,container-queries"></script>
<link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;600;700;800&amp;family=Inter:wght@400;600&amp;display=swap" rel="stylesheet"/>
<link href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:wght,FILL@100..700,0..1&amp;display=swap" rel="stylesheet"/>
<style>
        .material-symbols-outlined {
            font-variation-settings: 'FILL' 0, 'wght' 400, 'GRAD' 0, 'opsz' 24;
        }
        .glass-card {
            background: rgba(255, 255, 255, 0.03);
            backdrop-filter: blur(20px);
            border: 1px solid rgba(171, 199, 255, 0.2);
        }
        .neon-glow-fuchsia {
            box-shadow: 0 0 30px rgba(255, 0, 255, 0.3);
        }
        ::-webkit-scrollbar {
            width: 8px;
        }
        ::-webkit-scrollbar-track {
            background: #131313;
        }
        ::-webkit-scrollbar-thumb {
            background: linear-gradient(to bottom, #ff00ff, #abc7ff);
            border-radius: 4px;
        }

        @keyframes flow {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }
        .animate-flow {
            background: linear-gradient(-45deg, rgba(20, 20, 20, 1), rgba(40, 0, 40, 0.5), rgba(0, 20, 40, 0.5), rgba(20, 20, 20, 1));
            background-size: 400% 400%;
            animation: flow 15s ease infinite;
        }

        .carousel-track {
            display: flex;
            transition: transform 0.7s cubic-bezier(0.4, 0, 0.2, 1);
        }
        .carousel-item {
            min-width: 100%;
        }

        @keyframes pulse-whatsapp {
            0% { box-shadow: 0 0 0 0 rgba(37, 211, 102, 0.6); }
            70% { box-shadow: 0 0 0 15px rgba(37, 211, 102, 0); }
            100% { box-shadow: 0 0 0 0 rgba(37, 211, 102, 0); }
        }
        .animate-pulse-whatsapp {
            animation: pulse-whatsapp 2s infinite;
        }
    </style>
<script id="tailwind-config">
        tailwind.config = {
            darkMode: "class",
            theme: {
                extend: {
                    "colors": {
                        "secondary-fixed-dim": "#abc7ff",
                        "secondary-container": "#2c4979",
                        "on-secondary": "#0e305e",
                        "primary-fixed-dim": "#ffabf3",
                        "on-background": "#e5e2e1",
                        "primary-fixed": "#ffd7f5",
                        "on-secondary-fixed-variant": "#294676",
                        "on-surface": "#e5e2e1",
                        "on-error": "#690005",
                        "on-tertiary-fixed": "#1a1e00",
                        "surface-tint": "#ffabf3",
                        "on-secondary-container": "#9db9f0",
                        "on-primary-container": "#7d3878",
                        "inverse-on-surface": "#313030",
                        "on-primary-fixed": "#380038",
                        "on-primary": "#551353",
                        "deep-black": "#000000",
                        "glass-border": "rgba(171, 199, 255, 0.2)",
                        "surface-container-highest": "#353534",
                        "surface-dim": "#131313",
                        "surface-container": "#201f1f",
                        "outline-variant": "#50434c",
                        "on-tertiary": "#2e3400",
                        "outline": "#9c8c97",
                        "surface-variant": "#353534",
                        "primary": "#ffd7f5",
                        "tertiary": "#dbed5d",
                        "on-tertiary-container": "#4e5700",
                        "primary-container": "#ffabf3",
                        "surface-container-high": "#2a2a2a",
                        "on-secondary-fixed": "#001b3f",
                        "tertiary-container": "#bfd043",
                        "surface": "#131313",
                        "surface-bright": "#393939",
                        "error-container": "#93000a",
                        "inverse-surface": "#e5e2e1",
                        "on-surface-variant": "#d3c2cd",
                        "tertiary-fixed": "#dbed5d",
                        "error": "#ffb4ab",
                        "background": "#131313",
                        "inverse-primary": "#8a4484",
                        "surface-container-lowest": "#0e0e0e",
                        "on-primary-fixed-variant": "#6f2c6b",
                        "surface-container-low": "#1c1b1b",
                        "neon-fuchsia": "#ff00ff",
                        "on-tertiary-fixed-variant": "#434b00",
                        "fuchsia-glow": "rgba(255, 0, 255, 0.3)",
                        "tertiary-fixed-dim": "#bfd043",
                        "on-error-container": "#ffdad6",
                        "secondary": "#abc7ff",
                        "secondary-fixed": "#d7e2ff"
                    },
                    "borderRadius": {
                        "DEFAULT": "0.25rem",
                        "lg": "0.5rem",
                        "xl": "0.75rem",
                        "full": "9999px"
                    },
                    "spacing": {
                        "gutter-mobile": "12px",
                        "margin-mobile": "20px",
                        "xs": "8px",
                        "xl": "64px",
                        "md": "24px",
                        "sm": "16px",
                        "lg": "40px",
                        "base": "4px"
                    },
                    "fontFamily": {
                        "headline-md": ["Montserrat"],
                        "label-md": ["Inter"],
                        "headline-lg": ["Montserrat"],
                        "headline-lg-mobile": ["Montserrat"],
                        "body-md": ["Inter"],
                        "body-lg": ["Inter"],
                        "display-lg": ["Montserrat"]
                    },
                    "fontSize": {
                        "headline-md": ["24px", {"lineHeight": "32px", "fontWeight": "600"}],
                        "label-md": ["14px", {"lineHeight": "20px", "letterSpacing": "0.05em", "fontWeight": "600"}],
                        "headline-lg": ["32px", {"lineHeight": "40px", "letterSpacing": "-0.01em", "fontWeight": "700"}],
                        "headline-lg-mobile": ["28px", {"lineHeight": "34px", "fontWeight": "700"}],
                        "body-md": ["16px", {"lineHeight": "24px", "fontWeight": "400"}],
                        "body-lg": ["18px", {"lineHeight": "28px", "fontWeight": "400"}],
                        "display-lg": ["48px", {"lineHeight": "52px", "letterSpacing": "-0.02em", "fontWeight": "800"}]
                    }
                },
            },
        }
    </script>
</head>
<body class="bg-background text-on-background font-body-md selection:bg-neon-fuchsia selection:text-white animate-flow">
<header class="fixed top-0 w-full z-50 bg-surface/80 backdrop-blur-xl border-b border-glass-border shadow-[0_4px_30px_rgba(255,0,255,0.1)]">
<div class="flex justify-between items-center px-margin-mobile md:px-xl h-16 w-full">
<div class="flex items-center gap-4">
<span class="material-symbols-outlined text-primary cursor-pointer hover:text-neon-fuchsia transition-colors duration-300">menu</span>
<span class="font-display-lg text-[24px] md:text-headline-lg text-neon-fuchsia tracking-widest uppercase font-extrabold filter drop-shadow-[0_0_8px_rgba(255,0,255,0.5)]">MAGENTA</span>
</div>
<div class="hidden md:flex gap-8 items-center">
<a class="font-label-md text-label-md text-on-surface-variant hover:text-neon-fuchsia transition-colors duration-300" href="#cotton">CATÁLOGO</a>
<a class="font-label-md text-label-md text-on-surface-variant hover:text-neon-fuchsia transition-colors duration-300" href="#sports">DEPORTES</a>
<a class="font-label-md text-label-md text-on-surface-variant hover:text-neon-fuchsia transition-colors duration-300" href="#tech">TECNOLOGÍA</a>
<a class="font-label-md text-label-md text-on-surface-variant hover:text-neon-fuchsia transition-colors duration-300" href="#services">SERVICIOS</a>
</div>
<div class="flex items-center gap-4">
<span class="material-symbols-outlined text-primary cursor-pointer hover:text-neon-fuchsia transition-colors duration-300">shopping_bag</span>
</div>
</div>
</header>
<!-- Floating WhatsApp -->
<a class="fixed bottom-24 right-6 md:bottom-10 md:right-10 z-[60] w-14 h-14 bg-[#25D366] rounded-full flex items-center justify-center text-white shadow-lg animate-pulse-whatsapp hover:scale-110 transition-transform" href="https://wa.me/51937190991" target="_blank">
<svg class="w-8 h-8 fill-current" viewbox="0 0 24 24">
<path d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347m-5.421 7.403h-.004a9.87 9.87 0 01-5.031-1.378l-.361-.214-3.741.982.998-3.648-.235-.374a9.86 9.86 0 01-1.51-5.26c.001-5.45 4.436-9.884 9.888-9.884 2.64 0 5.122 1.03 6.988 2.898a9.825 9.825 0 012.893 6.994c-.003 5.45-4.437 9.884-9.885 9.884m8.413-18.297A11.815 11.815 0 0012.05 0C5.495 0 .16 5.335.157 11.892c0 2.096.547 4.142 1.588 5.945L.057 24l6.305-1.654a11.882 11.882 0 005.683 1.448h.005c6.554 0 11.89-5.335 11.893-11.893a11.821 11.821 0 00-3.48-8.413z"></path>
</svg>
</a>
<main class="pt-16 pb-24 md:pb-0">
<!-- Hero -->
<section class="relative min-h-[90vh] flex flex-col items-center justify-center overflow-hidden px-margin-mobile">
<div class="relative z-10 text-center max-w-4xl">
<div class="mb-8 transform transition-transform duration-700">
<img alt="MAGENTA Logo" class="mx-auto w-48 md:w-64 filter drop-shadow-[0_0_20px_rgba(255,0,255,0.4)]" src="https://lh3.googleusercontent.com/aida-public/AB6AXuBui5EROSmYosxyKK3BE0QCowSkc_AqAZzvC2Rf96DmbPtnAa15Ho-sfmJgFAmudTxaGzhVp4EGrTy3pB3MzDeLniJvf6zDnQwBS8V2SZxe-zNbFkmnA7qYnv6Npn6cYkdSW2gfagqYcycezjLrdmk2YfCCAnkBS5tx8IGNB-1HziJ-6ELeQ1nXTKJ7mF87JM3L13-Vr-IA3-Dq5S11GDjC9aOvPNybhvNrme0pFvq_aEobcX_ynLb_g2sy2vb983Q7N-6Ch_WHQNqd"/>
</div>
<h1 class="font-display-lg text-headline-lg-mobile md:text-display-lg text-white mb-6 tracking-tight leading-none">
                Sublimación Digital de <br/>
<span class="text-transparent bg-clip-text bg-gradient-to-r from-neon-fuchsia to-secondary">Alta Calidad</span>
</h1>
<p class="font-body-lg text-on-surface-variant mb-10 max-w-2xl mx-auto">
                Especialistas en la creación de prendas de alto impacto visual y durabilidad extrema para cada momento especial.
            </p>
<div class="flex flex-col md:flex-row gap-4 justify-center">
<button class="bg-primary-container text-on-primary-container px-10 py-4 rounded-full font-label-md text-label-md uppercase tracking-[0.2em] neon-glow-fuchsia hover:scale-105 hover:brightness-110 transition-all active:scale-95">
                    Cotizar Ahora
                </button>
<button class="glass-card text-white px-10 py-4 rounded-full font-label-md text-label-md uppercase tracking-[0.2em] border border-glass-border hover:bg-white/10 hover:border-neon-fuchsia transition-all active:scale-95">
                    Ver Catálogo
                </button>
</div>
</div>
<div class="absolute bottom-10 left-1/2 -translate-x-1/2 flex flex-col items-center gap-2 opacity-50">
<span class="text-xs uppercase tracking-widest font-label-md">Explorar</span>
<div class="w-[2px] h-12 bg-gradient-to-b from-neon-fuchsia to-transparent animate-bounce"></div>
</div>
</section>
<!-- Polos de Algodón Jersey Spum -->
<section class="py-xl px-margin-mobile md:px-xl" id="cotton">
<div class="text-center mb-16">
<h2 class="font-headline-lg text-headline-lg-mobile md:text-headline-lg text-white mb-4">Polos de Algodón Jersey Spum</h2>
<div class="w-32 h-1 bg-neon-fuchsia mx-auto mb-6"></div>
<p class="text-on-surface-variant max-w-2xl mx-auto font-body-lg">Prendas con tacto de algodón, suaves y frescas, personalizadas con la mejor calidad de impresión.</p>
</div>
<div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-8">
<!-- Aniversarios -->
<div class="glass-card rounded-3xl overflow-hidden group hover:border-primary-fixed transition-all duration-500">
<div class="h-48 relative overflow-hidden">
<img alt="Cumpleaños" class="absolute inset-0 w-full h-full object-cover group-hover:scale-110 transition-transform duration-700" src="https://lh3.googleusercontent.com/aida-public/AB6AXuDw6Mg4-5BVp0NyYMCdh-FEMpMTN09pyxW2MmI_FEzf-aWwIp2ZfPGH7elDESZI6JzjxcZxgbZ2DABz3L2RQ17z8RcSYLE1X72ptbEvXfcqI1yZ-YtsfWz3eyp7Z51xoFQZNeuLhJVfiNkGkRspBcGfKfHGin10wQA9cia7M0nARl_RRpLY8ZLFrhTqtYT1e6V807NzKe58fRfgR-la7tHc2JqJ0GoGSuzUgoPv9J2hxQWC8aAsnM-FGnQmpqTgM6HexcTA3AAKvFP6"/>
<div class="absolute inset-0 bg-gradient-to-t from-surface-container to-transparent opacity-40"></div>
</div>
<div class="p-8">
    <!-- Cumpleaños -->
<h3 class="font-headline-md text-white mb-4">Cumpleaños</h3>
<p class="text-on-surface-variant text-sm mb-8 leading-relaxed">Diseños personalizados para que tu día sea inolvidable. El detalle perfecto para regalar.</p>
<a href="https://drive.google.com/drive/folders/1pmPN7RWWmc1j6k8CIP3-YXw_xS1MNKRf?usp=drive_link"
   target="_blank"
   class="w-full block text-center bg-surface-container-highest text-white py-4 rounded-xl">
   Ver Catálogo
</a>
</div>
</div><div class="glass-card rounded-3xl overflow-hidden group hover:border-neon-fuchsia transition-all duration-500">
<div class="h-48 relative overflow-hidden">
<img alt="Aniversarios / 14 de Febrero" class="absolute inset-0 w-full h-full object-cover group-hover:scale-110 transition-transform duration-700" src="https://lh3.googleusercontent.com/aida-public/AB6AXuCBHM1PzZsDaU4ZW2QSyvsSgDaowqP5JlQ71xuM1M5i81qN9N5a93xaqhRT3UIsxkz57P5hv-aaEoI8sPre0QSjSsxXFYeKw9TaGZEMIb5x1iWLftv4fp1BCwmqSWzANbHGRSSMSVT19WUwx6npQmkjhE4bBi2C6w2h80K07sI-rcymsebCZHNIK_Ag4Mj9x8mgH7jMYIi6i4RVgq4d3vkzJL7NGripbO02P-VXB-LK4jAuPl0IlIr9BPelvW2J84IIWcwypA6EVEDc"/>
<div class="absolute inset-0 bg-gradient-to-t from-surface-container to-transparent opacity-40"></div>
</div>
<div class="p-8">
<h3 class="font-headline-md text-white mb-4">Aniversarios</h3>
<p class="text-on-surface-variant text-sm mb-8 leading-relaxed">Diseños exclusivos para celebrar juntos. El regalo perfecto para esa fecha especial.</p>
<a href="https://drive.google.com/drive/folders/TU_ID_CARPETA"
   target="_blank"
   class="w-full block text-center bg-surface-container-highest text-white py-4 rounded-xl">
   Ver Catálogo
</a>
</div>
</div>
<!-- Polos para Difuntos -->
<div class="glass-card rounded-3xl overflow-hidden group hover:border-red-500/50 transition-all duration-500">

    <div class="h-48 relative overflow-hidden">
        <img alt="Polos para Difuntos"
             class="absolute inset-0 w-full h-full object-cover group-hover:scale-110 transition-transform duration-700"
             src="https://drive.google.com/thumbnail?id=10KNqXQiJ-97fVEStBpT1-SVQ2WTlxNpk&sz=w1000"/>

        <div class="absolute inset-0 bg-gradient-to-t from-surface-container to-transparent opacity-40"></div>
    </div>

    <div class="p-8">

        <h3 class="font-headline-md text-white mb-4">
            Polos para Difuntos
        </h3>

        <p class="text-on-surface-variant text-sm mb-8 leading-relaxed">
            Diseños personalizados para homenajes, aniversarios, misas y recordatorios.
        </p>

      <button
    onclick="document.getElementById('modalDifuntos').style.display='flex'"
    class="w-full bg-red-600 text-white py-4 rounded-xl font-label-md text-xs uppercase tracking-widest hover:bg-red-700 transition-all">
    Ver Catálogo
</button> 
    </div>

</div>

       <!-- MODAL CATÁLOGO DIFUNTOS -->
<div id="modalDifuntos"
     style="display:none;"
     class="fixed inset-0 bg-black/90 z-[9999] items-center justify-center p-6">

    <div class="bg-surface-container rounded-3xl max-w-7xl w-full max-h-[90vh] overflow-y-auto p-8">

        <div class="flex justify-between items-center mb-8">
            <h2 class="text-3xl font-bold text-white">
                Catálogo Polos para Difuntos
            </h2>

            <button
                onclick="document.getElementById('modalDifuntos').style.display='none'"
                class="text-white text-4xl">
                ×
            </button>
        </div>

        <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-6">

    <div class="glass-card rounded-2xl overflow-hidden">

    <a href="https://drive.google.com/file/d/10KNqXQiJ-97fVEStBpT1-SVQ2WTlxNpk/view?usp=drive_link"
       target="_blank">

        <img src="https://drive.google.com/thumbnail?id=10KNqXQiJ-97fVEStBpT1-SVQ2WTlxNpk&sz=w1000"
             class="w-full h-80 object-cover hover:scale-105 transition-all duration-300 cursor-pointer">

    </a>

    <div class="p-3 text-center text-white font-bold">
        M1
    </div>

</div>
<div class="glass-card rounded-2xl overflow-hidden">
    <a href="https://drive.google.com/file/d/1lQXUFyYpfPXgwRweW7w1sae1ZAhn1f8w/view?usp=drive_link" target="_blank">
        <img src="https://drive.google.com/thumbnail?id=1lQXUFyYpfPXgwRweW7w1sae1ZAhn1f8w&sz=w1000" class="w-full h-80 object-cover hover:scale-105 transition-all duration-300 cursor-pointer">
    </a>
    <div class="p-3 text-center text-white font-bold">M2</div>
</div>

<div class="glass-card rounded-2xl overflow-hidden">
    <a href="https://drive.google.com/file/d/1avWgtW5qtDQJErtQM9VzKfvtzRg-exoH/view?usp=drive_link" target="_blank">
        <img src="https://drive.google.com/thumbnail?id=1avWgtW5qtDQJErtQM9VzKfvtzRg-exoH&sz=w1000" class="w-full h-80 object-cover hover:scale-105 transition-all duration-300 cursor-pointer">
    </a>
    <div class="p-3 text-center text-white font-bold">M3</div>
</div>

<div class="glass-card rounded-2xl overflow-hidden">
    <a href="https://drive.google.com/file/d/1Ip08ZiwYuqAh7ltBSAvRBWvdgbUTgqZC/view?usp=drive_link" target="_blank">
        <img src="https://drive.google.com/thumbnail?id=1Ip08ZiwYuqAh7ltBSAvRBWvdgbUTgqZC&sz=w1000" class="w-full h-80 object-cover hover:scale-105 transition-all duration-300 cursor-pointer">
    </a>
    <div class="p-3 text-center text-white font-bold">M4</div>
</div>

<div class="glass-card rounded-2xl overflow-hidden">
    <a href="https://drive.google.com/file/d/1BLuXgdLPbmGotZaGo8Xb5Tgm6gHkcFBj/view?usp=drive_link" target="_blank">
        <img src="https://drive.google.com/thumbnail?id=1BLuXgdLPbmGotZaGo8Xb5Tgm6gHkcFBj&sz=w1000" class="w-full h-80 object-cover hover:scale-105 transition-all duration-300 cursor-pointer">
    </a>
    <div class="p-3 text-center text-white font-bold">M5</div>
</div>

<div class="glass-card rounded-2xl overflow-hidden">
    <a href="https://drive.google.com/file/d/1K_2Z0kJrOQxpcE-aN4MkcP0bIgf2h-ax/view?usp=drive_link" target="_blank">
        <img src="https://drive.google.com/thumbnail?id=1K_2Z0kJrOQxpcE-aN4MkcP0bIgf2h-ax&sz=w1000" class="w-full h-80 object-cover hover:scale-105 transition-all duration-300 cursor-pointer">
    </a>
    <div class="p-3 text-center text-white font-bold">M6</div>
</div>

<div class="glass-card rounded-2xl overflow-hidden">
    <a href="https://drive.google.com/file/d/19QInsfvxXrknGUCQ4iF5GaBv7mliLUec/view?usp=drive_link" target="_blank">
        <img src="https://drive.google.com/thumbnail?id=19QInsfvxXrknGUCQ4iF5GaBv7mliLUec&sz=w1000" class="w-full h-80 object-cover hover:scale-105 transition-all duration-300 cursor-pointer">
    </a>
    <div class="p-3 text-center text-white font-bold">M7</div>
</div>

<div class="glass-card rounded-2xl overflow-hidden">
    <a href="https://drive.google.com/file/d/1PAwZFOy8fGik-TgAN1uoVcxlPB7PPRqN/view?usp=drive_link" target="_blank">
        <img src="https://drive.google.com/thumbnail?id=1PAwZFOy8fGik-TgAN1uoVcxlPB7PPRqN&sz=w1000" class="w-full h-80 object-cover hover:scale-105 transition-all duration-300 cursor-pointer">
    </a>
    <div class="p-3 text-center text-white font-bold">M8</div>
</div>

<div class="glass-card rounded-2xl overflow-hidden">
    <a href="https://drive.google.com/file/d/14zx2yQb5zQJlDkH6WRFh665QB72YRO8h/view?usp=drive_link" target="_blank">
        <img src="https://drive.google.com/thumbnail?id=14zx2yQb5zQJlDkH6WRFh665QB72YRO8h&sz=w1000" class="w-full h-80 object-cover hover:scale-105 transition-all duration-300 cursor-pointer">
    </a>
    <div class="p-3 text-center text-white font-bold">M9</div>
</div>

<div class="glass-card rounded-2xl overflow-hidden">
    <a href="https://drive.google.com/file/d/1fs8R27cfzHFekscvUu6FWhzwWyijvqKo/view?usp=sharing" target="_blank">
        <img src="https://drive.google.com/thumbnail?id=1fs8R27cfzHFekscvUu6FWhzwWyijvqKo&sz=w1000" class="w-full h-80 object-cover hover:scale-105 transition-all duration-300 cursor-pointer">
    </a>
    <div class="p-3 text-center text-white font-bold">M10</div>
</div>

<div class="glass-card rounded-2xl overflow-hidden">
    <a href="https://drive.google.com/file/d/1qzjUrr5kzZJRsFXBc7-zmTvBc5ZR5bkq/view?usp=drive_link" target="_blank">
        <img src="https://drive.google.com/thumbnail?id=1qzjUrr5kzZJRsFXBc7-zmTvBc5ZR5bkq&sz=w1000" class="w-full h-80 object-cover hover:scale-105 transition-all duration-300 cursor-pointer">
    </a>
    <div class="p-3 text-center text-white font-bold">M11</div>
</div>

<div class="glass-card rounded-2xl overflow-hidden">
    <a href="https://drive.google.com/file/d/1uIg-g5sVK9Wkzq4tyQIBY0naCQl6RpiT/view?usp=drive_link" target="_blank">
        <img src="https://drive.google.com/thumbnail?id=1uIg-g5sVK9Wkzq4tyQIBY0naCQl6RpiT&sz=w1000" class="w-full h-80 object-cover hover:scale-105 transition-all duration-300 cursor-pointer">
    </a>
    <div class="p-3 text-center text-white font-bold">M12</div>
</div>
</div> <!-- FIN GRID -->

</div> <!-- FIN CONTENIDO MODAL -->

</div> <!-- FIN MODAL -->
<!-- 14 de Febrero -->
<div class="glass-card rounded-3xl overflow-hidden group hover:border-red-500/50 transition-all duration-500">
<div class="h-48 relative overflow-hidden">
<img alt="14 de Febrero" class="absolute inset-0 w-full h-full object-cover group-hover:scale-110 transition-transform duration-700" src="https://lh3.googleusercontent.com/aida-public/AB6AXuCBHM1PzZsDaU4ZW2QSyvsSgDaowqP5JlQ71xuM1M5i81qN9N5a93xaqhRT3UIsxkz57P5hv-aaEoI8sPre0QSjSsxXFYeKw9TaGZEMIb5x1iWLftv4fp1BCwmqSWzANbHGRSSMSVT19WUwx6npQmkjhE4bBi2C6w2h80K07sI-rcymsebCZHNIK_Ag4Mj9x8mgH7jMYIi6i4RVgq4d3vkzJL7NGripbO02P-VXB-LK4jAuPl0IlIr9BPelvW2J84IIWcwypA6EVEDc"/>
<div class="absolute inset-0 bg-gradient-to-t from-surface-container to-transparent opacity-40"></div>
</div>
<div class="p-8">
<h3 class="font-headline-md text-white mb-4">14 de Febrero</h3>
<p class="text-on-surface-variant text-sm mb-8 leading-relaxed">Polos para parejas y dúos creativos. Expresa tu amor con un diseño único.</p>
<a href="https://drive.google.com/drive/folders/ID_PADRE" target="_blank">
   Ver Catálogo
</a>
</div>
</div>
<!-- Día del Padre -->
<div class="glass-card rounded-3xl overflow-hidden group hover:border-secondary transition-all duration-500">
<div class="h-48 relative overflow-hidden">
<img alt="Día del Padre" class="absolute inset-0 w-full h-full object-cover group-hover:scale-110 transition-transform duration-700" src="https://lh3.googleusercontent.com/aida-public/AB6AXuDsUSjaB2OWMvnhmAIs9wdgcdNYYhmvzEmjzqEK3EgG2P07WjpCQTTnPZQIBZWicRMxFlf3dWB3XkA8ZRE5zagaqm9wjng4_xqb-jcstA9Re8LQPCzJGzRJBdXKvBTdz-MBSYs6U9Z6U255Z1u-bCi8sqLovSfyMLjFDiEgpUIhyff37w4QYZpB28vCWMHhm_oXMQcE_WP5WIsK96c8b_6wqjsF7EedlwcfhBzMus0tJsqSfsa8Et3RPp1iZp_UYdJazGQj2QSMrCB1"/>
<div class="absolute inset-0 bg-gradient-to-t from-surface-container to-transparent opacity-40"></div>
</div>
<div class="p-8">
<h3 class="font-headline-md text-white mb-4">Día del Padre</h3>
<p class="text-on-surface-variant text-sm mb-8 leading-relaxed">Homenajea al héroe de la casa con poleras y polos personalizados de gran calidad.</p>
<button class="w-full bg-surface-container-highest text-white py-4 rounded-xl font-label-md text-xs uppercase tracking-widest hover:bg-secondary hover:text-on-secondary transition-all border border-glass-border">Ver Catálogo</button>
</div>
</div>
<!-- Día de la Madre -->
<div class="glass-card rounded-3xl overflow-hidden group hover:border-primary-fixed transition-all duration-500">
<div class="h-48 relative overflow-hidden">
<img alt="Día de la Madre" class="absolute inset-0 w-full h-full object-cover group-hover:scale-110 transition-transform duration-700" src="https://lh3.googleusercontent.com/aida-public/AB6AXuDOFR39c6dojbjvGKgriHIigJKsSaijtlZVm0m11k9bDkCPttsDID2yyhJ_Msb7GiywphfV5UrJAGmAZhyP6kkHwG0Y66delLKL2-rFDhFmIUBLHj6AA7hr9fIl_c6cEN5F_5GtrMVOWecPPDZOhC90YvTAQpepT2D3sL1pQH7hbRV3Vex45mSWd8hsADa1ihWJMW8gPpprLRSNW30WtRz-CDFSEW3i34DJ0tC_V5TWEbBH1m2xOuXCVl36YXembHVeE0SYkd3nHjhl"/>
<div class="absolute inset-0 bg-gradient-to-t from-surface-container to-transparent opacity-40"></div>
</div>
<div class="p-8">
<h3 class="font-headline-md text-white mb-4">Día de la Madre</h3>
<p class="text-on-surface-variant text-sm mb-8 leading-relaxed">Para la reina del hogar, diseños llenos de color y sentimiento que duran para siempre.</p>
<button class="w-full bg-surface-container-highest text-white py-4 rounded-xl font-label-md text-xs uppercase tracking-widest hover:bg-primary-container hover:text-on-primary-container transition-all border border-glass-border">Ver Catálogo</button>
</div>
</div>
<!-- Día del Niño -->
<div class="glass-card rounded-3xl overflow-hidden group hover:border-tertiary transition-all duration-500">
<div class="h-48 relative overflow-hidden">
<img alt="Día del Niño" class="absolute inset-0 w-full h-full object-cover group-hover:scale-110 transition-transform duration-700" src="https://lh3.googleusercontent.com/aida-public/AB6AXuDgT8qFJhMz2x1TmDy2_PEaSfgWFEoxToWPn5dpoU6TYZnJRbmoQOE5HlQkAchFtFh-LQTEne69DcWZ-FuUTCmfVHwI-JTIu4TFDUWriYmSHwQtxgtC-WbFXZrofhTvu9aPnQ_xN30aWzKaK5nHZqeONPkOmuREbSZilQozSn7by2etk6a3wCwMtOHYLI-C2uhtzSCXy0GS3BDm8cImOrv-TmwUD9mt1pi-LpvYlBEuC0QiCbEzgRnLqDZBx1qoqFFNtnpCKXM7C1uA"/>
<div class="absolute inset-0 bg-gradient-to-t from-surface-container to-transparent opacity-40"></div>
</div>
<div class="p-8">
<h3 class="font-headline-md text-white mb-4">Día del Niño</h3>
<p class="text-on-surface-variant text-sm mb-8 leading-relaxed">Personajes y colores vibrantes para los más pequeños. Resistentes a toda aventura.</p>
<button class="w-full bg-surface-container-highest text-white py-4 rounded-xl font-label-md text-xs uppercase tracking-widest hover:bg-tertiary hover:text-on-tertiary transition-all border border-glass-border">Ver Catálogo</button>
</div>
</div>
<!-- Día del Maestro -->
<div class="glass-card rounded-3xl overflow-hidden group hover:border-white transition-all duration-500">
<div class="h-48 relative overflow-hidden">
<img alt="Día del Maestro" class="absolute inset-0 w-full h-full object-cover group-hover:scale-110 transition-transform duration-700" src="https://lh3.googleusercontent.com/aida-public/AB6AXuDO-DmILVPKzO3T33IPvbiX4tV7cD1LSezWKxcm229lXsghoeFH2QXGiyVTNWPYjyhEvcXvNuI8hcTi-rkbE--2NlFCGsBkireabYXwOqjMuEi1vdvitmjX2asE-1KFBDX6iEGD3H2t2n-oAoX-ONky3EcKM2ddWnzigNcHur4RA8fKtrVT7xStiUvqFiZvcvPhKkcRKGNUcbKKOj69IsgBi9Ue7AfKfoCWQ0aL-HMb7X3x4UaTOp91tr2Lp9mhzhbTtJcBIw94G_xR"/>
<div class="absolute inset-0 bg-gradient-to-t from-surface-container to-transparent opacity-40"></div>
</div>
<div class="p-8">
<h3 class="font-headline-md text-white mb-4">Día del Maestro</h3>
<p class="text-on-surface-variant text-sm mb-8 leading-relaxed">Un detalle significativo para quienes educan con pasión. Calidad y distinción.</p>
<button class="w-full bg-surface-container-highest text-white py-4 rounded-xl font-label-md text-xs uppercase tracking-widest hover:bg-white hover:text-black transition-all border border-glass-border">Ver Catálogo</button>
</div>
</div>
</div>
</section>
<!-- Ropa Deportiva Sublimada -->
<section class="py-xl bg-surface-container-low/20" id="sports">
<div class="px-margin-mobile md:px-xl max-w-7xl mx-auto">
<div class="flex flex-col md:flex-row md:items-end justify-between gap-6 mb-12">
<div>
<h2 class="font-headline-lg text-headline-lg-mobile md:text-headline-lg text-white mb-2">Ropa Deportiva Sublimada</h2>
<div class="w-20 h-1 bg-neon-fuchsia"></div>
</div>
</div>
<div class="grid grid-cols-1 md:grid-cols-3 gap-8">
<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Magenta Urep - Fútbol</title>

<style>
body{
  margin:0;
  font-family: Arial, sans-serif;
  background:#0b0b0f;
}

.glass-card{
  background: rgba(255,255,255,0.05);
  backdrop-filter: blur(10px);
  border: 1px solid rgba(255,255,255,0.1);
}

</style>
</head>

<body>

<!-- =========================
CATEGORÍA FUTBOL
========================= -->
<div class="relative group overflow-hidden rounded-3xl glass-card aspect-[4/5]" style="max-width:350px;margin:40px auto;">

  <img 
    src="https://drive.google.com/thumbnail?id=ID_CATEGORIA&sz=w1000"
    style="width:100%;height:100%;object-fit:cover;filter:brightness(70%)">

  <div style="position:absolute;bottom:0;padding:20px;color:white">

    <h2 style="font-size:28px;margin:0">Fútbol</h2>
    <p style="font-size:13px;opacity:0.8">
      Equipaciones deportivas dry-fit
    </p>

    <button 
      onclick="document.getElementById('catalogoFutbol').style.display='block'"
      style="margin-top:10px;padding:10px 20px;background:#ff00cc;color:white;border:none;border-radius:20px;cursor:pointer">
      Ver Modelos
    </button>

  </div>
</div>


<!-- =========================
CATALOGO MODAL
========================= -->
<div id="catalogoFutbol"
     style="display:none;position:fixed;top:0;left:0;width:100%;height:100%;background:black;overflow:auto;z-index:9999;padding:20px;">

  <div style="display:flex;justify-content:space-between;align-items:center">
    <h1 style="color:white">Catálogo Fútbol</h1>

    <button onclick="document.getElementById('catalogoFutbol').style.display='none'"
            style="font-size:30px;background:none;border:none;color:white;cursor:pointer">
      ×
    </button>
  </div>

  <!-- GRID -->
  <div style="display:grid;grid-template-columns:repeat(auto-fit,minmax(180px,1fr));gap:15px;margin-top:20px;">


    <!-- ================= PRODUCTO F01 ================= -->
 <!-- F01 FÚTBOL -->
<div class="glass-card rounded-2xl overflow-hidden group">

    <!-- IMAGEN -->
    <a href="https://drive.google.com/file/d/1wL9z3mkAlerovNW9yPef48aH6v3FJJtw/view?usp=sharing"
       target="_blank">

        <div class="w-full h-80 bg-black flex items-center justify-center overflow-hidden">

            <img 
                src="https://drive.google.com/thumbnail?id=1wL9z3mkAlerovNW9yPef48aH6v3FJJtw&sz=w1000"
                class="max-h-full max-w-full object-contain transition-transform duration-300 group-hover:scale-105"
                alt="F01 Fútbol"
            >

        </div>

    </a>

    <!-- INFO -->
    <div class="p-4 text-center text-white">

        <div class="font-bold text-lg">F01</div>

        <p class="text-sm text-white/70 mb-4">
            Conjunto deportivo de fútbol personalizado
        </p>

        <a href="https://wa.me/51937190991?text=Hola%20quiero%20comprar%20el%20modelo%20F01%20de%20Fútbol"
           target="_blank">

            <button class="w-full bg-green-500 hover:bg-green-600 text-white py-3 rounded-xl font-bold uppercase tracking-widest transition-all">
                Comprar
            </button>

        </a>

    </div>

</div>
    <!-- ================= PRODUCTO F02 ================= -->
    <div class="glass-card">
      <a href="https://drive.google.com/file/d/ID_F02/view" target="_blank">
        <img src="https://drive.google.com/thumbnail?id=ID_F02&sz=w1000"
             style="width:100%;height:200px;object-fit:cover">
      </a>
      <div style="color:white;text-align:center;padding:10px">F02</div>
      <a href="https://wa.me/51999999999?text=Quiero%20el%20modelo%20F02"
         style="display:block;background:#25D366;color:white;text-align:center;padding:8px;text-decoration:none">
         Comprar
      </a>
    </div>


    <!-- ================= PRODUCTO F03 ================= -->
    <div class="glass-card">
      <a href="https://drive.google.com/file/d/ID_F03/view" target="_blank">
        <img src="https://drive.google.com/thumbnail?id=ID_F03&sz=w1000"
             style="width:100%;height:200px;object-fit:cover">
      </a>
      <div style="color:white;text-align:center;padding:10px">F03</div>
      <a href="https://wa.me/51999999999?text=Quiero%20el%20modelo%20F03"
         style="display:block;background:#25D366;color:white;text-align:center;padding:8px;text-decoration:none">
         Comprar
      </a>
    </div>


    <!-- 🔁 REPITE HASTA F50 -->
    <!-- Solo cambia:
         ID_F04, ID_F05... etc
         F04, F05...
    -->

  </div>
</div>

<!-- Voley -->
<div class="relative group overflow-hidden rounded-3xl glass-card aspect-[4/5]">
<img alt="Voley" class="absolute inset-0 w-full h-full object-cover group-hover:scale-110 transition-transform duration-700 brightness-75" src="https://lh3.googleusercontent.com/aida/ADBb0uiepDtsX38eChRkLVsmJXdUmKa6x0Ufl_EZQiZZ6sxPtJfg8qNU4MjFlttmNmR5oOGlCb-8kYTNgNu3WkHbF7wGTv1BOzVuQPP2wZq-rUDFXGTJXe9nsSKXP80wS-v0ulwvm---KSr2qLsxrjbTOoL1l4PzoI3o4i1BUsDlSQEefw_GfOMqAq6uEborKBc_00ce7vthZmJJEqYrOkrr8ytrKCqhwZpBoFIHjmrBfP6anBKv-6edtzTZ9oU"/>
<div class="absolute inset-0 bg-gradient-to-t from-black via-black/20 to-transparent p-8 flex flex-col justify-end">
<h3 class="text-white font-display-lg text-3xl mb-2">Voley</h3>
<p class="text-on-surface-variant text-sm mb-6">Corte anatómico para máximo rendimiento.</p>
<button class="w-fit bg-secondary text-on-secondary px-8 py-3 rounded-full font-label-md text-xs uppercase tracking-widest hover:scale-105 transition-all">Ver Modelos</button>
</div>
</div>
<!-- Basket -->
<div class="relative group overflow-hidden rounded-3xl glass-card aspect-[4/5]">
<img alt="Basket" class="absolute inset-0 w-full h-full object-cover group-hover:scale-110 transition-transform duration-700 brightness-75" src="https://lh3.googleusercontent.com/aida-public/AB6AXuD8kgav9IEovAqAiiV6J5PESFhN2x6UcxQoPi4GHb5zilox7eXW6OOU7Wje2UUNT_mOYdL08krFhzVHuf129fD8Kue_dsO-GfVXxyBwcv4rtzlW5Tre0GOF5CpxNzZO0xoiJH4mrAy0FzgGPz_R1cn74-Iy31-CEdwgg4pMlwFgOiGLxLpCSM78KjsSVrzHWQOQa8tLUjwr4mpBa8hfrDfUtdqAjdAh5wx14Qz29ckZHFtFdJ77OB-TBcyETHsfDde0okIVb91g2Gt2"/>
<div class="absolute inset-0 bg-gradient-to-t from-black via-black/20 to-transparent p-8 flex flex-col justify-end">
<h3 class="text-white font-display-lg text-3xl mb-2">Basket</h3>
<p class="text-on-surface-variant text-sm mb-6">Camisetas y shorts en malla mesh premium.</p>
<button class="w-fit bg-tertiary text-on-tertiary px-8 py-3 rounded-full font-label-md text-xs uppercase tracking-widest hover:scale-105 transition-all">Ver Modelos</button>
</div>
</div>
</div>
</div>
</section>
<!-- Tecnología de Punta -->
<section class="py-xl px-margin-mobile md:px-xl" id="tech">
<div class="max-w-7xl mx-auto flex flex-col md:flex-row items-center gap-12">
<div class="w-full md:w-1/2">
<span class="text-neon-fuchsia font-label-md uppercase tracking-[0.3em]">Nuestra Tecnología</span>
<h2 class="font-display-lg text-headline-lg-mobile md:text-headline-lg text-white mt-4 mb-8">Epson SureColor F6200</h2>
<p class="font-body-lg text-on-surface-variant mb-6 leading-relaxed">
                    Utilizamos maquinaria de última generación para garantizar que cada diseño cobre vida con una nitidez incomparable. La **Epson F6200** nos permite lograr:
                </p>
<ul class="space-y-4 mb-10">
<li class="flex items-center gap-3 text-on-surface">
<span class="material-symbols-outlined text-neon-fuchsia">check_circle</span>
                        Impresión en alta definición (HD)
                    </li>
<li class="flex items-center gap-3 text-on-surface">
<span class="material-symbols-outlined text-neon-fuchsia">check_circle</span>
                        Colores vibrantes y tonos flúor reales
                    </li>
<li class="flex items-center gap-3 text-on-surface">
<span class="material-symbols-outlined text-neon-fuchsia">check_circle</span>
                        Degradados suaves y sin rastro de trama
                    </li>
</ul>
<div class="grid grid-cols-2 gap-4">
<div class="glass-card p-4 rounded-2xl text-center">
<p class="text-neon-fuchsia font-bold text-xl">100%</p>
<p class="text-[10px] uppercase text-on-surface-variant">Fidelidad de Color</p>
</div>
<div class="glass-card p-4 rounded-2xl text-center">
<p class="text-secondary font-bold text-xl">PRO</p>
<p class="text-[10px] uppercase text-on-surface-variant">Calidad de Exportación</p>
</div>
</div>
</div>
<div class="w-full md:w-1/2 grid grid-cols-2 gap-4">
<div class="space-y-4">
<img alt="Tecnología de Sublimación 1" class="rounded-3xl border border-glass-border shadow-2xl w-full aspect-square object-cover" src="https://lh3.googleusercontent.com/aida-public/AB6AXuD8kgav9IEovAqAiiV6J5PESFhN2x6UcxQoPi4GHb5zilox7eXW6OOU7Wje2UUNT_mOYdL08krFhzVHuf129fD8Kue_dsO-GfVXxyBwcv4rtzlW5Tre0GOF5CpxNzZO0xoiJH4mrAy0FzgGPz_R1cn74-Iy31-CEdwgg4pMlwFgOiGLxLpCSM78KjsSVrzHWQOQa8tLUjwr4mpBa8hfrDfUtdqAjdAh5wx14Qz29ckZHFtFdJ77OB-TBcyETHsfDde0okIVb91g2Gt2"/>
<div class="bg-neon-fuchsia h-24 rounded-3xl flex items-center justify-center">
<span class="material-symbols-outlined text-white text-4xl">print</span>
</div>
</div>
<div class="space-y-4 mt-8">
<div class="bg-secondary h-24 rounded-3xl flex items-center justify-center">
<span class="material-symbols-outlined text-white text-4xl">palette</span>
</div>
<img alt="Tecnología de Sublimación 2" class="rounded-3xl border border-glass-border shadow-2xl w-full aspect-square object-cover" src="https://lh3.googleusercontent.com/aida-public/AB6AXuDBTl6Ynox1ZUVN87XMyaK4EWHG3oSt_aOQNb2MmujYBhc-jhSDGq0k4EwfUyNqRCSPfp-lpkeChEqPvyhUL_QDPMmb_xN5zim3gYTifmpFZk2xiEfFqTWhh-33lnCw9cmOd9QopiAQdRZpLgVk5Awau3shPmOUxaV0Iyr3uERhGUe_f1VvXfqXDjR3kuzNqPVF2V90Prp5WRQSKMyDA0rhy6L1fvy_7FCyyyHU465f9pPa51BQD8sVNA39Dl_fdAKr-jBQP1KtQD96"/>
</div>
</div>
</div>
</section>
<!-- Servicios para Confeccionistas -->
<section class="py-xl bg-surface-container" id="services">
<div class="px-margin-mobile md:px-xl max-w-7xl mx-auto">
<div class="text-center mb-16">
<h2 class="font-headline-lg text-white mb-4">Servicios para Confeccionistas</h2>
<p class="text-on-surface-variant max-w-2xl mx-auto">Impulsamos tu negocio con servicios de impresión por volumen y personalizados.</p>
</div>
<div class="grid grid-cols-1 md:grid-cols-2 gap-8">
<!-- Por Metro Lineal -->
<div class="glass-card p-10 rounded-[40px] border-l-4 border-l-neon-fuchsia group hover:bg-white/5 transition-all">
<div class="flex items-center gap-6 mb-8">
<div class="w-16 h-16 rounded-2xl bg-neon-fuchsia/10 flex items-center justify-center">
<span class="material-symbols-outlined text-neon-fuchsia text-3xl">straighten</span>
</div>
<h3 class="text-white font-headline-md">Por Metro Lineal</h3>
</div>
<p class="text-on-surface-variant mb-10 leading-relaxed">Ideal para grandes producciones. Trae tu tela y nosotros ponemos el color. Servicio rápido y preciso.</p>
<div class="flex items-center justify-between">
<span class="text-white font-bold text-2xl">Consultar Precio</span>
<a class="bg-neon-fuchsia text-white px-8 py-3 rounded-full font-label-md text-xs uppercase tracking-widest hover:scale-105 transition-all" href="https://wa.me/51937190991">Cotizar Ahora</a>
</div>
</div>
<!-- Por Prenda -->
<div class="glass-card p-10 rounded-[40px] border-l-4 border-l-secondary group hover:bg-white/5 transition-all">
<div class="flex items-center gap-6 mb-8">
<div class="w-16 h-16 rounded-2xl bg-secondary/10 flex items-center justify-center">
<span class="material-symbols-outlined text-secondary text-3xl">checkroom</span>
</div>
<h3 class="text-white font-headline-md">Por Prenda</h3>
</div>
<p class="text-on-surface-variant mb-10 leading-relaxed">Personalización individual o por pequeños lotes. Acabados perfectos en cada detalle de la prenda.</p>
<div class="flex items-center justify-between">
<span class="text-white font-bold text-2xl">Desde S/ 15.00</span>
<a class="bg-secondary text-on-secondary px-8 py-3 rounded-full font-label-md text-xs uppercase tracking-widest hover:scale-105 transition-all" href="https://wa.me/51937190991">Saber Más</a>
</div>
</div>
</div>
</div>
</section>
<!-- Ubicación -->
<section class="py-xl px-margin-mobile md:px-xl" id="location">
<div class="mb-12">
<h2 class="font-headline-lg text-white mb-2">Nuestra Ubicación</h2>
<div class="w-20 h-1 bg-neon-fuchsia"></div>
</div>
<div class="grid grid-cols-1 lg:grid-cols-3 gap-8">
<div class="lg:col-span-2 relative h-[400px] rounded-3xl overflow-hidden glass-card group">
<a class="absolute inset-0 block" href="https://www.google.com/maps/search/?api=1&amp;query=Centro+Comercial+Hatun+Huasi+Ate" target="_blank">
<div class="w-full h-full bg-[#1a1a1a] relative">
<div class="absolute inset-0 opacity-20" style="background-image: linear-gradient(#333 1px, transparent 1px), linear-gradient(90deg, #333 1px, transparent 1px); background-size: 50px 50px;"></div>
<svg class="absolute inset-0 w-full h-full opacity-30" preserveaspectratio="none" viewbox="0 0 100 100">
<path d="M0 20 Q 50 30 100 10" fill="none" stroke="#ff00ff" stroke-width="0.5"></path>
<path d="M20 0 Q 30 50 10 100" fill="none" stroke="#abc7ff" stroke-width="0.5"></path>
</svg>
<div class="absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2 flex flex-col items-center">
<div class="w-12 h-12 bg-neon-fuchsia rounded-full flex items-center justify-center animate-bounce shadow-[0_0_20px_rgba(255,0,255,0.8)]">
<span class="material-symbols-outlined text-white text-3xl">location_on</span>
</div>
</div>
</div>
<div class="absolute inset-0 bg-gradient-to-t from-black/80 to-transparent flex items-end p-8">
<span class="text-white font-label-md text-xs uppercase tracking-widest flex items-center gap-2">
<span class="material-symbols-outlined text-sm">open_in_new</span> Abrir en Google Maps
                        </span>
</div>
</a>
</div>
<div class="glass-card p-10 rounded-3xl flex flex-col justify-center">
<h3 class="text-white font-headline-md mb-6">Visítanos</h3>
<div class="space-y-8 mb-10">
<div class="flex items-start gap-4">
<span class="material-symbols-outlined text-neon-fuchsia">location_on</span>
<div>
<p class="text-white font-semibold">Dirección</p>
<p class="text-on-surface-variant text-sm">Centro Comercial Hatun Huasi, Ate Peru (X39F+FM9)</p>
</div>
</div>
<div class="flex items-start gap-4">
<span class="material-symbols-outlined text-neon-fuchsia">schedule</span>
<div>
<p class="text-white font-semibold">Horario</p>
<p class="text-on-surface-variant text-sm">Lun - Sáb: 10:00 AM - 7:00 PM</p>
</div>
</div>
<div class="flex items-start gap-4">
<span class="material-symbols-outlined text-neon-fuchsia">call</span>
<div>
<p class="text-white font-semibold">Teléfono</p>
<p class="text-on-surface-variant text-sm">+51 937 190 991</p>
</div>
</div>
</div>
<a class="w-full bg-neon-fuchsia text-white py-4 rounded-full font-label-md text-xs uppercase tracking-widest text-center hover:brightness-110 transition-all flex items-center justify-center gap-2 shadow-[0_0_15px_rgba(255,0,255,0.3)]" href="https://www.google.com/maps/search/?api=1&amp;query=Centro+Comercial+Hatun+Huasi+Ate" target="_blank">
<span class="material-symbols-outlined text-sm">directions</span> Cómo llegar
                </a>
</div>
</div>
</section>
</main>
<footer class="bg-surface-container-lowest pt-20 pb-10 border-t border-glass-border">
<div class="max-w-7xl mx-auto px-margin-mobile md:px-xl">
<div class="grid grid-cols-1 md:grid-cols-4 gap-12 mb-16">
<div class="col-span-1 md:col-span-2">
<span class="font-display-lg text-[28px] text-neon-fuchsia tracking-widest uppercase font-extrabold mb-6 block">MAGENTA</span>
<p class="text-on-surface-variant max-w-sm mb-6">Expertos en sublimación digital y confección de prendas deportivas y publicitarias de alta gama.</p>
<div class="flex gap-4">
<a class="w-10 h-10 rounded-full glass-card flex items-center justify-center hover:text-neon-fuchsia transition-all border border-glass-border" href="#"><span class="material-symbols-outlined text-[20px]">public</span></a>
<a class="w-10 h-10 rounded-full glass-card flex items-center justify-center hover:text-neon-fuchsia transition-all border border-glass-border" href="#"><span class="material-symbols-outlined text-[20px]">alternate_email</span></a>
</div>
</div>
<div>
<h5 class="text-white font-label-md uppercase mb-6">Categorías</h5>
<ul class="space-y-4 text-on-surface-variant text-sm">
<li class=""><a class="hover:text-neon-fuchsia transition-colors" href="#cotton">Polos Jersey Spum</a></li>
<li class=""><a class="hover:text-neon-fuchsia transition-colors" href="#sports">Uniformes Deportivos</a></li>
<li class=""><a class="hover:text-neon-fuchsia transition-colors" href="#services">Servicio Confeccionistas</a></li>
</ul>
</div>
<div>
<h5 class="text-white font-label-md uppercase mb-6">Magenta Digital</h5>
<ul class="space-y-4 text-on-surface-variant text-sm">
<li class="flex items-center gap-2"><span class="material-symbols-outlined text-neon-fuchsia text-sm">call</span> +51 937 190 991</li>
<li class="flex items-center gap-2"><span class="material-symbols-outlined text-neon-fuchsia text-sm">location_on</span> Centro Comercial Hatun Huasi, Ate</li>
</ul>
</div>
</div>
<div class="pt-8 border-t border-glass-border text-center text-[10px] text-on-surface-variant/40 uppercase tracking-[0.3em]">
            © 2019 MAGENTA SUBLIMADO DIGITAL. TODOS LOS DERECHOS RESERVADOS.
        </div>
</div>
</footer>
<!-- Bottom Navigation for Mobile -->
<nav class="md:hidden fixed bottom-0 w-full z-50 bg-surface-container-lowest/90 backdrop-blur-2xl border-t border-glass-border">
<div class="flex justify-around items-center py-3">
<a class="flex flex-col items-center text-neon-fuchsia" href="#cotton">
<span class="material-symbols-outlined">grid_view</span>
<span class="text-[10px] uppercase font-bold mt-1">Catálogo</span>
</a>
<a class="flex flex-col items-center text-on-surface-variant opacity-70" href="#sports">
<span class="material-symbols-outlined">sports_basketball</span>
<span class="text-[10px] uppercase font-bold mt-1">Deportes</span>
</a>
<a class="flex flex-col items-center text-on-surface-variant opacity-70" href="#services">
<span class="material-symbols-outlined">settings</span>
<span class="text-[10px] uppercase font-bold mt-1">Servicios</span>
</a>
<a class="flex flex-col items-center text-on-surface-variant opacity-70" href="https://wa.me/51937190991">
<span class="material-symbols-outlined">chat</span>
<span class="text-[10px] uppercase font-bold mt-1">WhatsApp</span>
</a>
</div>
</nav>
<script>
    window.addEventListener('scroll', () => {
        const header = document.querySelector('header');
        if (window.scrollY > 50) {
            header.style.backgroundColor = 'rgba(19, 19, 19, 0.95)';
        } else {
            header.style.backgroundColor = 'rgba(19, 19, 19, 0.8)';
        }
    });
</script>
</body></html>
