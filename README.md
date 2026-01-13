<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>IE421 Project - Home</title>
    <link rel="stylesheet" href="style.css">
</head>
<body class="home-page">
    <div class="background-overlay"></div>

    <!-- Long Boi animation container -->
    <div class="long-boi-track">
        <svg class="long-boi" viewBox="0 0 60 300" xmlns="http://www.w3.org/2000/svg" aria-hidden="true">
            <rect x="20" y="60" width="20" height="190" rx="10" ry="10" fill="#f9f9f9" />
            <circle cx="30" cy="40" r="18" fill="#f9f9f9" />
            <polygon points="38,38 58,44 38,50" fill="#f5c46b" />
            <circle cx="25" cy="35" r="3" fill="#000000" />
            <rect x="16" y="250" width="14" height="8" fill="#f5c46b" />
            <rect x="30" y="250" width="14" height="8" fill="#f5c46b" />
        </svg>
    </div>

    <header class="top-nav">
        <nav class="nav-links">
            <a href="project-details.html" class="nav-button">Project Details</a>
            <a href="visualizations.html" class="nav-button">Visualizations</a>
        </nav>
    </header>

    <main class="home-main">
        <h1 class="site-title">IE421 Project</h1>
    </main>

    <footer class="team-footer">
        <div class="team-container">
            <span class="team-member">Meryem Öncü</span>
            <span class="team-member">Ahmed Efe Koluaçık</span>
            <span class="team-member">Beyza Altınköprü</span>
            <span class="team-member">Yağmur Kondakcı</span>
            <span class="team-member">Öykü Akdoğan</span>
        </div>
    </footer>

    <script src="script.js"></script>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>IE421 Project - Project Details</title>
    <link rel="stylesheet" href="style.css">
</head>
<body class="details-page">
    <header class="top-nav">
        <nav class="nav-links">
            <a href="index.html" class="nav-button">Home</a>
            <a href="project-details.html" class="nav-button nav-button-active">Project Details</a>
            <a href="visualizations.html" class="nav-button">Visualizations</a>
        </nav>
    </header>

    <main class="content-main">
        <section class="content-section">
            <h2 class="section-title">Project Motivation</h2>
            <div class="section-body"></div>
        </section>

        <section class="content-section">
            <h2 class="section-title">Research Questions</h2>
            <div class="section-body"></div>
        </section>

        <section class="content-section">
            <h2 class="section-title">Datasets</h2>
            <div class="section-body"></div>
        </section>

        <section class="content-section">
            <h2 class="section-title">Methodology</h2>
            <div class="section-body"></div>
        </section>
    </main>

    <script src="script.js"></script>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>IE421 Project - Visualizations</title>
    <link rel="stylesheet" href="style.css">
</head>
<body class="visualizations-page">
    <header class="top-nav">
        <nav class="nav-links">
            <a href="index.html" class="nav-button">Home</a>
            <a href="project-details.html" class="nav-button">Project Details</a>
            <a href="visualizations.html" class="nav-button nav-button-active">Visualizations</a>
        </nav>
    </header>

    <main class="visualizations-main">
        <section class="viz-block">
            <h2 class="viz-title">Daily Rhythm Visualizations</h2>
            <div class="viz-chart-placeholder"></div>
            <div class="viz-text-placeholder"></div>
        </section>

        <section class="viz-block">
            <h2 class="viz-title">Transportation &amp; Mobility</h2>
            <div class="viz-chart-placeholder"></div>
            <div class="viz-text-placeholder"></div>
        </section>

        <section class="viz-block">
            <h2 class="viz-title">Noise &amp; Social Activity</h2>
            <div class="viz-chart-placeholder"></div>
            <div class="viz-text-placeholder"></div>
        </section>

        <section class="viz-block">
            <h2 class="viz-title">Hot &amp; Cold Zones</h2>
            <div class="viz-chart-placeholder"></div>
            <div class="viz-text-placeholder"></div>
        </section>
    </main>

    <script src="script.js"></script>
</body>
</html>
:root {
    --bg-black: #000000;
    --navy-frame: #050b1a;
    --navy-surface: #0b1020;
    --accent-gold: #f5c46b;
    --accent-blue: #5ea4ff;
    --text-primary: #ffffff;
    --text-muted: #b6c1d6;
    --border-subtle: rgba(255, 255, 255, 0.08);
    --shadow-soft: 0 24px 80px rgba(0, 0, 0, 0.85);
    --radius-large: 18px;
    --transition-fast: 0.2s ease-out;
    --transition-med: 0.35s ease-out;
    --font-sans: system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen, Ubuntu, Cantarell, "Open Sans", "Helvetica Neue", sans-serif;
}

