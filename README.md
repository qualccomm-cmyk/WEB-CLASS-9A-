<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>BEST CLASS 9.A - SMP PGRI KLAPANUNGGAL</title>
    <!-- Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@700;800;900&family=Space+Grotesk:wght@600;700&display=swap" rel="stylesheet">

    <style>
        /* === RESET & VARIABLE SYSTEM === */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            -webkit-tap-highlight-color: transparent;
        }

        :root {
            --bg-color: #f7f5ee;
            --main-yellow: #ffde59;
            --main-green: #00e676;
            --main-cyan: #00f0ff;
            --main-pink: #ff3366;
            --dark-border: #121212;
            --card-bg: #ffffff;
            --shadow-hard: 5px 5px 0px var(--dark-border);
            --shadow-hard-lg: 8px 8px 0px var(--dark-border);
        }

        body {
            font-family: 'Space Grotesk', 'Plus Jakarta Sans', sans-serif;
            background-color: var(--bg-color);
            color: var(--dark-border);
            overflow-x: hidden;
            width: 100%;
            min-height: 100vh;
            padding-bottom: 40px;
        }

        /* === ANIMATED GRID ART BACKGROUND === */
        .grid-bg {
            position: fixed;
            top: 0;
            left: 0;
            width: 100vw;
            height: 100vh;
            background-size: 32px 32px;
            background-image: 
                linear-gradient(to right, rgba(18, 18, 18, 0.07) 2px, transparent 2px),
                linear-gradient(to bottom, rgba(18, 18, 18, 0.07) 2px, transparent 2px);
            animation: gridMove 12s linear infinite;
            z-index: -1;
            pointer-events: none;
        }

        @keyframes gridMove {
            0% { background-position: 0 0; }
            100% { background-position: 32px 32px; }
        }

        /* === LAYOUT CONTAINER === */
        .app-container {
            width: 100%;
            max-width: 480px;
            margin: 0 auto;
            padding: 16px;
        }

        /* === NAVBAR UTAMA === */
        .navbar {
            display: flex;
            align-items: center;
            justify-content: space-between;
            background: var(--card-bg);
            border: 3.5px solid var(--dark-border);
            border-radius: 20px;
            padding: 10px 14px;
            box-shadow: var(--shadow-hard);
            margin-bottom: 20px;
            position: sticky;
            top: 10px;
            z-index: 100;
        }

        /* BINGKAI POJOK KIRI ATAS (PROFIL 9AKELAS.JPG) */
        .profile-frame-futuristic {
            position: relative;
            width: 52px;
            height: 52px;
            border-radius: 50%;
            border: 3.5px solid var(--dark-border);
            background: var(--main-cyan);
            box-shadow: 3px 3px 0px var(--dark-border);
            padding: 3px;
            flex-shrink: 0;
        }

        .profile-frame-futuristic img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            border-radius: 50%;
            display: block;
        }

        .profile-badge-dot {
            position: absolute;
            bottom: -2px;
            right: -2px;
            width: 16px;
            height: 16px;
            background: var(--main-green);
            border: 2px solid var(--dark-border);
            border-radius: 50%;
        }

        .nav-title-group {
            display: flex;
            flex-direction: column;
            justify-content: center;
            margin-left: 10px;
            flex-grow: 1;
        }

        .nav-badge {
            background: var(--main-yellow);
            border: 2px solid var(--dark-border);
            padding: 2px 8px;
            border-radius: 10px;
            font-size: 10px;
            font-weight: 900;
            width: fit-content;
            text-transform: uppercase;
            box-shadow: 2px 2px 0px var(--dark-border);
        }

        .nav-school {
            font-size: 13px;
            font-weight: 800;
            margin-top: 2px;
            line-height: 1.1;
        }

        .nav-btn-menu {
            width: 42px;
            height: 42px;
            background: var(--main-pink);
            border: 3px solid var(--dark-border);
            border-radius: 12px;
            box-shadow: 2.5px 2.5px 0px var(--dark-border);
            display: flex;
            align-items: center;
            justify-content: center;
            cursor: pointer;
            transition: transform 0.1s;
        }

        .nav-btn-menu:active {
            transform: translate(2px, 2px);
            box-shadow: 0px 0px 0px var(--dark-border);
        }

        /* CUSTOM SVG ICON */
        .svg-icon {
            width: 22px;
            height: 22px;
            fill: none;
            stroke: var(--dark-border);
            stroke-width: 3;
            stroke-linecap: round;
            stroke-linejoin: round;
        }

        /* === DASHBOARD HERO SECTION === */
        .hero-section {
            background: var(--card-bg);
            border: 3.5px solid var(--dark-border);
            border-radius: 24px;
            padding: 18px;
            box-shadow: var(--shadow-hard-lg);
            margin-bottom: 24px;
            position: relative;
            overflow: hidden;
        }

        .hero-tag-pill {
            display: inline-block;
            background: var(--main-green);
            border: 2.5px solid var(--dark-border);
            padding: 4px 12px;
            border-radius: 50px;
            font-size: 12px;
            font-weight: 800;
            box-shadow: 3px 3px 0px var(--dark-border);
            margin-bottom: 14px;
        }

        /* STYLING FOTO SETENGAH MIRING MODERN DENGAN 22 FOTO & WATERMARK */
        .hero-media-wrapper {
            width: 100%;
            margin: 8px 0 16px 0;
            perspective: 1000px;
        }

        .hero-photo-frame {
            width: 100%;
            height: 210px;
            border: 3.5px solid var(--dark-border);
            border-radius: 18px;
            overflow: hidden;
            background: var(--main-cyan);
            box-shadow: 6px 6px 0px var(--main-pink);
            transform: rotate(-2.5deg) scale(0.98);
            transition: all 0.3s ease;
            position: relative;
        }

        .hero-photo-frame:hover {
            transform: rotate(0deg) scale(1);
        }

        .hero-watermark-badge {
            position: absolute;
            top: 10px;
            left: 10px;
            background: var(--main-yellow);
            border: 2px solid var(--dark-border);
            padding: 3px 8px;
            border-radius: 6px;
            font-size: 10px;
            font-weight: 900;
            text-transform: uppercase;
            box-shadow: 2px 2px 0px var(--dark-border);
            z-index: 20;
            letter-spacing: 0.5px;
            font-family: 'Space Grotesk', sans-serif;
        }

        .hero-slider-track {
            display: flex;
            width: 100%;
            height: 100%;
            transition: transform 0.5s ease-in-out;
        }

        .hero-slider-track img {
            flex: 0 0 100%;
            width: 100%;
            height: 100%;
            object-fit: cover;
            display: block;
        }

        .hero-title {
            font-size: 26px;
            font-weight: 900;
            line-height: 1.1;
            margin-bottom: 8px;
            text-transform: uppercase;
            letter-spacing: -0.5px;
        }

        .hero-desc {
            font-size: 13.5px;
            font-weight: 600;
            color: #333;
            line-height: 1.45;
        }

        /* === SLIDER INFORMASI === */
        .slider-container {
            width: 100%;
            overflow: hidden;
            border: 3.5px solid var(--dark-border);
            border-radius: 20px;
            box-shadow: var(--shadow-hard);
            margin-bottom: 24px;
            position: relative;
            background: var(--card-bg);
            cursor: grab;
        }

        .slider-track {
            display: flex;
            width: 100%;
            transition: transform 0.5s cubic-bezier(0.25, 1, 0.5, 1);
        }

        .slide {
            flex: 0 0 100%;
            padding: 24px 18px;
            display: flex;
            flex-direction: column;
            justify-content: center;
        }

        .slide h4 {
            font-size: 20px;
            font-weight: 900;
            margin-bottom: 6px;
            text-transform: uppercase;
            line-height: 1.1;
        }

        .slide p {
            font-size: 13.5px;
            font-weight: 600;
        }

        .slider-indicators {
            position: absolute;
            bottom: 12px;
            left: 50%;
            transform: translateX(-50%);
            display: flex;
            gap: 6px;
        }

        .indicator {
            width: 12px;
            height: 12px;
            border-radius: 50%;
            border: 2px solid var(--dark-border);
            background: #fff;
            transition: all 0.3s ease;
        }

        .indicator.active {
            background: var(--dark-border);
            width: 24px;
            border-radius: 10px;
        }

        /* === MENU QUICK BUTTONS === */
        .menu-grid {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 12px;
            margin-bottom: 24px;
        }

        .btn-card {
            background: var(--card-bg);
            border: 3.5px solid var(--dark-border);
            border-radius: 16px;
            padding: 14px 12px;
            box-shadow: var(--shadow-hard);
            cursor: pointer;
            text-align: left;
            transition: all 0.15s ease;
            display: flex;
            flex-direction: column;
            justify-content: space-between;
            min-height: 95px;
            position: relative;
            text-decoration: none;
            color: inherit;
        }

        .btn-card:active {
            transform: translate(3px, 3px);
            box-shadow: 2px 2px 0px var(--dark-border);
        }

        .bg-yellow { background: var(--main-yellow); }
        .bg-cyan { background: var(--main-cyan); }
        .bg-green { background: var(--main-green); }
        .bg-pink { background: var(--main-pink); color: #fff; }
        .bg-pink .btn-title { color: #fff; }
        .text-white { color: #fff; }

        .btn-badge-icon {
            width: 32px;
            height: 32px;
            border: 2.5px solid var(--dark-border);
            border-radius: 10px;
            background: #fff;
            display: flex;
            align-items: center;
            justify-content: center;
            box-shadow: 2px 2px 0px var(--dark-border);
            margin-bottom: 8px;
        }

        .btn-title {
            font-size: 14px;
            font-weight: 800;
            line-height: 1.2;
            text-transform: uppercase;
        }

        /* === CONTENT SECTIONS === */
        .section-box {
            background: var(--card-bg);
            border: 3.5px solid var(--dark-border);
            border-radius: 20px;
            padding: 18px;
            box-shadow: var(--shadow-hard);
            margin-bottom: 20px;
        }

        .section-header {
            display: flex;
            align-items: center;
            gap: 10px;
            margin-bottom: 14px;
            border-bottom: 3px solid var(--dark-border);
            padding-bottom: 10px;
        }

        .section-header-title {
            font-size: 18px;
            font-weight: 900;
            text-transform: uppercase;
        }

        /* INTERACTIVE INFO CARDS */
        .interactive-card {
            background: #fafafa;
            border: 2.5px solid var(--dark-border);
            border-radius: 14px;
            padding: 12px 14px;
            margin-bottom: 10px;
            box-shadow: 3px 3px 0px var(--dark-border);
            cursor: pointer;
            transition: transform 0.15s, background-color 0.15s;
            display: flex;
            align-items: center;
            justify-content: space-between;
        }

        .interactive-card:active {
            transform: translate(2px, 2px);
            box-shadow: 1px 1px 0px var(--dark-border);
            background: var(--main-yellow);
        }

        .card-info-text h4 {
            font-size: 14px;
            font-weight: 800;
            margin-bottom: 2px;
        }

        .card-info-text p {
            font-size: 12px;
            font-weight: 600;
            color: #555;
        }

        /* === FLOATING ANIMATED MODAL === */
        .modal-overlay {
            position: fixed;
            top: 0;
            left: 0;
            width: 100vw;
            height: 100vh;
            background: rgba(0, 0, 0, 0.6);
            backdrop-filter: blur(4px);
            z-index: 999;
            display: flex;
            align-items: center;
            justify-content: center;
            padding: 20px;
            opacity: 0;
            pointer-events: none;
            transition: opacity 0.25s ease;
        }

        .modal-overlay.active {
            opacity: 1;
            pointer-events: auto;
        }

        .modal-card {
            background: var(--card-bg);
            border: 4px solid var(--dark-border);
            border-radius: 24px;
            padding: 20px;
            width: 100%;
            max-width: 400px;
            box-shadow: 10px 10px 0px var(--dark-border);
            transform: translateY(40px) scale(0.9);
            transition: transform 0.3s cubic-bezier(0.175, 0.885, 0.32, 1.275);
            position: relative;
        }

        .modal-overlay.active .modal-card {
            transform: translateY(0) scale(1);
            animation: floatUpDown 3s ease-in-out infinite alternate;
        }

        @keyframes floatUpDown {
            0% { transform: translateY(0px); }
            100% { transform: translateY(-8px); }
        }

        .modal-close-btn {
            position: absolute;
            top: 14px;
            right: 14px;
            width: 36px;
            height: 36px;
            background: var(--main-pink);
            border: 2.5px solid var(--dark-border);
            border-radius: 10px;
            display: flex;
            align-items: center;
            justify-content: center;
            cursor: pointer;
            box-shadow: 2px 2px 0px var(--dark-border);
        }

        .modal-close-btn:active {
            transform: translate(2px, 2px);
            box-shadow: 0px 0px 0px var(--dark-border);
        }

        .modal-badge {
            display: inline-block;
            background: var(--main-cyan);
            border: 2px solid var(--dark-border);
            padding: 3px 10px;
            border-radius: 8px;
            font-size: 11px;
            font-weight: 800;
            margin-bottom: 10px;
            box-shadow: 2px 2px 0px var(--dark-border);
        }

        .modal-title {
            font-size: 20px;
            font-weight: 900;
            margin-bottom: 10px;
            line-height: 1.2;
        }

        .modal-body {
            font-size: 13.5px;
            line-height: 1.5;
            font-weight: 600;
            color: #222;
            max-height: 250px;
            overflow-y: auto;
        }

        /* === NAVIGATION DRAWER === */
        .drawer-overlay {
            position: fixed;
            top: 0; left: 0; width: 100vw; height: 100vh;
            background: rgba(0, 0, 0, 0.6);
            backdrop-filter: blur(4px);
            z-index: 1000;
            opacity: 0;
            pointer-events: none;
            transition: opacity 0.3s ease;
        }
        .drawer-overlay.active {
            opacity: 1; pointer-events: auto;
        }

        .nav-drawer {
            position: fixed;
            top: 0; right: -100%;
            width: 280px; height: 100vh;
            background: var(--card-bg);
            border-left: 4.5px solid var(--dark-border);
            box-shadow: -10px 0px 0px rgba(18, 18, 18, 0.2);
            z-index: 1001;
            transition: right 0.35s cubic-bezier(0.175, 0.885, 0.32, 1.275);
            display: flex; flex-direction: column;
            padding: 24px 20px;
            overflow-y: auto;
        }
        .nav-drawer.active {
            right: 0;
        }
        .drawer-header {
            display: flex;
            align-items: center;
            justify-content: space-between;
            margin-bottom: 20px;
            border-bottom: 3.5px solid var(--dark-border);
            padding-bottom: 14px;
        }
        .drawer-header h3 {
            font-size: 20px;
            font-weight: 900;
            text-transform: uppercase;
        }
        .drawer-content {
            display: flex;
            flex-direction: column;
            gap: 12px;
        }
        .drawer-link {
            display: block;
            padding: 14px;
            border: 3.5px solid var(--dark-border);
            border-radius: 14px;
            text-decoration: none;
            color: var(--dark-border);
            font-weight: 800;
            font-size: 15px;
            text-transform: uppercase;
            box-shadow: 4px 4px 0px var(--dark-border);
            transition: transform 0.15s, box-shadow 0.15s;
            cursor: pointer;
        }
        .drawer-link:active {
            transform: translate(3px, 3px);
            box-shadow: 1px 1px 0px var(--dark-border);
        }

        /* FOOTER */
        .footer {
            text-align: center;
            padding: 16px;
            font-size: 12px;
            font-weight: 800;
            text-transform: uppercase;
            letter-spacing: 0.5px;
        }

        /* === FLOATING AI BUTTON & MODAL === */
        .ai-floating-btn {
            position: fixed;
            bottom: 24px;
            right: 24px;
            width: 55px;
            height: 55px;
            background: linear-gradient(135deg, var(--main-cyan), var(--main-pink));
            border: 3px solid var(--dark-border);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 28px;
            box-shadow: 4px 4px 0px var(--dark-border);
            cursor: pointer;
            z-index: 999;
            transition: transform 0.2s, box-shadow 0.2s;
            animation: floatAiBtn 3s ease-in-out infinite;
        }

        .ai-floating-btn:active {
            transform: translateY(4px) scale(0.95);
            box-shadow: 0px 0px 0px var(--dark-border);
            animation: none;
        }

        @keyframes floatAiBtn {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-8px); }
        }

        .ai-iframe-overlay {
            position: fixed;
            top: 0; left: 0; width: 100vw; height: 100vh;
            background: rgba(0, 0, 0, 0.7);
            backdrop-filter: blur(5px);
            z-index: 9999;
            display: flex;
            align-items: center;
            justify-content: center;
            opacity: 0;
            pointer-events: none;
            transition: opacity 0.3s ease;
        }

        .ai-iframe-overlay.active {
            opacity: 1;
            pointer-events: auto;
        }

        .ai-iframe-container {
            width: 95%;
            max-width: 1200px;
            height: 90vh;
            background: var(--bg-color);
            border: 4px solid var(--dark-border);
            border-radius: 20px;
            box-shadow: 8px 8px 0px var(--dark-border);
            position: relative;
            display: flex;
            flex-direction: column;
            overflow: hidden;
            transform: scale(0.9);
            transition: transform 0.3s cubic-bezier(0.175, 0.885, 0.32, 1.275);
        }

        .ai-iframe-overlay.active .ai-iframe-container {
            transform: scale(1);
        }

        .ai-iframe-header {
            background: var(--card-bg);
            padding: 12px 16px;
            border-bottom: 3px solid var(--dark-border);
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .ai-iframe-header h3 {
            font-size: 16px;
            font-weight: 900;
            display: flex;
            align-items: center;
            gap: 8px;
            text-transform: uppercase;
        }

        .ai-iframe-content {
            flex: 1;
            width: 100%;
            border: none;
            background: #fff;
        }

        @media (min-width: 768px) {
            .ai-floating-btn { width: 65px; height: 65px; font-size: 32px; bottom: 30px; right: 30px; }
        }
    </style>
</head>
<body>

    <!-- ANIMATED GRID ART BACKGROUND -->
    <div class="grid-bg"></div>

    <div class="app-container">

        <!-- NAVIGATION BAR -->
        <header class="navbar">
            <div class="profile-frame-futuristic" onclick="openModal('Profil 9A', 'Ini adalah foto profil utama Kelas 9.A SMP PGRI Klapanunggal. Tempat berkumpulnya para generasi juara, kreatif, dan beretika!', 'PROFIL KELAS')">
                <img src="9akelas.jpg" alt="Profil 9A" onerror="this.src='https://via.placeholder.com/150/00f0ff/121212?text=9A'">
                <div class="profile-badge-dot"></div>
            </div>

            <div class="nav-title-group">
                <span class="nav-badge">BEST CLASS 9.A</span>
                <span class="nav-school">SMP PGRI KLAPANUNGGAL</span>
            </div>

            <button class="nav-btn-menu" id="quickMenuBtn" onclick="openDrawer()">
                <svg class="svg-icon" viewBox="0 0 24 24">
                    <line x1="4" y1="6" x2="20" y2="6"></line>
                    <line x1="4" y1="12" x2="20" y2="12"></line>
                    <line x1="4" y1="18" x2="20" y2="18"></line>
                </svg>
            </button>
        </header>

        <!-- VIEW 1: BERANDA HOME -->
        <div id="viewHome" class="app-view">
            <!-- DASHBOARD HERO SECTION -->
            <section class="hero-section">
                <span class="hero-tag-pill">Best class 9.A</span>
                
                <!-- FOTO SETENGAH MIRING MODERN DENGAN 22 FOTO & WATERMARK -->
                <div class="hero-media-wrapper">
                    <div class="hero-photo-frame">
                        <div class="hero-watermark-badge">random photo 9a</div>
                        <div class="hero-slider-track" id="heroPhotoTrack">
                            <img src="1.jpg" alt="1.jpg" onerror="this.src='https://via.placeholder.com/400x250/00f0ff/121212?text=1.jpg'">
                            <img src="2.jpg" alt="2.jpg" onerror="this.src='https://via.placeholder.com/400x250/ffde59/121212?text=2.jpg'">
                            <img src="3.jpg" alt="3.jpg" onerror="this.src='https://via.placeholder.com/400x250/00e676/121212?text=3.jpg'">
                            <img src="4.jpg" alt="4.jpg" onerror="this.src='https://via.placeholder.com/400x250/ff3366/121212?text=4.jpg'">
                            <img src="5.jpg" alt="5.jpg" onerror="this.src='https://via.placeholder.com/400x250/00f0ff/121212?text=5.jpg'">
                            <img src="6.jpg" alt="6.jpg" onerror="this.src='https://via.placeholder.com/400x250/ffde59/121212?text=6.jpg'">
                            <img src="7.jpg" alt="7.jpg" onerror="this.src='https://via.placeholder.com/400x250/00e676/121212?text=7.jpg'">
                            <img src="8.jpg" alt="8.jpg" onerror="this.src='https://via.placeholder.com/400x250/ff3366/121212?text=8.jpg'">
                            <img src="9.jpg" alt="9.jpg" onerror="this.src='https://via.placeholder.com/400x250/00f0ff/121212?text=9.jpg'">
                            <img src="10.jpg" alt="10.jpg" onerror="this.src='https://via.placeholder.com/400x250/ffde59/121212?text=10.jpg'">
                            <img src="11.jpg" alt="11.jpg" onerror="this.src='https://via.placeholder.com/400x250/00e676/121212?text=11.jpg'">
                            <img src="12.jpg" alt="12.jpg" onerror="this.src='https://via.placeholder.com/400x250/ff3366/121212?text=12.jpg'">
                            <img src="13.jpg" alt="13.jpg" onerror="this.src='https://via.placeholder.com/400x250/00f0ff/121212?text=13.jpg'">
                            <img src="14.jpg" alt="14.jpg" onerror="this.src='https://via.placeholder.com/400x250/ffde59/121212?text=14.jpg'">
                            <img src="15.jpg" alt="15.jpg" onerror="this.src='https://via.placeholder.com/400x250/00e676/121212?text=15.jpg'">
                            <img src="16.jpg" alt="16.jpg" onerror="this.src='https://via.placeholder.com/400x250/ff3366/121212?text=16.jpg'">
                            <img src="17.jpg" alt="17.jpg" onerror="this.src='https://via.placeholder.com/400x250/00f0ff/121212?text=17.jpg'">
                            <img src="18.jpg" alt="18.jpg" onerror="this.src='https://via.placeholder.com/400x250/ffde59/121212?text=18.jpg'">
                            <img src="19.jpg" alt="19.jpg" onerror="this.src='https://via.placeholder.com/400x250/00e676/121212?text=19.jpg'">
                            <img src="20.jpg" alt="20.jpg" onerror="this.src='https://via.placeholder.com/400x250/ff3366/121212?text=20.jpg'">
                            <img src="21.jpg" alt="21.jpg" onerror="this.src='https://via.placeholder.com/400x250/00f0ff/121212?text=21.jpg'">
                            <img src="22.jpg" alt="22.jpg" onerror="this.src='https://via.placeholder.com/400x250/ffde59/121212?text=22.jpg'">
                        </div>
                    </div>
                </div>

                <h1 class="hero-title">WELCOME TO CLASS 9.A WEB</h1>
                <p class="hero-desc">
                    Pusat informasi resmi kelas **9.A SMP PGRI Klapanunggal**. Tempat berbaurnya semangat belajar, kreativitas tanpa batas, serta kepatuhan terhadap tata tertib sekolah!
                </p>
            </section>

            <!-- AUTO SLIDER INFORMASI -->
            <div class="slider-container">
                <div class="slider-track" id="sliderTrack">
                    <div class="slide bg-cyan">
                        <span class="hero-tag-pill" style="margin-bottom: 10px; width: fit-content;">PRESTASI</span>
                        <h4>BERBAKAT</h4>
                        <p>Raih prestasi, dan bakat,dan gapai cita-cita!</p>
                    </div>
                    <div class="slide bg-yellow">
                        <span class="hero-tag-pill" style="margin-bottom: 10px; width: fit-content; background: var(--main-pink); color: #fff;">KEGIATAN</span>
                        <h4>PIKET KELAS</h4>
                        <p> wajib piket dengan jadwal yang sudah di sesuaikan!,dan mari wujudkan kelas paling bersih!</p>
                    </div>
                    <div class="slide bg-pink text-white">
                        <span class="hero-tag-pill" style="margin-bottom: 10px; width: fit-content; background: var(--main-cyan); color: var(--dark-border);">KATA KATA</span>
                        <h4 class="text-white">HARI INI</h4>
                        <p>Kayu jati di tengah hutan, ditebang tukang bawa ke kota. Tuntutlah ilmu dengan ingatan, agar hidup tidak sengsara!</p>
                    </div>
                </div>
                <div class="slider-indicators" id="sliderIndicators">
                    <span class="indicator active"></span>
                    <span class="indicator"></span>
                    <span class="indicator"></span>
                </div>
            </div>

            <!-- FUNCTIONAL MENU BUTTONS -->
            <div class="menu-grid">
                <a href="#etika" class="btn-card bg-yellow">
                    <div class="btn-badge-icon">
                        <svg class="svg-icon" viewBox="0 0 24 24"><path d="M12 2L2 7l10 5 10-5-10-5zM2 17l10 5 10-5M2 12l10 5 10-5"></path></svg>
                    </div>
                    <div class="btn-title">Etika Belajar</div>
                </a>

                <a href="#tatatertib" class="btn-card bg-cyan">
                    <div class="btn-badge-icon">
                        <svg class="svg-icon" viewBox="0 0 24 24"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"></path><polyline points="14 2 14 8 20 8"></polyline><line x1="16" y1="13" x2="8" y2="13"></line><line x1="16" y1="17" x2="8" y2="17"></line></svg>
                    </div>
                    <div class="btn-title">Tata Tertib</div>
                </a>

                <a href="#pelajaran" class="btn-card bg-green">
                    <div class="btn-badge-icon">
                        <svg class="svg-icon" viewBox="0 0 24 24"><path d="M4 19.5A2.5 2.5 0 0 1 6.5 17H20"></path><path d="M6.5 2H20v20H6.5A2.5 2.5 0 0 1 4 19.5v-15A2.5 2.5 0 0 1 6.5 2z"></path></svg>
                    </div>
                    <div class="btn-title">Pelajaran</div>
                </a>

                <a href="#faq" class="btn-card bg-pink">
                    <div class="btn-badge-icon">
                        <svg class="svg-icon" viewBox="0 0 24 24"><circle cx="12" cy="12" r="10"></circle><path d="M9.09 9a3 3 0 0 1 5.83 1c0 2-3 3-3 3"></path><line x1="12" y1="17" x2="12.01" y2="17"></line></svg>
                    </div>
                    <div class="btn-title">FAQ Kelas</div>
                </a>
            </div>

            <!-- SECTION: ETIKA BELAJAR -->
            <section class="section-box" id="etika">
                <div class="section-header">
                    <svg class="svg-icon" viewBox="0 0 24 24"><path d="M22 11.08V12a10 10 0 1 1-5.93-9.14"></path><polyline points="22 4 12 14.01 9 11.01"></polyline></svg>
                    <h2 class="section-header-title">Etika Belajar 9.A</h2>
                </div>

                <div class="interactive-card" onclick="openModal('Hormat Kepada Guru', 'Selalu menyapa, menggunakan bahasa yang sopan, dan mendengarkan dengan seksama saat guru menjelaskan di depan kelas.', 'ETIKA #1')">
                    <div class="card-info-text">
                        <h4>1. Penghormatan Guru</h4>
                        <p>Sopan santun & memperhatikan penjelasan.</p>
                    </div>
                    <svg class="svg-icon" viewBox="0 0 24 24"><polyline points="9 18 15 12 9 6"></polyline></svg>
                </div>

                <div class="interactive-card" onclick="openModal('Kekompakan & Kerja Sama', 'Dilarang keras melakukan bullying. Kelas 9.A menjunjung tinggi rasa solidaritas, saling membantu saat diskusi kelompok.', 'ETIKA #2')">
                    <div class="card-info-text">
                        <h4>2. Solidaritas Tanpa Bullying</h4>
                        <p>Saling merangkul & merawat persahabatan.</p>
                    </div>
                    <svg class="svg-icon" viewBox="0 0 24 24"><polyline points="9 18 15 12 9 6"></polyline></svg>
                </div>

                <div class="interactive-card" onclick="openModal('Fokus & Aktif', 'Hadir tepat waktu sebelum bel berbunyi, menyiapkan buku pelajaran, dan tidak memotong pembicaraan saat sesi tanya jawab.', 'ETIKA #3')">
                    <div class="card-info-text">
                        <h4>3. Kedisiplinan Belajar</h4>
                        <p>Siap materi & aktif bertanya secara tertib.</p>
                    </div>
                    <svg class="svg-icon" viewBox="0 0 24 24"><polyline points="9 18 15 12 9 6"></polyline></svg>
                </div>
            </section>

            <!-- SECTION: TATA TERTIB SEKOLAH -->
            <section class="section-box" id="tatatertib">
                <div class="section-header">
                    <svg class="svg-icon" viewBox="0 0 24 24"><rect x="3" y="4" width="18" height="18" rx="2" ry="2"></rect><line x1="16" y1="2" x2="16" y2="6"></line><line x1="8" y1="2" x2="8" y2="6"></line><line x1="3" y1="10" x2="21" y2="10"></line></svg>
                    <h2 class="section-header-title">Tata Tertib Sekolah</h2>
                </div>

                <div class="interactive-card" onclick="openModal('Kehadiran Tepat Waktu', 'Siswa wajib hadir di SMP PGRI Klapanunggal sebelum pukul 06.30 WIB. Keterlambatan lebih dari dari jam bel sesudah berbunnyi selama 3 kali terlambat akan mendapatkan pembinaan dari Guru BK.', 'TATA TERTIB')">
                    <div class="card-info-text">
                        <h4>Waktu Masuk & Kehadiran</h4>
                        <p>Maksimal pkl 06.30 WIB di sekolah.</p>
                    </div>
                    <svg class="svg-icon" viewBox="0 0 24 24"><polyline points="9 18 15 12 9 6"></polyline></svg>
                </div>

                <div class="interactive-card" onclick="openModal('Seragam Lengkap & Rapi', 'Senin-Selasa: Putih Biru + Atribut Lengkap. Rabu: Pramuka. Kamis: Batik Sekolah. Jumat: Busana Muslim/Olahraga.', 'SERAGAM')">
                    <div class="card-info-text">
                        <h4>Ketentuan Seragam</h4>
                        <p>Rapi, lengkap dengan atribut & sepatu hitam.</p>
                    </div>
                    <svg class="svg-icon" viewBox="0 0 24 24"><polyline points="9 18 15 12 9 6"></polyline></svg>
                </div>
            </section>

            <!-- SECTION: INFORMASI PELAJARAN -->
            <section class="section-box" id="pelajaran">
                <div class="section-header">
                    <svg class="svg-icon" viewBox="0 0 24 24"><path d="M2 3h6a4 4 0 0 1 4 4v14a3 3 0 0 0-3-3H2z"></path><path d="M22 3h-6a4 4 0 0 0-4 4v14a3 3 0 0 1 3-3h7z"></path></svg>
                    <h2 class="section-header-title">Pelajaran Utama</h2>
                </div>

                <div class="interactive-card" onclick="openModal('Mata Pelajaran Utama 9.A', 'Matematika, Bahasa Indonesia, IPA Terpadu, IPS, Bahasa Inggris,B.sunda,Pendidikan Agama, PPKn, PJOK, serta Seni musik.', 'MATEPEL 9.A')">
                    <div class="card-info-text">
                        <h4>Kurikulum & Mapel 9.A</h4>
                        <p>Fokus persiapan ujian & asesmen akhir.</p>
                    </div>
                    <svg class="svg-icon" viewBox="0 0 24 24"><polyline points="9 18 15 12 9 6"></polyline></svg>
                </div>
            </section>

            <!-- SECTION: FAQ KELAS -->
            <section class="section-box" id="faq">
                <div class="section-header">
                    <svg class="svg-icon" viewBox="0 0 24 24"><path d="M21 15a2 2 0 0 1-2 2H7l-4 4V5a2 2 0 0 1 2-2h14a2 2 0 0 1 2 2z"></path></svg>
                    <h2 class="section-header-title">FAQ Class 9.A</h2>
                </div>

                <div class="interactive-card" onclick="openModal('Siapa Wali Kelas 9.A?', 'Wali kelas 9.A adalah Pembimbing Akademik utama yang selalu mendukung kegiatan belajar dan menjaga keharmonisan murid kelas 9.A yaitu ibu mega.', 'FAQ #1')">
                    <div class="card-info-text">
                        <h4>Siapa Wali Kelas 9.A?</h4>
                        <p>Klik untuk informasi selengkapnya.</p>
                    </div>
                    <svg class="svg-icon" viewBox="0 0 24 24"><polyline points="9 18 15 12 9 6"></polyline></svg>
                </div>

                <div class="interactive-card" onclick="openModal('Bagaimana Sistem Piket Kebersihan?', 'Piket dilaksanakan sesuai jadwal harian. Petugas wajib membersihkan papan tulis, menyapu lantai, dan membuang sampah sebelum bel masuk.', 'FAQ #2')">
                    <div class="card-info-text">
                        <h4>Jadwal & Aturan Piket</h4>
                        <p>Ketentuan kebersihan ruang kelas 9.A.</p>
                    </div>
                    <svg class="svg-icon" viewBox="0 0 24 24"><polyline points="9 18 15 12 9 6"></polyline></svg>
                </div>
            </section>
        </div>

        <!-- VIEW 2: STRUKTUR KELAS (TERPISAH) -->
        <div id="viewStruktur" class="app-view" style="display: none;">
            <div class="section-box">
                <div class="section-header">
                    <svg class="svg-icon" viewBox="0 0 24 24"><path d="M17 21v-2a4 4 0 0 0-4-4H5a4 4 0 0 0-4 4v2"></path><circle cx="9" cy="7" r="4"></circle><path d="M23 21v-2a4 4 0 0 0-3-3.87"></path><path d="M16 3.13a4 4 0 0 1 0 7.75"></path></svg>
                    <h2 class="section-header-title">Struktur Kelas 9.A</h2>
                </div>

                <!-- WALI KELAS -->
                <div style="background: var(--main-yellow); border: 3px solid var(--dark-border); border-radius: 14px; padding: 14px; margin-bottom: 14px; box-shadow: 3px 3px 0px var(--dark-border); text-align: center;">
                    <span class="nav-badge" style="margin: 0 auto 6px auto;">WALI KELAS</span>
                    <h3 style="font-size: 18px; font-weight: 900; text-transform: uppercase;">Ibu Mega Soraya</h3>
                </div>

                <!-- KETUA & WAKIL KETUA KELAS -->
                <div style="display: grid; grid-template-columns: 1fr 1fr; gap: 10px; margin-bottom: 14px;">
                    <div style="background: var(--main-cyan); border: 3px solid var(--dark-border); border-radius: 14px; padding: 12px; box-shadow: 3px 3px 0px var(--dark-border); text-align: center;">
                        <span class="nav-badge" style="font-size: 9px; margin: 0 auto 4px auto;">KETUA KELAS</span>
                        <h4 style="font-size: 15px; font-weight: 900; text-transform: uppercase;">Sharena</h4>
                    </div>
                    <div style="background: var(--main-green); border: 3px solid var(--dark-border); border-radius: 14px; padding: 12px; box-shadow: 3px 3px 0px var(--dark-border); text-align: center;">
                        <span class="nav-badge" style="font-size: 9px; margin: 0 auto 4px auto; background: var(--main-yellow);">WAKIL KETUA</span>
                        <h4 style="font-size: 15px; font-weight: 900; text-transform: uppercase;">Ahsani</h4>
                    </div>
                </div>

                <!-- SEKRETARIS & BENDAHARA -->
                <div style="display: grid; grid-template-columns: 1fr 1fr; gap: 10px; margin-bottom: 20px;">
                    <div style="background: #fff; border: 3px solid var(--dark-border); border-radius: 14px; padding: 12px; box-shadow: 3px 3px 0px var(--dark-border);">
                        <span class="nav-badge" style="font-size: 9px; margin-bottom: 6px; background: var(--main-pink); color: #fff;">SEKRETARIS</span>
                        <p style="font-size: 13px; font-weight: 800; line-height: 1.4;">1. Lulu Fuatsah<br>2. Elisa Putri</p>
                    </div>
                    <div style="background: #fff; border: 3px solid var(--dark-border); border-radius: 14px; padding: 12px; box-shadow: 3px 3px 0px var(--dark-border);">
                        <span class="nav-badge" style="font-size: 9px; margin-bottom: 6px; background: var(--main-yellow);">BENDAHARA</span>
                        <p style="font-size: 13px; font-weight: 800; line-height: 1.4;">1. Natasya Nuraini<br>2. Nuraini</p>
                    </div>
                </div>

                <!-- SEKSI BIDANG HEADER -->
                <div style="background: var(--dark-border); color: #fff; padding: 10px; border-radius: 10px; text-align: center; font-weight: 900; font-size: 15px; text-transform: uppercase; margin-bottom: 14px; box-shadow: 3px 3px 0px var(--main-cyan);">
                    Seksi Bidang
                </div>

                <!-- SEKSI BIDANG GRID -->
                <div style="display: grid; grid-template-columns: repeat(2, 1fr); gap: 10px; margin-bottom: 10px;">
                    <div style="background: var(--main-yellow); border: 2.5px solid var(--dark-border); border-radius: 12px; padding: 10px; box-shadow: 2px 2px 0px var(--dark-border);">
                        <h5 style="font-size: 11px; font-weight: 900; text-transform: uppercase; margin-bottom: 4px;">SIE. KEAMANAN</h5>
                        <p style="font-size: 12px; font-weight: 700;">Davina & M Dika</p>
                    </div>
                    <div style="background: var(--main-cyan); border: 2.5px solid var(--dark-border); border-radius: 12px; padding: 10px; box-shadow: 2px 2px 0px var(--dark-border);">
                        <h5 style="font-size: 11px; font-weight: 900; text-transform: uppercase; margin-bottom: 4px;">SIE. KEBERSIHAN</h5>
                        <p style="font-size: 12px; font-weight: 700;">Anisa & Anin</p>
                    </div>
                </div>
                <div style="display: grid; grid-template-columns: repeat(2, 1fr); gap: 10px; margin-bottom: 10px;">
                    <div style="background: var(--main-green); border: 2.5px solid var(--dark-border); border-radius: 12px; padding: 10px; box-shadow: 2px 2px 0px var(--dark-border);">
                        <h5 style="font-size: 11px; font-weight: 900; text-transform: uppercase; margin-bottom: 4px;">SIE. UPACARA</h5>
                        <p style="font-size: 12px; font-weight: 700;">Kiran & Nanda</p>
                    </div>
                    <div style="background: var(--main-pink); color: #fff; border: 2.5px solid var(--dark-border); border-radius: 12px; padding: 10px; box-shadow: 2px 2px 0px var(--dark-border);">
                        <h5 style="font-size: 11px; font-weight: 900; text-transform: uppercase; margin-bottom: 4px; color: #fff;">SIE. OLAHRAGA</h5>
                        <p style="font-size: 12px; font-weight: 700;">M Risky Pratama & Rico</p>
                    </div>
                </div>
                <div style="display: grid; grid-template-columns: repeat(2, 1fr); gap: 10px;">
                    <div style="background: var(--main-cyan); border: 2.5px solid var(--dark-border); border-radius: 12px; padding: 10px; box-shadow: 2px 2px 0px var(--dark-border);">
                        <h5 style="font-size: 11px; font-weight: 900; text-transform: uppercase; margin-bottom: 4px;">SIE. KEROHANIAN</h5>
                        <p style="font-size: 12px; font-weight: 700;">Azzahra & Dinatiar</p>
                    </div>
                    <div style="background: var(--main-yellow); border: 2.5px solid var(--dark-border); border-radius: 12px; padding: 10px; box-shadow: 2px 2px 0px var(--dark-border);">
                        <h5 style="font-size: 11px; font-weight: 900; text-transform: uppercase; margin-bottom: 4px;">SIE. P3K</h5>
                        <p style="font-size: 12px; font-weight: 700;">Frisca & Diva</p>
                    </div>
                </div>
            </div>
            <div style="text-align: center; margin-top: 16px;">
                <button onclick="switchView('home')" style="background: var(--main-pink); color: #fff; border: 3px solid var(--dark-border); padding: 12px 24px; border-radius: 14px; font-weight: 900; text-transform: uppercase; box-shadow: 4px 4px 0px var(--dark-border); cursor: pointer;">Kembali ke Beranda</button>
            </div>
        </div>

        <!-- VIEW 3: JADWAL PELAJARAN (TERPISAH) -->
        <div id="viewJadwal" class="app-view" style="display: none;">
            <div class="section-box">
                <div class="section-header">
                    <svg class="svg-icon" viewBox="0 0 24 24"><rect x="3" y="4" width="18" height="18" rx="2" ry="2"></rect><line x1="16" y1="2" x2="16" y2="6"></line><line x1="8" y1="2" x2="8" y2="6"></line><line x1="3" y1="10" x2="21" y2="10"></line></svg>
                    <h2 class="section-header-title">Jadwal Pelajaran 9.A</h2>
                </div>

                <div style="background: var(--main-yellow); border: 2.5px solid var(--dark-border); border-radius: 14px; padding: 12px 14px; margin-bottom: 10px; box-shadow: 3px 3px 0px var(--dark-border);">
                    <h4 style="font-size: 15px; font-weight: 900; text-transform: uppercase; margin-bottom: 4px;">SENIN</h4>
                    <p style="font-size: 13px; font-weight: 800; color: #222;">Pend Pancasila, dan IPA</p>
                </div>

                <div style="background: var(--main-cyan); border: 2.5px solid var(--dark-border); border-radius: 14px; padding: 12px 14px; margin-bottom: 10px; box-shadow: 3px 3px 0px var(--dark-border);">
                    <h4 style="font-size: 15px; font-weight: 900; text-transform: uppercase; margin-bottom: 4px;">SELASA</h4>
                    <p style="font-size: 13px; font-weight: 800; color: #222;">B. Indo, B. Inggris, dan IPS</p>
                </div>

                <div style="background: var(--main-green); border: 2.5px solid var(--dark-border); border-radius: 14px; padding: 12px 14px; margin-bottom: 10px; box-shadow: 3px 3px 0px var(--dark-border);">
                    <h4 style="font-size: 15px; font-weight: 900; text-transform: uppercase; margin-bottom: 4px;">RABU</h4>
                    <p style="font-size: 13px; font-weight: 800; color: #222;">PJOK, MTK, IPS</p>
                </div>

                <div style="background: var(--main-pink); color: #fff; border: 2.5px solid var(--dark-border); border-radius: 14px; padding: 12px 14px; margin-bottom: 10px; box-shadow: 3px 3px 0px var(--dark-border);">
                    <h4 style="font-size: 15px; font-weight: 900; text-transform: uppercase; margin-bottom: 4px; color: #fff;">KAMIS</h4>
                    <p style="font-size: 13px; font-weight: 800; color: #fff;">MTK, Seni Musik, B. Sunda</p>
                </div>

                <div style="background: var(--main-cyan); border: 2.5px solid var(--dark-border); border-radius: 14px; padding: 12px 14px; margin-bottom: 10px; box-shadow: 3px 3px 0px var(--dark-border);">
                    <h4 style="font-size: 15px; font-weight: 900; text-transform: uppercase; margin-bottom: 4px;">JUMAT</h4>
                    <p style="font-size: 13px; font-weight: 800; color: #222;">B. Inggris, BK, Informatika, dan PAIBP</p>
                </div>

                <div style="background: var(--main-yellow); border: 2.5px solid var(--dark-border); border-radius: 14px; padding: 12px 14px; margin-bottom: 10px; box-shadow: 3px 3px 0px var(--dark-border);">
                    <h4 style="font-size: 15px; font-weight: 900; text-transform: uppercase; margin-bottom: 4px;">SABTU</h4>
                    <p style="font-size: 13px; font-weight: 800; color: #222;">B. Indo, IPA, PAIBP</p>
                </div>
            </div>
            <div style="text-align: center; margin-top: 16px;">
                <button onclick="switchView('home')" style="background: var(--main-pink); color: #fff; border: 3px solid var(--dark-border); padding: 12px 24px; border-radius: 14px; font-weight: 900; text-transform: uppercase; box-shadow: 4px 4px 0px var(--dark-border); cursor: pointer;">Kembali ke Beranda</button>
            </div>
        </div>

        <footer class="footer">
            &copy; 2026 BEST CLASS 9.A • SMP PGRI KLAPANUNGGAL 
          proram by vlz4you
        </footer>

    </div>

    <!-- SIDEBAR NAVIGATION DRAWER -->
    <div class="drawer-overlay" id="drawerOverlay" onclick="closeDrawer()"></div>
    <div class="nav-drawer" id="navDrawer">
        <div class="drawer-header">
            <h3>Menu Utama</h3>
            <button class="modal-close-btn" style="position: static;" onclick="closeDrawer()">
                <svg class="svg-icon" stroke="#fff" viewBox="0 0 24 24">
                    <line x1="18" y1="6" x2="6" y2="18"></line>
                    <line x1="6" y1="6" x2="18" y2="18"></line>
                </svg>
            </button>
        </div>
        <div class="drawer-content">
            <a class="drawer-link bg-yellow" onclick="switchView('home'); closeDrawer();">Beranda Home</a>
            <a class="drawer-link bg-cyan" onclick="switchView('struktur'); closeDrawer();">Struktur Kelas</a>
            <a class="drawer-link bg-green" onclick="switchView('jadwal'); closeDrawer();">Jadwal Pelajaran</a>
            <a href="#etika" class="drawer-link bg-pink text-white" onclick="switchView('home'); closeDrawer();">Etika Belajar</a>
            <a href="#tatatertib" class="drawer-link bg-yellow" onclick="switchView('home'); closeDrawer();">Tata Tertib</a>
            <a href="#pelajaran" class="drawer-link bg-cyan" onclick="switchView('home'); closeDrawer();">Pelajaran Utama</a>
            <a href="#faq" class="drawer-link bg-green" onclick="switchView('home'); closeDrawer();">FAQ Kelas</a>
        </div>
    </div>

    <!-- FLOATING ANIMATED POPUP MODAL -->
    <div class="modal-overlay" id="modalOverlay">
        <div class="modal-card">
            <button class="modal-close-btn" onclick="closeModal()">
                <svg class="svg-icon" stroke="#fff" viewBox="0 0 24 24">
                    <line x1="18" y1="6" x2="6" y2="18"></line>
                    <line x1="6" y1="6" x2="18" y2="18"></line>
                </svg>
            </button>
            <span class="modal-badge" id="modalBadge">INFO AKADEMIK</span>
            <h3 class="modal-title" id="modalTitle">Judul Informasi</h3>
            <div class="modal-body" id="modalBody">
                Deskripsi detail informasi akan muncul di sini secara dinamis...
            </div>
        </div>
    </div>

    <!-- FLOATING AI BUTTON -->
    <div class="ai-floating-btn" onclick="openAiModal()">AI</div>

    <!-- AI IFRAME OVERLAY -->
    <div class="ai-iframe-overlay" id="aiIframeOverlay">
        <div class="ai-iframe-container">
            <div class="ai-iframe-header">
                <h3>AI Assistant</h3>
                <button class="modal-close-btn" style="position: static;" onclick="closeAiModal()">
                    <svg class="svg-icon" stroke="#fff" viewBox="0 0 24 24" style="width:18px;height:18px;">
                        <line x1="18" y1="6" x2="6" y2="18"></line>
                        <line x1="6" y1="6" x2="18" y2="18"></line>
                    </svg>
                </button>
            </div>
            <iframe src="ClasAi.html" class="ai-iframe-content" id="aiIframe" title="ClasAi File"></iframe>
        </div>
    </div>

    <!-- JAVASCRIPT LOGIC -->
    <script>
        /* === LOGIKA VIEW SWITCHING (BERANDA, STRUKTUR, JADWAL) === */
        function switchView(viewName) {
            document.getElementById('viewHome').style.display = (viewName === 'home') ? 'block' : 'none';
            document.getElementById('viewStruktur').style.display = (viewName === 'struktur') ? 'block' : 'none';
            document.getElementById('viewJadwal').style.display = (viewName === 'jadwal') ? 'block' : 'none';
            window.scrollTo({ top: 0, behavior: 'smooth' });
        }

        /* === LOGIKA SIDEBAR NAV DRAWER === */
        function openDrawer() {
            document.getElementById('drawerOverlay').classList.add('active');
            document.getElementById('navDrawer').classList.add('active');
        }

        function closeDrawer() {
            document.getElementById('drawerOverlay').classList.remove('active');
            document.getElementById('navDrawer').classList.remove('active');
        }

        /* === LOGIKA SLIDER HERO FOTO 22 FOTO OTOMATIS === */
        let currentHeroSlide = 0;
        const totalHeroSlides = 22;
        function moveHeroSlider() {
            currentHeroSlide = (currentHeroSlide + 1) % totalHeroSlides;
            const track = document.getElementById('heroPhotoTrack');
            if(track) {
                track.style.transform = `translateX(-${currentHeroSlide * 100}%)`;
            }
        }
        setInterval(moveHeroSlider, 3000);

        /* === LOGIKA SLIDER INFORMASI === */
        let currentSlide = 0;
        const totalSlides = 3;
        
        function moveSlider() {
            currentSlide = (currentSlide + 1) % totalSlides;
            updateSliderView();
        }

        function updateSliderView() {
            const track = document.getElementById('sliderTrack');
            const indicators = document.querySelectorAll('.indicator');
            if(track) {
                track.style.transform = `translateX(-${currentSlide * 100}%)`;
            }
            indicators.forEach((ind, index) => {
                if(index === currentSlide) {
                    ind.classList.add('active');
                } else {
                    ind.classList.remove('active');
                }
            });
        }
        setInterval(moveSlider, 3500);

        /* === LOGIKA MODAL POPUP === */
        function openModal(title, text, badgeText) {
            const overlay = document.getElementById('modalOverlay');
            const modalTitle = document.getElementById('modalTitle');
            const modalBody = document.getElementById('modalBody');
            const modalBadge = document.getElementById('modalBadge');

            modalTitle.innerText = title;
            modalBody.innerText = text;
            modalBadge.innerText = badgeText || 'INFORMASI 9.A';

            overlay.classList.add('active');
        }

        function closeModal() {
            const overlay = document.getElementById('modalOverlay');
            overlay.classList.remove('active');
        }

        document.getElementById('modalOverlay').addEventListener('click', function(e) {
            if (e.target === this) {
                closeModal();
            }
        });

        /* === LOGIKA AI IFRAME MODAL === */
        function openAiModal() {
            document.getElementById('aiIframeOverlay').classList.add('active');
        }

        function closeAiModal() {
            document.getElementById('aiIframeOverlay').classList.remove('active');
        }

        // Close AI Modal if clicking outside the container
        document.getElementById('aiIframeOverlay').addEventListener('click', function(e) {
            if (e.target === this) {
                closeAiModal();
            }
        });

        /* === LOGIKA SMOOTH SCROLLING === */
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if(target) {
                    setTimeout(() => {
                        target.scrollIntoView({
                            behavior: 'smooth',
                            block: 'start'
                        });
                    }, 200);
                }
            });
        });
    </script>
</body>
</html>
