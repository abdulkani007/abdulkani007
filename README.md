<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Abdul Kani — GitHub README Preview</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800;900&family=JetBrains+Mono:wght@400;500;600&family=Poppins:wght@600;700;800;900&display=swap" rel="stylesheet">
    <script src="https://code.iconify.design/3/3.1.0/iconify.min.js"></script>
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        inter: ['Inter', 'sans-serif'],
                        poppins: ['Poppins', 'sans-serif'],
                        mono: ['JetBrains Mono', 'monospace'],
                    },
                    colors: {
                        brand: {
                            50: '#ecfeff',
                            100: '#cffafe',
                            200: '#a5f3fc',
                            300: '#67e8f9',
                            400: '#22d3ee',
                            500: '#06b6d4',
                            600: '#0891b2',
                            700: '#0e7490',
                            800: '#155e75',
                            900: '#164e63',
                        }
                    }
                }
            }
        }
    </script>
    <style>
        * { margin: 0; padding: 0; box-sizing: border-box; }
        body {
            font-family: 'Inter', sans-serif;
            background: #030305;
            color: #ffffff;
            overflow-x: hidden;
        }
        ::-webkit-scrollbar { width: 6px; }
        ::-webkit-scrollbar-track { background: #030305; }
        ::-webkit-scrollbar-thumb { background: #333; border-radius: 3px; }
        ::-webkit-scrollbar-thumb:hover { background: #555; }

        .bg-grid {
            background-image:
                linear-gradient(to right, rgba(255,255,255,0.02) 1px, transparent 1px),
                linear-gradient(to bottom, rgba(255,255,255,0.02) 1px, transparent 1px);
            background-size: 40px 40px;
            mask-image: radial-gradient(ellipse at center, black 30%, transparent 75%);
        }

        .glass-card {
            background: rgba(10, 10, 12, 0.75);
            backdrop-filter: blur(20px);
            border: 1px solid rgba(255,255,255,0.06);
            box-shadow: 0 8px 32px rgba(0,0,0,0.6);
        }

        .glass-card-hover {
            transition: all 0.4s cubic-bezier(0.16, 1, 0.3, 1);
        }
        .glass-card-hover:hover {
            border-color: rgba(6,182,212,0.3);
            box-shadow: 0 0 40px -10px rgba(6,182,212,0.15);
            transform: translateY(-4px);
        }

        .text-gradient {
            background: linear-gradient(to bottom right, #ffffff, #94a3b8);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }

        .text-gradient-cyan {
            background: linear-gradient(135deg, #22d3ee, #06b6d4, #0891b2);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }

        .text-gradient-warm {
            background: linear-gradient(135deg, #f59e0b, #ef4444, #ec4899);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }

        .glow-cyan {
            box-shadow: 0 0 60px -15px rgba(6,182,212,0.3);
        }

        .glow-dot {
            box-shadow: 0 0 12px rgba(6,182,212,0.8);
        }

        @keyframes float {
            0%, 100% { transform: translateY(0px); }
            50% { transform: translateY(-12px); }
        }
        @keyframes float-delayed {
            0%, 100% { transform: translateY(0px); }
            50% { transform: translateY(-8px); }
        }
        @keyframes pulse-ring {
            0% { transform: scale(1); opacity: 0.6; }
            100% { transform: scale(2.5); opacity: 0; }
        }
        @keyframes typing {
            from { width: 0; }
            to { width: 100%; }
        }
        @keyframes blink {
            50% { border-color: transparent; }
        }
        @keyframes slide-up {
            from { opacity: 0; transform: translateY(30px); }
            to { opacity: 1; transform: translateY(0); }
        }
        @keyframes slide-in-left {
            from { opacity: 0; transform: translateX(-30px); }
            to { opacity: 1; transform: translateX(0); }
        }
        @keyframes fade-in {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        @keyframes shimmer {
            0% { background-position: -200% 0; }
            100% { background-position: 200% 0; }
        }
        @keyframes orbit {
            from { transform: rotate(0deg) translateX(140px) rotate(0deg); }
            to { transform: rotate(360deg) translateX(140px) rotate(-360deg); }
        }
        @keyframes orbit-reverse {
            from { transform: rotate(360deg) translateX(100px) rotate(-360deg); }
            to { transform: rotate(0deg) translateX(100px) rotate(0deg); }
        }
        @keyframes rotate-slow {
            from { transform: rotate(0deg); }
            to { transform: rotate(360deg); }
        }

        .animate-float { animation: float 6s ease-in-out infinite; }
        .animate-float-delayed { animation: float-delayed 7s ease-in-out infinite 1s; }
        .animate-pulse-ring { animation: pulse-ring 2s cubic-bezier(0,0,0.2,1) infinite; }
        .animate-slide-up { animation: slide-up 0.8s cubic-bezier(0.16, 1, 0.3, 1) forwards; }
        .animate-slide-in-left { animation: slide-in-left 0.8s cubic-bezier(0.16, 1, 0.3, 1) forwards; }
        .animate-fade-in { animation: fade-in 1s ease forwards; }
        .animate-orbit { animation: orbit 20s linear infinite; }
        .animate-orbit-reverse { animation: orbit-reverse 15s linear infinite; }
        .animate-rotate-slow { animation: rotate-slow 30s linear infinite; }

        .shimmer-bg {
            background: linear-gradient(90deg, transparent, rgba(255,255,255,0.04), transparent);
            background-size: 200% 100%;
            animation: shimmer 3s ease-in-out infinite;
        }

        .tech-icon {
            transition: all 0.3s cubic-bezier(0.16, 1, 0.3, 1);
            filter: grayscale(40%) brightness(0.8);
        }
        .tech-icon:hover {
            filter: grayscale(0%) brightness(1.1);
            transform: translateY(-6px) scale(1.1);
        }

        .project-card {
            position: relative;
            overflow: hidden;
        }
        .project-card::before {
            content: '';
            position: absolute;
            top: 0; left: 0; right: 0;
            height: 2px;
            background: linear-gradient(90deg, transparent, #06b6d4, transparent);
            opacity: 0;
            transition: opacity 0.4s;
        }
        .project-card:hover::before {
            opacity: 1;
        }

        .stat-card {
            position: relative;
            overflow: hidden;
        }
        .stat-card::after {
            content: '';
            position: absolute;
            bottom: 0; left: 0; right: 0;
            height: 3px;
            background: linear-gradient(90deg, #06b6d4, #8b5cf6);
            transform: scaleX(0);
            transform-origin: left;
            transition: transform 0.5s cubic-bezier(0.16, 1, 0.3, 1);
        }
        .stat-card:hover::after {
            transform: scaleX(1);
        }

        .badge-shine {
            position: relative;
            overflow: hidden;
        }
        .badge-shine::after {
            content: '';
            position: absolute;
            top: -50%; left: -50%;
            width: 200%; height: 200%;
            background: linear-gradient(45deg, transparent 40%, rgba(255,255,255,0.08) 50%, transparent 60%);
            animation: shimmer 4s ease-in-out infinite;
        }

        .section-reveal {
            opacity: 0;
            transform: translateY(30px);
            transition: all 0.8s cubic-bezier(0.16, 1, 0.3, 1);
        }
        .section-reveal.visible {
            opacity: 1;
            transform: translateY(0);
        }

        .nav-glass {
            background: rgba(3, 3, 5, 0.8);
            backdrop-filter: blur(16px);
            border-bottom: 1px solid rgba(255,255,255,0.05);
        }

        .code-block {
            background: rgba(0,0,0,0.5);
            border: 1px solid rgba(255,255,255,0.06);
            border-radius: 12px;
            overflow: hidden;
        }
        .code-header {
            background: rgba(255,255,255,0.03);
            border-bottom: 1px solid rgba(255,255,255,0.06);
            padding: 10px 16px;
            display: flex;
            align-items: center;
            gap: 8px;
        }
        .code-dot {
            width: 10px; height: 10px;
            border-radius: 50%;
        }

        .trophy-card {
            transition: all 0.4s cubic-bezier(0.16, 1, 0.3, 1);
        }
        .trophy-card:hover {
            transform: scale(1.05);
        }

        .connect-btn {
            transition: all 0.3s cubic-bezier(0.16, 1, 0.3, 1);
            position: relative;
            overflow: hidden;
        }
        .connect-btn::before {
            content: '';
            position: absolute;
            inset: 0;
            background: linear-gradient(135deg, rgba(255,255,255,0.1), transparent);
            opacity: 0;
            transition: opacity 0.3s;
        }
        .connect-btn:hover::before {
            opacity: 1;
        }
        .connect-btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 8px 30px rgba(0,0,0,0.4);
        }

        .tab-btn {
            transition: all 0.3s ease;
        }
        .tab-btn.active {
            background: rgba(6,182,212,0.15);
            color: #22d3ee;
            border-color: rgba(6,182,212,0.3);
        }

        .markdown-output {
            background: #0d1117;
            border: 1px solid rgba(255,255,255,0.1);
            border-radius: 16px;
            overflow: hidden;
        }
        .markdown-header {
            background: linear-gradient(135deg, rgba(6,182,212,0.1), rgba(139,92,246,0.1));
            border-bottom: 1px solid rgba(255,255,255,0.06);
            padding: 14px 20px;
            display: flex;
            align-items: center;
            justify-content: space-between;
        }
    </style>
</head>
<body class="bg-grid">

    <!-- Ambient Glow -->
    <div class="fixed inset-0 pointer-events-none z-0">
        <div class="absolute top-0 left-1/2 -translate-x-1/2 w-[900px] h-[500px] bg-brand-500/[0.04] rounded-full blur-[150px]"></div>
        <div class="absolute top-[60%] right-0 w-[500px] h-[500px] bg-purple-500/[0.03] rounded-full blur-[120px]"></div>
        <div class="absolute bottom-0 left-0 w-[600px] h-[400px] bg-blue-500/[0.02] rounded-full blur-[100px]"></div>
    </div>

    <!-- Navigation -->
    <nav class="fixed top-0 left-0 right-0 z-50 nav-glass">
        <div class="max-w-7xl mx-auto px-6 h-16 flex items-center justify-between">
            <div class="flex items-center gap-3">
                <div class="w-8 h-8 rounded-lg bg-gradient-to-br from-brand-400 to-brand-600 flex items-center justify-center">
                    <span class="text-white font-bold text-sm font-poppins">A</span>
                </div>
                <span class="font-poppins font-bold text-lg tracking-tight">Abdul Kani</span>
            </div>
            <div class="hidden md:flex items-center gap-6">
                <a href="#about" class="text-sm font-medium text-slate-400 hover:text-white transition-colors duration-300">About</a>
                <a href="#stack" class="text-sm font-medium text-slate-400 hover:text-white transition-colors duration-300">Tech Stack</a>
                <a href="#projects" class="text-sm font-medium text-slate-400 hover:text-white transition-colors duration-300">Projects</a>
                <a href="#stats" class="text-sm font-medium text-slate-400 hover:text-white transition-colors duration-300">Stats</a>
                <a href="#connect" class="text-sm font-medium text-slate-400 hover:text-white transition-colors duration-300">Connect</a>
            </div>
            <button id="copyMdBtn" class="flex items-center gap-2 px-4 py-2 rounded-full bg-brand-500/10 border border-brand-500/20 text-brand-400 text-xs font-semibold tracking-wide uppercase hover:bg-brand-500/20 transition-all duration-300">
                <span class="iconify" data-icon="lucide:copy" data-width="14"></span>
                Copy Markdown
            </button>
        </div>
    </nav>

    <!-- Toast -->
    <div id="toast" class="fixed top-20 right-6 z-[100] px-5 py-3 rounded-xl bg-emerald-500/10 border border-emerald-500/30 text-emerald-400 text-sm font-medium flex items-center gap-2 opacity-0 translate-x-8 transition-all duration-500 pointer-events-none">
        <span class="iconify" data-icon="lucide:check-circle" data-width="16"></span>
        Markdown copied to clipboard!
    </div>

    <!-- Hero Section -->
    <section class="relative min-h-screen flex items-center justify-center pt-16 overflow-hidden">
        <!-- Orbiting Elements -->
        <div class="absolute inset-0 flex items-center justify-center pointer-events-none">
            <div class="animate-orbit opacity-30">
                <div class="w-3 h-3 rounded-full bg-brand-400 glow-dot"></div>
            </div>
        </div>
        <div class="absolute inset-0 flex items-center justify-center pointer-events-none">
            <div class="animate-orbit-reverse opacity-20">
                <div class="w-2 h-2 rounded-full bg-purple-400"></div>
            </div>
        </div>

        <!-- Rotating ring -->
        <div class="absolute inset-0 flex items-center justify-center pointer-events-none">
            <div class="w-[300px] h-[300px] md:w-[400px] md:h-[400px] rounded-full border border-white/[0.03] animate-rotate-slow"></div>
        </div>
        <div class="absolute inset-0 flex items-center justify-center pointer-events-none">
            <div class="w-[500px] h-[500px] md:w-[650px] md:h-[650px] rounded-full border border-white/[0.02] animate-rotate-slow" style="animation-direction: reverse; animation-duration: 45s;"></div>
        </div>

        <div class="relative z-10 text-center px-6 max-w-4xl mx-auto">
            <!-- Status Badge -->
            <div class="inline-flex items-center gap-2 px-4 py-2 rounded-full bg-white/[0.03] border border-white/[0.06] mb-8 animate-fade-in" style="animation-delay: 0.2s;">
                <span class="relative flex h-2.5 w-2.5">
                    <span class="animate-pulse-ring absolute inline-flex h-full w-full rounded-full bg-emerald-400 opacity-75"></span>
                    <span class="relative inline-flex rounded-full h-2.5 w-2.5 bg-emerald-400"></span>
                </span>
                <span class="text-xs font-medium text-slate-400 tracking-wide uppercase">Available for Opportunities</span>
            </div>

            <!-- Name -->
            <h1 class="font-poppins font-black text-5xl md:text-7xl lg:text-8xl tracking-tight leading-[1.05] mb-6 animate-slide-up" style="animation-delay: 0.3s;">
                <span class="text-gradient">Abdul</span>
                <br>
                <span class="text-gradient-cyan">Kani</span>
            </h1>

            <!-- Typing subtitle -->
            <div class="h-10 mb-8 animate-slide-up" style="animation-delay: 0.5s;">
                <p class="text-lg md:text-xl font-light text-slate-400 tracking-tight">
                    AI Engineer <span class="text-brand-400 mx-2">·</span> Full Stack Developer <span class="text-brand-400 mx-2">·</span> Hackathon Builder
                </p>
            </div>

            <!-- Profile Views -->
            <div class="animate-slide-up" style="animation-delay: 0.7s;">
                <div class="inline-flex items-center gap-3 px-5 py-2.5 rounded-full bg-white/[0.03] border border-white/[0.06]">
                    <span class="iconify text-brand-400" data-icon="lucide:eye" data-width="16"></span>
                    <span class="text-sm text-slate-300 font-medium" id="viewCount">0</span>
                    <span class="text-xs text-slate-500">profile views</span>
                </div>
            </div>

            <!-- CTA Buttons -->
            <div class="flex flex-wrap items-center justify-center gap-4 mt-10 animate-slide-up" style="animation-delay: 0.9s;">
                <a href="#projects" class="group flex items-center gap-2 px-7 py-3.5 rounded-full bg-white text-black text-sm font-semibold hover:shadow-[0_0_40px_-10px_rgba(255,255,255,0.3)] transition-all duration-300 hover:-translate-y-0.5">
                    View Projects
                    <span class="iconify group-hover:translate-x-1 transition-transform" data-icon="lucide:arrow-right" data-width="16"></span>
                </a>
                <a href="#connect" class="flex items-center gap-2 px-7 py-3.5 rounded-full bg-white/[0.06] border border-white/[0.1] text-white text-sm font-medium hover:bg-white/[0.1] hover:border-white/[0.2] transition-all duration-300 hover:-translate-y-0.5">
                    <span class="iconify" data-icon="lucide:mail" data-width="16"></span>
                    Get In Touch
                </a>
            </div>
        </div>

        <!-- Scroll indicator -->
        <div class="absolute bottom-8 left-1/2 -translate-x-1/2 flex flex-col items-center gap-2 animate-fade-in" style="animation-delay: 1.5s;">
            <span class="text-[10px] uppercase tracking-[0.2em] text-slate-600 font-medium">Scroll</span>
            <div class="w-5 h-8 rounded-full border border-white/10 flex items-start justify-center p-1">
                <div class="w-1 h-2 rounded-full bg-brand-400 animate-bounce"></div>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="relative py-24 md:py-32 px-6 section-reveal">
        <div class="max-w-7xl mx-auto">
            <div class="grid md:grid-cols-2 gap-12 md:gap-16 items-center">
                <!-- Left -->
                <div>
                    <div class="flex items-center gap-3 mb-6">
                        <div class="h-px w-8 bg-brand-500"></div>
                        <span class="text-xs font-semibold uppercase tracking-[0.2em] text-brand-400">About Me</span>
                    </div>
                    <h2 class="font-poppins font-bold text-3xl md:text-4xl tracking-tight mb-6 text-gradient">
                        Building AI that solves<br>real-world problems
                    </h2>
                    <p class="text-slate-400 font-light leading-relaxed text-base mb-8">
                        I'm a B.Tech IT student at <span class="text-white font-medium">Sri Eshwar College of Engineering</span>, Tamil Nadu. I specialize in building <span class="text-brand-400 font-medium">Agentic AI Applications</span> and full-stack web platforms that bridge the gap between intelligence and usability.
                    </p>

                    <!-- Quick Info -->
                    <div class="grid grid-cols-2 gap-3">
                        <div class="flex items-center gap-2.5 text-sm text-slate-400">
                            <span class="iconify text-brand-400" data-icon="lucide:map-pin" data-width="14"></span>
                            Tamil Nadu, India
                        </div>
                        <div class="flex items-center gap-2.5 text-sm text-slate-400">
                            <span class="iconify text-brand-400" data-icon="lucide:graduation-cap" data-width="14"></span>
                            B.Tech IT
                        </div>
                        <div class="flex items-center gap-2.5 text-sm text-slate-400">
                            <span class="iconify text-brand-400" data-icon="lucide:building-2" data-width="14"></span>
                            SECE, Coimbatore
                        </div>
                        <div class="flex items-center gap-2.5 text-sm text-slate-400">
                            <span class="iconify text-brand-400" data-icon="lucide:trophy" data-width="14"></span>
                            Hackathon Builder
                        </div>
                    </div>
                </div>

                <!-- Right - Code Block -->
                <div class="code-block">
                    <div class="code-header">
                        <div class="code-dot bg-red-500/80"></div>
                        <div class="code-dot bg-yellow-500/80"></div>
                        <div class="code-dot bg-green-500/80"></div>
                        <span class="text-xs text-slate-500 ml-2 font-mono">about_me.py</span>
                    </div>
                    <pre class="p-5 text-sm font-mono leading-relaxed overflow-x-auto"><code><span class="text-purple-400">class</span> <span class="text-brand-300">Developer</span>:
    <span class="text-purple-400">def</span> <span class="text-white">__init__</span>(<span class="text-orange-300">self</span>):
        <span class="text-orange-300">self</span>.name = <span class="text-emerald-400">"Abdul Kani"</span>
        <span class="text-orange-300">self</span>.role = <span class="text-emerald-400">"AI Engineer & Full Stack Dev"</span>
        <span class="text-orange-300">self</span>.passion = [
            <span class="text-emerald-400">"Agentic AI"</span>,
            <span class="text-emerald-400">"Computer Vision"</span>,
            <span class="text-emerald-400">"MERN Stack"</span>,
            <span class="text-emerald-400">"Intelligent Automation"</span>
        ]
        <span class="text-orange-300">self</span>.currently_building = <span class="text-emerald-400">"AI Products"</span>

    <span class="text-purple-400">def</span> <span class="text-white">get_motto</span>(<span class="text-orange-300">self</span>):
        <span class="text-purple-400">return</span> <span class="text-emerald-400">"Code. Learn. Build. Repeat."</span></code></pre>
                </div>
            </div>
        </div>
    </section>

    <!-- What I Love -->
    <section class="relative py-16 px-6 section-reveal">
        <div class="max-w-5xl mx-auto">
            <div class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-6 gap-4">
                <div class="glass-card glass-card-hover rounded-2xl p-5 text-center group cursor-default">
                    <div class="text-3xl mb-3 group-hover:scale-110 transition-transform duration-300">🤖</div>
                    <div class="text-xs font-medium text-slate-300">AI & ML</div>
                </div>
                <div class="glass-card glass-card-hover rounded-2xl p-5 text-center group cursor-default">
                    <div class="text-3xl mb-3 group-hover:scale-110 transition-transform duration-300">🌐</div>
                    <div class="text-xs font-medium text-slate-300">Full Stack</div>
                </div>
                <div class="glass-card glass-card-hover rounded-2xl p-5 text-center group cursor-default">
                    <div class="text-3xl mb-3 group-hover:scale-110 transition-transform duration-300">⚡</div>
                    <div class="text-xs font-medium text-slate-300">AI Products</div>
                </div>
                <div class="glass-card glass-card-hover rounded-2xl p-5 text-center group cursor-default">
                    <div class="text-3xl mb-3 group-hover:scale-110 transition-transform duration-300">🏆</div>
                    <div class="text-xs font-medium text-slate-300">Hackathons</div>
                </div>
                <div class="glass-card glass-card-hover rounded-2xl p-5 text-center group cursor-default">
                    <div class="text-3xl mb-3 group-hover:scale-110 transition-transform duration-300">📱</div>
                    <div class="text-xs font-medium text-slate-300">UI/UX</div>
                </div>
                <div class="glass-card glass-card-hover rounded-2xl p-5 text-center group cursor-default">
                    <div class="text-3xl mb-3 group-hover:scale-110 transition-transform duration-300">☁️</div>
                    <div class="text-xs font-medium text-slate-300">Cloud</div>
                </div>
            </div>
        </div>
    </section>

    <!-- Tech Stack Section -->
    <section id="stack" class="relative py-24 md:py-32 px-6 section-reveal">
        <div class="max-w-7xl mx-auto">
            <div class="text-center mb-16">
                <div class="flex items-center justify-center gap-3 mb-6">
                    <div class="h-px w-8 bg-brand-500"></div>
                    <span class="text-xs font-semibold uppercase tracking-[0.2em] text-brand-400">Tech Stack</span>
                    <div class="h-px w-8 bg-brand-500"></div>
                </div>
                <h2 class="font-poppins font-bold text-3xl md:text-4xl tracking-tight text-gradient">Tools I Work With</h2>
            </div>

            <div class="space-y-8">
                <!-- Languages -->
                <div class="glass-card rounded-2xl p-6 md:p-8">
                    <div class="flex items-center gap-3 mb-5">
                        <span class="iconify text-brand-400" data-icon="lucide:code-2" data-width="18"></span>
                        <h3 class="text-sm font-semibold uppercase tracking-wider text-slate-300">Languages</h3>
                    </div>
                    <div class="flex flex-wrap gap-4">
                        <div class="tech-icon flex items-center gap-2.5 px-4 py-2.5 rounded-xl bg-white/[0.03] border border-white/[0.06]">
                            <span class="iconify text-[#3776AB]" data-icon="logos:python" data-width="22"></span>
                            <span class="text-sm text-slate-300">Python</span>
                        </div>
                        <div class="tech-icon flex items-center gap-2.5 px-4 py-2.5 rounded-xl bg-white/[0.03] border border-white/[0.06]">
                            <span class="iconify text-[#ED8B00]" data-icon="logos:java" data-width="22"></span>
                            <span class="text-sm text-slate-300">Java</span>
                        </div>
                        <div class="tech-icon flex items-center gap-2.5 px-4 py-2.5 rounded-xl bg-white/[0.03] border border-white/[0.06]">
                            <span class="iconify" data-icon="logos:c-plusplus" data-width="22"></span>
                            <span class="text-sm text-slate-300">C++</span>
                        </div>
                        <div class="tech-icon flex items-center gap-2.5 px-4 py-2.5 rounded-xl bg-white/[0.03] border border-white/[0.06]">
                            <span class="iconify" data-icon="logos:c" data-width="22"></span>
                            <span class="text-sm text-slate-300">C</span>
                        </div>
                        <div class="tech-icon flex items-center gap-2.5 px-4 py-2.5 rounded-xl bg-white/[0.03] border border-white/[0.06]">
                            <span class="iconify text-[#F7DF1E]" data-icon="logos:javascript" data-width="22"></span>
                            <span class="text-sm text-slate-300">JavaScript</span>
                        </div>
                    </div>
                </div>

                <!-- Frontend -->
                <div class="glass-card rounded-2xl p-6 md:p-8">
                    <div class="flex items-center gap-3 mb-5">
                        <span class="iconify text-brand-400" data-icon="lucide:layout" data-width="18"></span>
                        <h3 class="text-sm font-semibold uppercase tracking-wider text-slate-300">Frontend</h3>
                    </div>
                    <div class="flex flex-wrap gap-4">
                        <div class="tech-icon flex items-center gap-2.5 px-4 py-2.5 rounded-xl bg-white/[0.03] border border-white/[0.06]">
                            <span class="iconify text-[#61DAFB]" data-icon="logos:react" data-width="22"></span>
                            <span class="text-sm text-slate-300">React</span>
                        </div>
                        <div class="tech-icon flex items-center gap-2.5 px-4 py-2.5 rounded-xl bg-white/[0.03] border border-white/[0.06]">
                            <span class="iconify text-[#E34F26]" data-icon="logos:html-5" data-width="22"></span>
                            <span class="text-sm text-slate-300">HTML5</span>
                        </div>
                        <div class="tech-icon flex items-center gap-2.5 px-4 py-2.5 rounded-xl bg-white/[0.03] border border-white/[0.06]">
                            <span class="iconify text-[#1572B6]" data-icon="logos:css-3" data-width="22"></span>
                            <span class="text-sm text-slate-300">CSS3</span>
                        </div>
                        <div class="tech-icon flex items-center gap-2.5 px-4 py-2.5 rounded-xl bg-white/[0.03] border border-white/[0.06]">
                            <span class="iconify text-[#06B6D4]" data-icon="logos:tailwindcss-icon" data-width="22"></span>
                            <span class="text-sm text-slate-300">Tailwind CSS</span>
                        </div>
                    </div>
                </div>

                <!-- Backend & DB -->
                <div class="grid md:grid-cols-2 gap-8">
                    <div class="glass-card rounded-2xl p-6 md:p-8">
                        <div class="flex items-center gap-3 mb-5">
                            <span class="iconify text-brand-400" data-icon="lucide:server" data-width="18"></span>
                            <h3 class="text-sm font-semibold uppercase tracking-wider text-slate-300">Backend</h3>
                        </div>
                        <div class="flex flex-wrap gap-4">
                            <div class="tech-icon flex items-center gap-2.5 px-4 py-2.5 rounded-xl bg-white/[0.03] border border-white/[0.06]">
                                <span class="iconify text-[#339933]" data-icon="logos:nodejs-icon" data-width="22"></span>
                                <span class="text-sm text-slate-300">Node.js</span>
                            </div>
                            <div class="tech-icon flex items-center gap-2.5 px-4 py-2.5 rounded-xl bg-white/[0.03] border border-white/[0.06]">
                                <span class="iconify text-[#ffffff]" data-icon="skill-icons:expressjs-light" data-width="22"></span>
                                <span class="text-sm text-slate-300">Express</span>
                            </div>
                        </div>
                    </div>
                    <div class="glass-card rounded-2xl p-6 md:p-8">
                        <div class="flex items-center gap-3 mb-5">
                            <span class="iconify text-brand-400" data-icon="lucide:database" data-width="18"></span>
                            <h3 class="text-sm font-semibold uppercase tracking-wider text-slate-300">Database</h3>
                        </div>
                        <div class="flex flex-wrap gap-4">
                            <div class="tech-icon flex items-center gap-2.5 px-4 py-2.5 rounded-xl bg-white/[0.03] border border-white/[0.06]">
                                <span class="iconify text-[#47A248]" data-icon="logos:mongodb-icon" data-width="22"></span>
                                <span class="text-sm text-slate-300">MongoDB</span>
                            </div>
                            <div class="tech-icon flex items-center gap-2.5 px-4 py-2.5 rounded-xl bg-white/[0.03] border border-white/[0.06]">
                                <span class="iconify text-[#4479A1]" data-icon="logos:mysql-icon" data-width="22"></span>
                                <span class="text-sm text-slate-300">MySQL</span>
                            </div>
                            <div class="tech-icon flex items-center gap-2.5 px-4 py-2.5 rounded-xl bg-white/[0.03] border border-white/[0.06]">
                                <span class="iconify text-[#FFCA28]" data-icon="logos:firebase" data-width="22"></span>
                                <span class="text-sm text-slate-300">Firebase</span>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- AI & Tools -->
                <div class="glass-card rounded-2xl p-6 md:p-8">
                    <div class="flex items-center gap-3 mb-5">
                        <span class="iconify text-brand-400" data-icon="lucide:brain-circuit" data-width="18"></span>
                        <h3 class="text-sm font-semibold uppercase tracking-wider text-slate-300">AI & Tools</h3>
                    </div>
                    <div class="flex flex-wrap gap-4">
                        <div class="tech-icon flex items-center gap-2.5 px-4 py-2.5 rounded-xl bg-white/[0.03] border border-white/[0.06]">
                            <span class="iconify text-[#FF6F00]" data-icon="logos:tensorflow" data-width="22"></span>
                            <span class="text-sm text-slate-300">TensorFlow</span>
                        </div>
                        <div class="tech-icon flex items-center gap-2.5 px-4 py-2.5 rounded-xl bg-white/[0.03] border border-white/[0.06]">
                            <span class="iconify text-[#5C9FD8]" data-icon="logos:opencv" data-width="22"></span>
                            <span class="text-sm text-slate-300">OpenCV</span>
                        </div>
                        <div class="tech-icon flex items-center gap-2.5 px-4 py-2.5 rounded-xl bg-white/[0.03] border border-white/[0.06]">
                            <span class="iconify text-[#F05032]" data-icon="logos:git-icon" data-width="22"></span>
                            <span class="text-sm text-slate-300">Git</span>
                        </div>
                        <div class="tech-icon flex items-center gap-2.5 px-4 py-2.5 rounded-xl bg-white/[0.03] border border-white/[0.06]">
                            <span class="iconify" data-icon="logos:github-icon" data-width="22"></span>
                            <span class="text-sm text-slate-300">GitHub</span>
                        </div>
                        <div class="tech-icon flex items-center gap-2.5 px-4 py-2.5 rounded-xl bg-white/[0.03] border border-white/[0.06]">
                            <span class="iconify text-[#007ACC]" data-icon="logos:visual-studio-code" data-width="22"></span>
                            <span class="text-sm text-slate-300">VS Code</span>
                        </div>
                        <div class="tech-icon flex items-center gap-2.5 px-4 py-2.5 rounded-xl bg-white/[0.03] border border-white/[0.06]">
                            <span class="iconify text-[#FF6C37]" data-icon="logos:postman-icon" data-width="22"></span>
                            <span class="text-sm text-slate-300">Postman</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Projects Section -->
    <section id="projects" class="relative py-24 md:py-32 px-6 section-reveal">
        <div class="max-w-7xl mx-auto">
            <div class="text-center mb-16">
                <div class="flex items-center justify-center gap-3 mb-6">
                    <div class="h-px w-8 bg-brand-500"></div>
                    <span class="text-xs font-semibold uppercase tracking-[0.2em] text-brand-400">Featured Projects</span>
                    <div class="h-px w-8 bg-brand-500"></div>
                </div>
                <h2 class="font-poppins font-bold text-3xl md:text-4xl tracking-tight text-gradient">What I've Built</h2>
            </div>

            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-6">
                <!-- Project 1 - Featured -->
                <div class="project-card glass-card glass-card-hover rounded-2xl p-6 md:col-span-2 lg:col-span-2 lg:row-span-2 relative">
                    <div class="absolute top-4 right-4">
                        <span class="px-3 py-1 rounded-full bg-brand-500/10 border border-brand-500/20 text-brand-400 text-[10px] font-semibold uppercase tracking-wider">Featured</span>
                    </div>
                    <div class="flex items-start gap-4 mb-6">
                        <div class="w-14 h-14 rounded-2xl bg-gradient-to-br from-brand-500/20 to-purple-500/20 border border-brand-500/10 flex items-center justify-center flex-shrink-0">
                            <span class="text-2xl">🤖</span>
                        </div>
                        <div>
                            <h3 class="font-poppins font-bold text-xl text-white mb-1">AgenticLoan AI</h3>
                            <p class="text-sm text-slate-500">AI-powered Loan Approval Platform</p>
                        </div>
                    </div>
                    <p class="text-slate-400 font-light leading-relaxed text-sm mb-6 max-w-xl">
                        End-to-end AI platform that automates loan processing with GPT-powered assistance, voice interface, OCR document extraction, and predictive eligibility analysis.
                    </p>
                    <div class="grid grid-cols-2 sm:grid-cols-3 gap-3 mb-6">
                        <div class="flex items-center gap-2 text-xs text-slate-400">
                            <span class="iconify text-emerald-400" data-icon="lucide:check-circle-2" data-width="13"></span>
                            GPT AI Assistant
                        </div>
                        <div class="flex items-center gap-2 text-xs text-slate-400">
                            <span class="iconify text-emerald-400" data-icon="lucide:check-circle-2" data-width="13"></span>
                            Voice Assistant
                        </div>
                        <div class="flex items-center gap-2 text-xs text-slate-400">
                            <span class="iconify text-emerald-400" data-icon="lucide:check-circle-2" data-width="13"></span>
                            Eligibility Prediction
                        </div>
                        <div class="flex items-center gap-2 text-xs text-slate-400">
                            <span class="iconify text-emerald-400" data-icon="lucide:check-circle-2" data-width="13"></span>
                            OCR Processing
                        </div>
                        <div class="flex items-center gap-2 text-xs text-slate-400">
                            <span class="iconify text-emerald-400" data-icon="lucide:check-circle-2" data-width="13"></span>
                            Admin Dashboard
                        </div>
                        <div class="flex items-center gap-2 text-xs text-slate-400">
                            <span class="iconify text-emerald-400" data-icon="lucide:check-circle-2" data-width="13"></span>
                            Real-time Tracking
                        </div>
                    </div>
                    <div class="flex flex-wrap gap-2">
                        <span class="px-3 py-1 rounded-lg bg-white/[0.04] border border-white/[0.06] text-xs text-slate-400 font-mono">React</span>
                        <span class="px-3 py-1 rounded-lg bg-white/[0.04] border border-white/[0.06] text-xs text-slate-400 font-mono">Node.js</span>
                        <span class="px-3 py-1 rounded-lg bg-white/[0.04] border border-white/[0.06] text-xs text-slate-400 font-mono">MongoDB</span>
                        <span class="px-3 py-1 rounded-lg bg-brand-500/10 border border-brand-500/20 text-xs text-brand-400 font-mono">OpenAI</span>
                        <span class="px-3 py-1 rounded-lg bg-brand-500/10 border border-brand-500/20 text-xs text-brand-400 font-mono">OCR</span>
                    </div>
                </div>

                <!-- Project 2 -->
                <div class="project-card glass-card glass-card-hover rounded-2xl p-6">
                    <div class="w-12 h-12 rounded-2xl bg-gradient-to-br from-amber-500/20 to-red-500/20 border border-amber-500/10 flex items-center justify-center mb-4">
                        <span class="text-xl">🏛</span>
                    </div>
                    <h3 class="font-poppins font-bold text-base text-white mb-1">AI Bureaucracy Engine</h3>
                    <p class="text-xs text-slate-500 mb-4">AI Officer Assistant</p>
                    <div class="space-y-2 mb-4">
                        <div class="flex items-center gap-2 text-xs text-slate-400">
                            <span class="iconify text-emerald-400" data-icon="lucide:check-circle-2" data-width="12"></span>
                            Document Verification
                        </div>
                        <div class="flex items-center gap-2 text-xs text-slate-400">
                            <span class="iconify text-emerald-400" data-icon="lucide:check-circle-2" data-width="12"></span>
                            AI Approval Prediction
                        </div>
                        <div class="flex items-center gap-2 text-xs text-slate-400">
                            <span class="iconify text-emerald-400" data-icon="lucide:check-circle-2" data-width="12"></span>
                            Smart Recommendations
                        </div>
                    </div>
                    <div class="flex flex-wrap gap-1.5">
                        <span class="px-2 py-0.5 rounded bg-white/[0.04] text-[10px] text-slate-500 font-mono">Python</span>
                        <span class="px-2 py-0.5 rounded bg-white/[0.04] text-[10px] text-slate-500 font-mono">AI</span>
                        <span class="px-2 py-0.5 rounded bg-white/[0.04] text-[10px] text-slate-500 font-mono">OCR</span>
                    </div>
                </div>

                <!-- Project 3 -->
                <div class="project-card glass-card glass-card-hover rounded-2xl p-6">
                    <div class="w-12 h-12 rounded-2xl bg-gradient-to-br from-blue-500/20 to-indigo-500/20 border border-blue-500/10 flex items-center justify-center mb-4">
                        <span class="text-xl">🏫</span>
                    </div>
                    <h3 class="font-poppins font-bold text-base text-white mb-1">CampusCare</h3>
                    <p class="text-xs text-slate-500 mb-4">AI Hostel Complaint System</p>
                    <div class="space-y-2 mb-4">
                        <div class="flex items-center gap-2 text-xs text-slate-400">
                            <span class="iconify text-emerald-400" data-icon="lucide:check-circle-2" data-width="12"></span>
                            Complaint Detection
                        </div>
                        <div class="flex items-center gap-2 text-xs text-slate-400">
                            <span class="iconify text-emerald-400" data-icon="lucide:check-circle-2" data-width="12"></span>
                            Duplicate Grouping
                        </div>
                        <div class="flex items-center gap-2 text-xs text-slate-400">
                            <span class="iconify text-emerald-400" data-icon="lucide:check-circle-2" data-width="12"></span>
                            Smart Analytics
                        </div>
                    </div>
                    <div class="flex flex-wrap gap-1.5">
                        <span class="px-2 py-0.5 rounded bg-white/[0.04] text-[10px] text-slate-500 font-mono">MERN</span>
                        <span class="px-2 py-0.5 rounded bg-white/[0.04] text-[10px] text-slate-500 font-mono">NLP</span>
                    </div>
                </div>

                <!-- Project 4 -->
                <div class="project-card glass-card glass-card-hover rounded-2xl p-6">
                    <div class="w-12 h-12 rounded-2xl bg-gradient-to-br from-pink-500/20 to-rose-500/20 border border-pink-500/10 flex items-center justify-center mb-4">
                        <span class="text-xl">🤟</span>
                    </div>
                    <h3 class="font-poppins font-bold text-base text-white mb-1">UniComm AI</h3>
                    <p class="text-xs text-slate-500 mb-4">Universal Communication Platform</p>
                    <div class="space-y-2 mb-4">
                        <div class="flex items-center gap-2 text-xs text-slate-400">
                            <span class="iconify text-emerald-400" data-icon="lucide:check-circle-2" data-width="12"></span>
                            Sign Language Recognition
                        </div>
                        <div class="flex items-center gap-2 text-xs text-slate-400">
                            <span class="iconify text-emerald-400" data-icon="lucide:check-circle-2" data-width="12"></span>
                            Speech & Translation
                        </div>
                        <div class="flex items-center gap-2 text-xs text-slate-400">
                            <span class="iconify text-emerald-400" data-icon="lucide:check-circle-2" data-width="12"></span>
                            Computer Vision
                        </div>
                    </div>
                    <div class="flex flex-wrap gap-1.5">
                        <span class="px-2 py-0.5 rounded bg-white/[0.04] text-[10px] text-slate-500 font-mono">Python</span>
                        <span class="px-2 py-0.5 rounded bg-white/[0.04] text-[10px] text-slate-500 font-mono">CV</span>
                        <span class="px-2 py-0.5 rounded bg-white/[0.04] text-[10px] text-slate-500 font-mono">MediaPipe</span>
                    </div>
                </div>

                <!-- Project 5 -->
                <div class="project-card glass-card glass-card-hover rounded-2xl p-6">
                    <div class="w-12 h-12 rounded-2xl bg-gradient-to-br from-green-500/20 to-emerald-500/20 border border-green-500/10 flex items-center justify-center mb-4">
                        <span class="text-xl">⚽</span>
                    </div>
                    <h3 class="font-poppins font-bold text-base text-white mb-1">SEMS</h3>
                    <p class="text-xs text-slate-500 mb-4">Sports Event Management</p>
                    <div class="space-y-2 mb-4">
                        <div class="flex items-center gap-2 text-xs text-slate-400">
                            <span class="iconify text-emerald-400" data-icon="lucide:check-circle-2" data-width="12"></span>
                            QR Verification
                        </div>
                        <div class="flex items-center gap-2 text-xs text-slate-400">
                            <span class="iconify text-emerald-400" data-icon="lucide:check-circle-2" data-width="12"></span>
                            Event Registration
                        </div>
                        <div class="flex items-center gap-2 text-xs text-slate-400">
                            <span class="iconify text-emerald-400" data-icon="lucide:check-circle-2" data-width="12"></span>
                            Admin Dashboard
                        </div>
                    </div>
                    <div class="flex flex-wrap gap-1.5">
                        <span class="px-2 py-0.5 rounded bg-white/[0.04] text-[10px] text-slate-500 font-mono">MERN</span>
                        <span class="px-2 py-0.5 rounded bg-white/[0.04] text-[10px] text-slate-500 font-mono">QR</span>
                    </div>
                </div>

                <!-- Project 6 -->
                <div class="project-card glass-card glass-card-hover rounded-2xl p-6">
                    <div class="w-12 h-12 rounded-2xl bg-gradient-to-br from-violet-500/20 to-purple-500/20 border border-violet-500/10 flex items-center justify-center mb-4">
                        <span class="text-xl">🎤</span>
                    </div>
                    <h3 class="font-poppins font-bold text-base text-white mb-1">Abbu Assistant</h3>
                    <p class="text-xs text-slate-500 mb-4">AI Voice Assistant</p>
                    <div class="space-y-2 mb-4">
                        <div class="flex items-center gap-2 text-xs text-slate-400">
                            <span class="iconify text-emerald-400" data-icon="lucide:check-circle-2" data-width="12"></span>
                            Speech Recognition
                        </div>
                        <div class="flex items-center gap-2 text-xs text-slate-400">
                            <span class="iconify text-emerald-400" data-icon="lucide:check-circle-2" data-width="12"></span>
                            Voice Commands
                        </div>
                        <div class="flex items-center gap-2 text-xs text-slate-400">
                            <span class="iconify text-emerald-400" data-icon="lucide:check-circle-2" data-width="12"></span>
                            Google Integration
                        </div>
                    </div>
                    <div class="flex flex-wrap gap-1.5">
                        <span class="px-2 py-0.5 rounded bg-white/[0.04] text-[10px] text-slate-500 font-mono">Python</span>
                        <span class="px-2 py-0.5 rounded bg-white/[0.04] text-[10px] text-slate-500 font-mono">NLP</span>
                        <span class="px-2 py-0.5 rounded bg-white/[0.04] text-[10px] text-slate-500 font-mono">API</span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Coding Profiles -->
    <section class="relative py-16 px-6 section-reveal">
        <div class="max-w-5xl mx-auto">
            <div class="text-center mb-12">
                <div class="flex items-center justify-center gap-3 mb-6">
                    <div class="h-px w-8 bg-brand-500"></div>
                    <span class="text-xs font-semibold uppercase tracking-[0.2em] text-brand-400">Coding Profiles</span>
                    <div class="h-px w-8 bg-brand-500"></div>
                </div>
            </div>
            <div class="grid grid-cols-2 md:grid-cols-4 gap-4">
                <div class="stat-card glass-card glass-card-hover rounded-2xl p-6 text-center">
                    <div class="text-2xl mb-2">💛</div>
                    <div class="font-poppins font-bold text-2xl text-white mb-1">230+</div>
                    <div class="text-xs text-slate-500 font-medium">LeetCode Problems</div>
                </div>
                <div class="stat-card glass-card glass-card-hover rounded-2xl p-6 text-center">
                    <div class="text-2xl mb-2">💙</div>
                    <div class="font-poppins font-bold text-2xl text-white mb-1">1120+</div>
                    <div class="text-xs text-slate-500 font-medium">Skillrack Problems</div>
                </div>
                <div class="stat-card glass-card glass-card-hover rounded-2xl p-6 text-center">
                    <div class="text-2xl mb-2">🤎</div>
                    <div class="font-poppins font-bold text-2xl text-white mb-1">300+</div>
                    <div class="text-xs text-slate-500 font-medium">CodeChef Problems</div>
                </div>
                <div class="stat-card glass-card glass-card-hover rounded-2xl p-6 text-center">
                    <div class="text-2xl mb-2">❤️</div>
                    <div class="font-poppins font-bold text-lg text-white mb-1">Certified</div>
                    <div class="text-xs text-slate-500 font-medium">HackerRank PS</div>
                </div>
            </div>
        </div>
    </section>

    <!-- Achievements & Certifications -->
    <section class="relative py-24 md:py-32 px-6 section-reveal">
        <div class="max-w-7xl mx-auto">
            <div class="grid md:grid-cols-2 gap-12 md:gap-16">
                <!-- Achievements -->
                <div>
                    <div class="flex items-center gap-3 mb-8">
                        <div class="h-px w-8 bg-brand-500"></div>
                        <span class="text-xs font-semibold uppercase tracking-[0.2em] text-brand-400">Achievements</span>
                    </div>
                    <div class="space-y-4">
                        <div class="trophy-card glass-card rounded-xl p-4 flex items-center gap-4">
                            <div class="w-10 h-10 rounded-xl bg-gradient-to-br from-slate-400/20 to-slate-600/20 flex items-center justify-center flex-shrink-0 text-lg">🥈</div>
                            <div>
                                <div class="text-sm font-semibold text-white">Runner-Up — Ripple Room</div>
                                <div class="text-xs text-slate-500">PSG Tech Hackathon</div>
                            </div>
                        </div>
                        <div class="trophy-card glass-card rounded-xl p-4 flex items-center gap-4">
                            <div class="w-10 h-10 rounded-xl bg-gradient-to-br from-amber-400/20 to-amber-600/20 flex items-center justify-center flex-shrink-0 text-lg">🏅</div>
                            <div>
                                <div class="text-sm font-semibold text-white">2nd Prize — Paper Presentation</div>
                                <div class="text-xs text-slate-500">KPR College</div>
                            </div>
                        </div>
                        <div class="trophy-card glass-card rounded-xl p-4 flex items-center gap-4">
                            <div class="w-10 h-10 rounded-xl bg-gradient-to-br from-brand-400/20 to-brand-600/20 flex items-center justify-center flex-shrink-0">
                                <span class="iconify text-brand-400" data-icon="lucide:trophy" data-width="18"></span>
                            </div>
                            <div>
                                <div class="text-sm font-semibold text-white">Multiple Hackathon Finalist</div>
                                <div class="text-xs text-slate-500">Various Institutions</div>
                            </div>
                        </div>
                        <div class="trophy-card glass-card rounded-xl p-4 flex items-center gap-4">
                            <div class="w-10 h-10 rounded-xl bg-gradient-to-br from-purple-400/20 to-purple-600/20 flex items-center justify-center flex-shrink-0">
                                <span class="iconify text-purple-400" data-icon="lucide:sparkles" data-width="18"></span>
                            </div>
                            <div>
                                <div class="text-sm font-semibold text-white">AI Application & MERN Developer</div>
                                <div class="text-xs text-slate-500">6+ Production Projects</div>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- Certifications -->
                <div>
                    <div class="flex items-center gap-3 mb-8">
                        <div class="h-px w-8 bg-brand-500"></div>
                        <span class="text-xs font-semibold uppercase tracking-[0.2em] text-brand-400">Certifications</span>
                    </div>
                    <div class="grid grid-cols-2 gap-3">
                        <div class="glass-card glass-card-hover rounded-xl p-4 flex items-center gap-3">
                            <span class="iconify text-brand-400 flex-shrink-0" data-icon="lucide:award" data-width="18"></span>
                            <span class="text-xs text-slate-300 font-medium">NPTEL DBMS</span>
                        </div>
                        <div class="glass-card glass-card-hover rounded-xl p-4 flex items-center gap-3">
                            <span class="iconify text-brand-400 flex-shrink-0" data-icon="lucide:award" data-width="18"></span>
                            <span class="text-xs text-slate-300 font-medium">Salesforce Agentforce</span>
                        </div>
                        <div class="glass-card glass-card-hover rounded-xl p-4 flex items-center gap-3">
                            <span class="iconify text-brand-400 flex-shrink-0" data-icon="lucide:award" data-width="18"></span>
                            <span class="text-xs text-slate-300 font-medium">Oracle Java</span>
                        </div>
                        <div class="glass-card glass-card-hover rounded-xl p-4 flex items-center gap-3">
                            <span class="iconify text-brand-400 flex-shrink-0" data-icon="lucide:award" data-width="18"></span>
                            <span class="text-xs text-slate-300 font-medium">MATLAB Onramp</span>
                        </div>
                        <div class="glass-card glass-card-hover rounded-xl p-4 flex items-center gap-3">
                            <span class="iconify text-brand-400 flex-shrink-0" data-icon="lucide:award" data-width="18"></span>
                            <span class="text-xs text-slate-300 font-medium">Robotics & AI</span>
                        </div>
                        <div class="glass-card glass-card-hover rounded-xl p-4 flex items-center gap-3">
                            <span class="iconify text-brand-400 flex-shrink-0" data-icon="lucide:award" data-width="18"></span>
                            <span class="text-xs text-slate-300 font-medium">IIT Bombay C & C++</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- GitHub Stats -->
    <section id="stats" class="relative py-24 md:py-32 px-6 section-reveal">
        <div class="max-w-5xl mx-auto">
            <div class="text-center mb-16">
                <div class="flex items-center justify-center gap-3 mb-6">
                    <div class="h-px w-8 bg-brand-500"></div>
                    <span class="text-xs font-semibold uppercase tracking-[0.2em] text-brand-400">GitHub Analytics</span>
                    <div class="h-px w-8 bg-brand-500"></div>
                </div>
                <h2 class="font-poppins font-bold text-3xl md:text-4xl tracking-tight text-gradient">My Activity</h2>
            </div>

            <div class="grid md:grid-cols-2 gap-6 mb-6">
                <div class="glass-card rounded-2xl p-1 overflow-hidden">
                    <img src="https://github-readme-stats.vercel.app/api?username=abdulkani007&show_icons=true&theme=tokyonight&hide_border=true&bg_color=0a0a0c&title_color=22d3ee&icon_color=22d3ee&text_color=94a3b8" alt="GitHub Stats" class="w-full rounded-xl" loading="lazy">
                </div>
                <div class="glass-card rounded-2xl p-1 overflow-hidden">
                    <img src="https://github-readme-streak-stats.herokuapp.com/?user=abdulkani007&theme=tokyonight&hide_border=true&background=0a0a0c&stroke=1e293b&ring=22d3ee&fire=22d3ee&currStreakLabel=22d3ee" alt="Streak Stats" class="w-full rounded-xl" loading="lazy">
                </div>
            </div>

            <div class="glass-card rounded-2xl p-1 overflow-hidden mb-6">
                <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=abdulkani007&layout=compact&theme=tokyonight&hide_border=true&bg_color=0a0a0c&title_color=22d3ee&text_color=94a3b8" alt="Top Languages" class="w-full rounded-xl" loading="lazy">
            </div>

            <div class="glass-card rounded-2xl p-1 overflow-hidden mb-6">
                <img src="https://github-readme-activity-graph.vercel.app/graph?username=abdulkani007&theme=tokyo-night&hide_border=true&bg_color=0a0a0c&color=22d3ee&line=22d3ee&point=0e7490" alt="Activity Graph" class="w-full rounded-xl" loading="lazy">
            </div>

            <div class="glass-card rounded-2xl p-1 overflow-hidden">
                <img src="https://github-profile-trophy.vercel.app/?username=abdulkani007&theme=algolia&no-frame=true&column=4&margin-w=15" alt="Trophies" class="w-full rounded-xl" loading="lazy">
            </div>
        </div>
    </section>

    <!-- Fun Code Block -->
    <section class="relative py-16 px-6 section-reveal">
        <div class="max-w-3xl mx-auto">
            <div class="code-block glow-cyan">
                <div class="code-header">
                    <div class="code-dot bg-red-500/80"></div>
                    <div class="code-dot bg-yellow-500/80"></div>
                    <div class="code-dot bg-green-500/80"></div>
                    <span class="text-xs text-slate-500 ml-2 font-mono">life.ts</span>
                    <span class="text-[10px] text-slate-600 ml-auto">⚡ always running</span>
                </div>
                <pre class="p-5 text-sm font-mono leading-loose"><code><span class="text-purple-400">while</span> (<span class="text-brand-300">alive</span>) {
    <span class="text-brand-300">eat</span>();     <span class="text-slate-600">// 🍕 fuel up</span>
    <span class="text-brand-300">code</span>();    <span class="text-slate-600">// 💻 build things</span>
    <span class="text-brand-300">learn</span>();   <span class="text-slate-600">// 📚 grow mind</span>
    <span class="text-brand-300">build</span>();   <span class="text-slate-600">// 🚀 ship products</span>
    <span class="text-brand-300">repeat</span>();  <span class="text-slate-600">// 🔁 never stop</span>
}</code></pre>
            </div>
        </div>
    </section>

    <!-- Connect Section -->
    <section id="connect" class="relative py-24 md:py-32 px-6 section-reveal">
        <div class="max-w-3xl mx-auto text-center">
            <div class="flex items-center justify-center gap-3 mb-6">
                <div class="h-px w-8 bg-brand-500"></div>
                <span class="text-xs font-semibold uppercase tracking-[0.2em] text-brand-400">Let's Connect</span>
                <div class="h-px w-8 bg-brand-500"></div>
            </div>
            <h2 class="font-poppins font-bold text-3xl md:text-5xl tracking-tight text-gradient mb-4">Get In Touch</h2>
            <p class="text-slate-400 font-light text-base mb-12 max-w-lg mx-auto">
                Always open to discussing new projects, creative ideas, or opportunities to be part of your vision.
            </p>

            <div class="flex flex-wrap items-center justify-center gap-4">
                <a href="mailto:abdulkani.b2024it@sece.ac.in" class="connect-btn flex items-center gap-3 px-6 py-3.5 rounded-2xl bg-[#EA4335]/10 border border-[#EA4335]/20 text-[#EA4335]">
                    <span class="iconify" data-icon="logos:google-gmail" data-width="20"></span>
                    <span class="text-sm font-medium">Email</span>
                </a>
                <a href="https://www.linkedin.com/in/abdul-kani-b-3b89aa332" target="_blank" class="connect-btn flex items-center gap-3 px-6 py-3.5 rounded-2xl bg-[#0077B5]/10 border border-[#0077B5]/20 text-[#0077B5]">
                    <span class="iconify" data-icon="logos:linkedin-icon" data-width="20"></span>
                    <span class="text-sm font-medium">LinkedIn</span>
                </a>
                <a href="https://dynamic-trifle-5a321e.netlify.app/" target="_blank" class="connect-btn flex items-center gap-3 px-6 py-3.5 rounded-2xl bg-white/[0.06] border border-white/[0.1] text-white">
                    <span class="iconify" data-icon="lucide:globe" data-width="20"></span>
                    <span class="text-sm font-medium">Portfolio</span>
                </a>
                <a href="https://www.instagram.com/ab_naszz___" target="_blank" class="connect-btn flex items-center gap-3 px-6 py-3.5 rounded-2xl bg-[#E4405F]/10 border border-[#E4405F]/20 text-[#E4405F]">
                    <span class="iconify" data-icon="logos:instagram-icon" data-width="20"></span>
                    <span class="text-sm font-medium">Instagram</span>
                </a>
                <a href="https://github.com/abdulkani007" target="_blank" class="connect-btn flex items-center gap-3 px-6 py-3.5 rounded-2xl bg-white/[0.06] border border-white/[0.1] text-white">
                    <span class="iconify" data-icon="lucide:github" data-width="20"></span>
                    <span class="text-sm font-medium">GitHub</span>
                </a>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="relative py-16 px-6 border-t border-white/[0.04]">
        <div class="max-w-5xl mx-auto text-center">
            <p class="text-sm text-slate-600 mb-2">Thanks for visiting my profile ⭐</p>
            <p class="text-xs text-slate-700 italic">"Building AI that solves real-world problems."</p>
        </div>
    </footer>

    <!-- Snake Animation -->
    <div class="py-8 overflow-hidden">
        <img src="https://raw.githubusercontent.com/Platane/snk/output/github-contribution-grid-snake-dark.svg" alt="Snake" class="w-full max-w-5xl mx-auto opacity-60" loading="lazy">
    </div>

    <script>
        // View count animation
        const viewCount = document.getElementById('viewCount');
        let count = 0;
        const target = 1247;
        const duration = 2000;
        const steps = 60;
        const increment = target / steps;
        const stepTime = duration / steps;
        const timer = setInterval(() => {
            count += increment;
            if (count >= target) {
                count = target;
                clearInterval(timer);
            }
            viewCount.textContent = Math.floor(count).toLocaleString();
        }, stepTime);

        // Scroll reveal
        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('visible');
                }
            });
        }, { threshold: 0.1, rootMargin: '0px 0px -50px 0px' });

        document.querySelectorAll('.section-reveal').forEach(el => observer.observe(el));

        // Smooth scroll
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({ behavior: 'smooth', block: 'start' });
                }
            });
        });

        // Copy markdown
        const markdownContent = `<div align="center">

<p>
  <img src="https://capsule-render.vercel.app/api?type=waving&height=200&color=0:0a0a0c,50:0e1a2e,100:0a0a0c&text=ABDUL%20KANI&fontSize=48&fontColor=22d3ee&animation=fadeIn&fontAlignY=38&desc=AI%20Engineer%20|%20Full%20Stack%20Developer%20|%20Hackathon%20Builder&descSize=16&descColor=94a3b8&descAlignY=60" alt="Header"/>
</p>

<p>
  <img src="https://readme-typing-svg.herokuapp.com?font=Inter&weight=600&size=22&pause=1000&color=22d3ee&center=true&vCenter=true&random=false&width=800&lines=Hi+%F0%9F%91%8B+I'm+Abdul+Kani;AI+Engineer+%7C+Full+Stack+Developer;Building+Real-World+AI+Applications;React+%E2%80%A2+Node.js+%E2%80%A2+Python+%E2%80%A2+Java;Always+Learning+Something+New+%F0%9F%9A%80"/>
</p>

<p>
  <img src="https://komarev.com/ghpvc/?username=abdulkani007&style=flat-square&color=22d3ee&label=PROFILE+VIEWS"/>
  <img src="https://img.shields.io/badge/STATUS-AVAILABLE_FOR_OPPORTUNITIES-emerald?style=flat-square"/>
</p>

</div>

---

## 👋 About Me

\`\`\`python
class Developer:
    def __init__(self):
        self.name = "Abdul Kani"
        self.role = "AI Engineer & Full Stack Dev"
        self.education = "B.Tech IT @ Sri Eshwar College of Engineering"
        self.location = "Tamil Nadu, India"
        self.passion = [
            "Agentic AI Applications",
            "Computer Vision Solutions",
            "MERN Stack Projects",
            "Intelligent Automation"
        ]
        self.currently_building = "AI Products"
\`\`\`

**What I Love:** 🤖 AI & ML · 🌐 Full Stack · ⚡ AI Products · 🏆 Hackathons · 📱 UI/UX · ☁️ Cloud

---

## 🧠 Tech Stack

<table>
<tr>
<td><b>Languages</b></td>
<td>
  <img src="https://skillicons.dev/icons?i=python,java,cpp,c,javascript"/>
</td>
</tr>
<tr>
<td><b>Frontend</b></td>
<td>
  <img src="https://skillicons.dev/icons?i=react,html,css,tailwind"/>
</td>
</tr>
<tr>
<td><b>Backend</b></td>
<td>
  <img src="https://skillicons.dev/icons?i=nodejs,express"/>
</td>
</tr>
<tr>
<td><b>Database</b></td>
<td>
  <img src="https://skillicons.dev/icons?i=mongodb,mysql,firebase"/>
</td>
</tr>
<tr>
<td><b>AI / Tools</b></td>
<td>
  <img src="https://skillicons.dev/icons?i=tensorflow,opencv,git,github,vscode,postman"/>
</td>
</tr>
</table>

---

## 🚀 Featured Projects

### 🤖 AgenticLoan AI — *AI-powered Loan Approval Platform*

> GPT-powered AI assistant with voice interface, OCR document processing, eligibility prediction, and real-time status tracking.

\`React\` \`Node.js\` \`MongoDB\` \`OpenAI\` \`OCR\`

### 🏛 AI Bureaucracy Reduction Engine — *AI Officer Assistant*

> Document verification, AI approval prediction, smart recommendations, and process automation.

\`Python\` \`AI\` \`OCR\`

### 🏫 CampusCare — *AI Hostel Complaint System*

> Intelligent complaint detection, duplicate grouping, smart dashboard, and analytics.

\`MERN\` \`NLP\`

### 🤟 UniComm AI — *Universal Communication Platform*

> Sign language recognition, speech recognition, translation, and computer vision.

\`Python\` \`CV\` \`MediaPipe\`

### ⚽ SEMS — *Sports Event Management System*

> QR verification, event registration, admin dashboard, and authentication.

\`MERN\` \`QR\`

### 🎤 Abbu Assistant — *AI Voice Assistant*

> Speech recognition, voice commands, Google integration, and automation.

\`Python\` \`NLP\` \`API\`

---

## 📊 Coding Profiles

| Platform | Problems |
|----------|----------|
| 💛 LeetCode | 230+ |
| 💙 Skillrack | 1120+ |
| 🤎 CodeChef | 300+ |
| ❤️ HackerRank | Problem Solving Certified |

---

## 🏆 Achievements

- 🥈 **Runner-Up** — Ripple Room, PSG Tech
- 🏅 **2nd Prize** — Paper Presentation, KPR College
- 🏆 Multiple Hackathon Finalist
- 🤖 AI Application & MERN Stack Developer
- 🚀 Open Source Learner

---

## 📜 Certifications

- NPTEL DBMS
- Salesforce Agentforce Specialist
- Oracle Java
- MATLAB Onramp
- Robotics & AI
- IIT Bombay C & C++

---

## 📈 GitHub Analytics

<p align="center">
  <img height="170" src="https://github-readme-stats.vercel.app/api?username=abdulkani007&show_icons=true&theme=tokyonight&hide_border=true&bg_color=0a0a0c&title_color=22d3ee&icon_color=22d3ee&text_color=94a3b8"/>
  <img height="170" src="https://github-readme-streak-stats.herokuapp.com/?user=abdulkani007&theme=tokyonight&hide_border=true&background=0a0a0c&stroke=1e293b&ring=22d3ee&fire=22d3ee&currStreakLabel=22d3ee"/>
</p>

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=abdulkani007&layout=compact&theme=tokyonight&hide_border=true&bg_color=0a0a0c&title_color=22d3ee&text_color=94a3b8"/>
</p>

<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=abdulkani007&theme=tokyo-night&hide_border=true&bg_color=0a0a0c&color=22d3ee&line=22d3ee&point=0e7490"/>
</p>

<p align="center">
  <img src="https://github-profile-trophy.vercel.app/?username=abdulkani007&theme=algolia&no-frame=true&column=4&margin-w=15"/>
</p>

---

## ⚡ Fun Fact

\`\`\`typescript
while (alive) {
    eat();    // 🍕 fuel up
    code();   // 💻 build things
    learn();  // 📚 grow mind
    build();  // 🚀 ship products
    repeat(); // 🔁 never stop
}
\`\`\`

---

## 🌐 Connect With Me

<p align="center">
  <a href="mailto:abdulkani.b2024it@sece.ac.in"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white"/></a>
  <a href="https://www.linkedin.com/in/abdul-kani-b-3b89aa332"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"/></a>
  <a href="https://dynamic-trifle-5a321e.netlify.app/"><img src="https://img.shields.io/badge/Portfolio-000000?style=for-the-badge&logo=firefox-browser&logoColor=white"/></a>
  <a href="https://www.instagram.com/ab_naszz___"><img src="https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white"/></a>
  <a href="https://github.com/abdulkani007"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white"/></a>
</p>

---

<div align="center">

⭐ Thanks for visiting my profile!

*"Building AI that solves real-world problems."*

<img src="https://capsule-render.vercel.app/api?type=waving&height=80&color=0:0a0a0c,50:0e1a2e,100:0a0a0c&section=footer"/>

</div>`;

        document.getElementById('copyMdBtn').addEventListener('click', () => {
            navigator.clipboard.writeText(markdownContent).then(() => {
                const toast = document.getElementById('toast');
                toast.style.opacity = '1';
                toast.style.transform = 'translateX(0)';
                toast.style.pointerEvents = 'auto';
                setTimeout(() => {
                    toast.style.opacity = '0';
                    toast.style.transform = 'translateX(8px)';
                    toast.style.pointerEvents = 'none';
                }, 3000);
            });
        });

        // Nav background on scroll
        const nav = document.querySelector('nav');
        window.addEventListener('scroll', () => {
            if (window.scrollY > 50) {
                nav.style.borderBottomColor = 'rgba(255,255,255,0.08)';
            } else {
                nav.style.borderBottomColor = 'rgba(255,255,255,0.05)';
            }
        });
    </script>
</body>
</html>