*,
*::before,
*::after {
    box-sizing: border-box;
}

html,
body {
    margin: 0;
    padding: 0;
    height: 100%;
}

body {
    font-family: var(--font-sans);
    background-color: var(--bg-black);
    color: var(--text-primary);
    -webkit-font-smoothing: antialiased;
}

a {
    color: inherit;
    text-decoration: none;
}

main {
    padding: 96px 7vw 72px;
}

.top-nav {
    position: fixed;
    top: 24px;
    right: 32px;
    z-index: 20;
}

.nav-links {
    display: flex;
    gap: 12px;
}

.nav-button {
    padding: 10px 20px;
    border-radius: 999px;
    border: 1px solid rgba(255, 255, 255, 0.28);
    background: radial-gradient(circle at top left, #1a2440, #050814);
    color: var(--text-primary);
    font-size: 0.9rem;
    letter-spacing: 0.06em;
    text-transform: uppercase;
    font-weight: 600;
    display: inline-flex;
    align-items: center;
    justify-content: center;
    cursor: pointer;
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.75);
    transition: background var(--transition-fast), border-color var(--transition-fast), transform var(--transition-fast), box-shadow var(--transition-fast), color var(--transition-fast);
}

.nav-button:hover {
    background: radial-gradient(circle at top left, #22325c, #050814);
    border-color: var(--accent-gold);
    transform: translateY(-2px);
    box-shadow: 0 18px 40px rgba(0, 0, 0, 0.9);
    color: #ffffff;
}

.nav-button-active {
    background: linear-gradient(135deg, var(--accent-gold), #ffdc9b);
    color: #151518;
    border-color: transparent;
}

.home-page {
    position: relative;
    min-height: 100vh;
    overflow: hidden;
    color: #ffffff;
}

.home-page::before {
    content: "";
    position: fixed;
    inset: 0;
    background-image: url("assets/nyc-home.jpg");
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
    opacity: 0.9;
    z-index: -2;
}

.background-overlay {
    position: fixed;
    inset: 0;
    background: radial-gradient(circle at top, rgba(15, 23, 42, 0.85), rgba(0, 0, 0, 0.95));
    mix-blend-mode: multiply;
    z-index: -1;
}

.long-boi-track {
    position: fixed;
    inset: 0;
    display: flex;
    align-items: flex-end;
    pointer-events: none;
    z-index: 5;
    overflow: hidden;
}

.long-boi {
    height: 80vh;
    max-height: 640px;
    min-height: 420px;
    filter: drop-shadow(0 24px 60px rgba(0, 0, 0, 0.95));
    animation: longBoiWalk 22s linear infinite;
    opacity: 0.96;
}

@keyframes longBoiWalk {
    0% {
        transform: translateX(-120%);
    }
    100% {
        transform: translateX(220%);
    }
}

.home-main {
    position: relative;
    min-height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
    pointer-events: none;
}

.site-title {
    font-size: clamp(3.2rem, 4.6vw, 4.8rem);
    letter-spacing: 0.4em;
    text-transform: uppercase;
    font-weight: 700;
    padding: 22px 36px;
    border-radius: 999px;
    border: 1px solid rgba(255, 255, 255, 0.25);
    background: radial-gradient(circle at top, rgba(15, 23, 42, 0.95), rgba(12, 10, 25, 0.96));
    box-shadow: 0 24px 80px rgba(0, 0, 0, 0.95);
    backdrop-filter: blur(18px);
    color: #fdfdfd;
    pointer-events: auto;
}

.team-footer {
    position: fixed;
    right: 32px;
    bottom: 28px;
    z-index: 10;
}

.team-container {
    display: flex;
    gap: 12px;
    padding: 10px 18px;
    border-radius: 999px;
    background: radial-gradient(circle at top left, rgba(15, 23, 42, 0.98), rgba(6, 10, 22, 0.98));
    border: 1px solid rgba(255, 255, 255, 0.16);
    box-shadow: 0 18px 60px rgba(0, 0, 0, 0.9);
    backdrop-filter: blur(16px);
}

.team-member {
    font-size: 0.8rem;
    color: var(--text-muted);
    white-space: nowrap;
}

.details-page {
    background-color: var(--bg-black);
    color: var(--text-primary);
}

.content-main {
    max-width: 1100px;
    margin: 0 auto;
    display: flex;
    flex-direction: column;
    gap: 28px;
}

.content-section {
    background: radial-gradient(circle at top left, #111829, var(--navy-frame));
    border-radius: var(--radius-large);
    padding: 22px 26px 24px;
    border: 1px solid var(--border-subtle);
    box-shadow: var(--shadow-soft);
    position: relative;
    overflow: hidden;
}

.content-section::before {
    content: "";
    position: absolute;
    inset: 0;
    background: radial-gradient(circle at top right, rgba(94, 164, 255, 0.18), transparent 55%);
    opacity: 0;
    transition: opacity var(--transition-med);
    pointer-events: none;
}

.content-section:hover::before {
    opacity: 1;
}

.section-title {
    margin: 0 0 14px;
    font-size: 1.1rem;
    text-transform: uppercase;
    letter-spacing: 0.16em;
    color: var(--accent-blue);
}

.section-body {
    min-height: 100px;
    border-radius: 12px;
    border: 1px dashed rgba(255, 255, 255, 0.2);
    background-color: rgba(4, 7, 18, 0.8);
    transition: border-color var(--transition-fast), background-color var(--transition-fast), transform var(--transition-fast);
}

.content-section:hover .section-body {
    border-color: rgba(245, 196, 107, 0.7);
    background-color: rgba(8, 12, 30, 0.96);
    transform: translateY(-1px);
}

.visualizations-page {
    background-color: var(--bg-black);
    color: var(--text-primary);
}

.visualizations-main {
    max-width: 1300px;
    margin: 0 auto;
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
    gap: 24px;
}

.viz-block {
    background: radial-gradient(circle at top left, #121b32, var(--navy-surface));
    border-radius: var(--radius-large);
    padding: 18px 20px 20px;
    border: 1px solid var(--border-subtle);
    box-shadow: var(--shadow-soft);
    display: flex;
    flex-direction: column;
    gap: 14px;
    position: relative;
    overflow: hidden;
}

.viz-block::after {
    content: "";
    position: absolute;
    inset: 0;
    background: radial-gradient(circle at bottom, rgba(245, 196, 107, 0.15), transparent 50%);
    mix-blend-mode: screen;
    opacity: 0;
    transition: opacity var(--transition-med);
    pointer-events: none;
}

.viz-block:hover::after {
    opacity: 1;
}

.viz-title {
    margin: 0;
    font-size: 1rem;
    text-transform: uppercase;
    letter-spacing: 0.18em;
    color: var(--accent-gold);
}

.viz-chart-placeholder {
    flex: 1;
    min-height: 180px;
    border-radius: 14px;
    border: 1px dashed rgba(255, 255, 255, 0.35);
    background: repeating-linear-gradient(135deg, rgba(255, 255, 255, 0.04), rgba(255, 255, 255, 0.04) 10px, rgba(255, 255, 255, 0.02) 10px, rgba(255, 255, 255, 0.02) 20px), radial-gradient(circle at top left, rgba(94, 164, 255, 0.18), transparent 60%);
    transition: border-color var(--transition-fast), box-shadow var(--transition-fast), transform var(--transition-fast);
}

.viz-block:hover .viz-chart-placeholder {
    border-color: rgba(245, 196, 107, 0.85);
    box-shadow: 0 18px 50px rgba(0, 0, 0, 0.9);
    transform: translateY(-1px);
}

.viz-text-placeholder {
    margin-top: 6px;
    min-height: 70px;
    border-radius: 12px;
    border: 1px dashed rgba(255, 255, 255, 0.22);
    background-color: rgba(4, 7, 18, 0.92);
    transition: border-color var(--transition-fast), background-color var(--transition-fast);
}

.viz-block:hover .viz-text-placeholder {
    border-color: rgba(94, 164, 255, 0.85);
    background-color: rgba(8, 12, 30, 0.98);
}

@media (max-width: 768px) {
    .top-nav {
        top: 18px;
        right: 16px;
    }

    .nav-links {
        gap: 8px;
    }

    .nav-button {
        padding: 8px 14px;
        font-size: 0.75rem;
    }

    main {
        padding: 90px 16px 60px;
    }

    .team-footer {
        right: 16px;
        bottom: 18px;
    }

    .team-container {
        flex-wrap: wrap;
        justify-content: flex-end;
        max-width: min(100vw - 32px, 520px);
    }

    .site-title {
        letter-spacing: 0.26em;
        padding-inline: 24px;
    }

    .long-boi {
        height: 70vh;
    }
}

@media (max-width: 480px) {
    .nav-links {
        flex-direction: column;
        align-items: flex-end;
    }

    .visualizations-main {
        grid-template-columns: 1fr;
    }
}
// Minimal JavaScript file for future enhancements.
// The current layout and animations are implemented purely in CSS.
