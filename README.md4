<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>IE421 Project - City's Life Rhythm</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background-color: #000;
            color: #fff;
            overflow-x: hidden;
        }

        /* Navigation Buttons */
        .nav-buttons {
            position: fixed;
            top: 24px;
            right: 24px;
            display: flex;
            gap: 16px;
            z-index: 1000;
        }

        .nav-button {
            padding: 12px 24px;
            background-color: #1a2332;
            color: #fff;
            border: 1px solid #2a3f5f;
            cursor: pointer;
            font-size: 14px;
            font-weight: 300;
            letter-spacing: 1px;
            transition: all 0.3s ease;
            text-decoration: none;
            display: inline-block;
        }

        .nav-button:hover {
            background-color: #2a3f5f;
            transform: translateY(-2px);
        }

        /* Home Page Styles */
        .home-container {
            position: relative;
            width: 100vw;
            height: 100vh;
            overflow: hidden;
        }

        .background {
            position: absolute;
            inset: 0;
            background: linear-gradient(to bottom, #ff9a56 0%, #ffc078 50%, #ffd89b 100%);
        }

        .background::after {
            content: '';
            position: absolute;
            inset: 0;
            background: rgba(0, 0, 0, 0.3);
        }

        /* City Skyline */
        .skyline {
            position: absolute;
            bottom: 0;
            left: 0;
            right: 0;
            height: 60%;
            background: linear-gradient(to top, #1a1a1a 0%, transparent 100%);
        }

        .building {
            position: absolute;
            bottom: 0;
            background: #222;
            box-shadow: inset 0 0 20px rgba(0, 0, 0, 0.5);
        }

        .building:nth-child(1) { left: 5%; width: 80px; height: 400px; background: #1a1a1a; }
        .building:nth-child(2) { left: 12%; width: 100px; height: 450px; background: #222; }
        .building:nth-child(3) { left: 20%; width: 70px; height: 350px; background: #2a2a2a; }
        .building:nth-child(4) { left: 28%; width: 120px; height: 500px; background: #1a1a1a; }
        .building:nth-child(5) { left: 38%; width: 90px; height: 420px; background: #222; }
        .building:nth-child(6) { left: 65%; width: 100px; height: 450px; background: #1a1a1a; }
        .building:nth-child(7) { left: 73%; width: 130px; height: 500px; background: #222; }
        .building:nth-child(8) { left: 83%; width: 95px; height: 400px; background: #2a2a2a; }
        .building:nth-child(9) { left: 90%; width: 85px; height: 350px; background: #222; }

        .main-title {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            font-size: 7rem;
            font-weight: 300;
            letter-spacing: 0.5rem;
            text-shadow: 0 4px 20px rgba(0, 0, 0, 0.5);
            z-index: 10;
        }

        .team-members {
            position: absolute;
            bottom: 32px;
            right: 32px;
            display: flex;
            gap: 24px;
            z-index: 10;
        }

        .team-member {
            font-size: 13px;
            font-weight: 300;
            letter-spacing: 1px;
            text-shadow: 0 2px 10px rgba(0, 0, 0, 0.5);
        }

        /* Content Pages Styles */
        .content-page {
            min-height: 100vh;
            padding: 48px;
        }

        .page-container {
            max-width: 1200px;
            margin: 0 auto;
            margin-top: 96px;
        }

        .page-title {
            font-size: 3rem;
            font-weight: 300;
            letter-spacing: 0.3rem;
            margin-bottom: 64px;
            text-align: center;
        }

        .section {
            background-color: #1a2332;
            border: 1px solid #2a3f5f;
            padding: 32px;
            margin-bottom: 32px;
            min-height: 200px;
        }

        .section-title {
            font-size: 1.5rem;
            font-weight: 300;
            letter-spacing: 0.2rem;
            margin-bottom: 16px;
            padding-bottom: 12px;
            border-bottom: 1px solid #2a3f5f;
        }

        .section-content {
            color: #999;
            font-size: 14px;
            font-style: italic;
            line-height: 1.8;
        }

        /* Visualization Specific Styles */
        .viz-container {
            max-width: 1400px;
        }

        .viz-block {
            background-color: #1a2332;
            border: 1px solid #2a3f5f;
            padding: 32px;
            margin-bottom: 48px;
        }

        .viz-title {
            font-size: 1.5rem;
            font-weight: 300;
            letter-spacing: 0.2rem;
            margin-bottom: 24px;
        }

        .chart-placeholder {
            background-color: #000;
            border: 1px solid #2a3f5f;
            height: 400px;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-bottom: 24px;
        }

        .chart-info {
            color: #666;
            font-size: 16px;
        }

        .explanation-area {
            color: #999;
            min-height: 100px;
            font-size: 14px;
            font-style: italic;
            line-height: 1.8;
        }

        @media (max-width: 768px) {
            .main-title {
                font-size: 3rem;
            }
            .team-members {
                flex-direction: column;
                gap: 12px;
            }
            .nav-buttons {
                flex-direction: column;
                gap: 8px;
            }
        }
    </style>
</head>
<body>
    <!-- HOME PAGE -->
    <div id="homePage" class="home-container">
        <div class="background">
            <div class="skyline">
                <div class="building"></div>
                <div class="building"></div>
                <div class="building"></div>
                <div class="building"></div>
                <div class="building"></div>
                <div class="building"></div>
                <div class="building"></div>
                <div class="building"></div>
                <div class="building"></div>
            </div>
        </div>

        <h1 class="main-title">City's Life Rhythm</h1>

        <div class="nav-buttons">
            <button class="nav-button" onclick="showPage('details')">Project Details</button>
            <button class="nav-button" onclick="showPage('visualizations')">Visualizations</button>
        </div>

        <div class="team-members">
            <div class="team-member">Meryem Öncü</div>
            <div class="team-member">Ahmed Efe Koluaçık</div>
            <div class="team-member">Beyza Altınköprü</div>
            <div class="team-member">Yağmur Kondakcı</div>
            <div class="team-member">Öykü Akdoğan</div>
        </div>
    </div>

    <!-- PROJECT DETAILS PAGE -->
    <div id="detailsPage" class="content-page" style="display: none;">
        <div class="nav-buttons">
            <button class="nav-button" onclick="showPage('home')">Home</button>
            <button class="nav-button" onclick="showPage('details')">Project Details</button>
            <button class="nav-button" onclick="showPage('visualizations')">Visualizations</button>
        </div>

        <div class="page-container">
            <h1 class="page-title">Project Details</h1>

            <div class="section">
                <h2 class="section-title">Project Motivation</h2>
                <div class="section-content">
                    <!-- EMPTY - Add your project motivation text here -->
                </div>
            </div>

            <div class="section">
                <h2 class="section-title">Research Questions</h2>
                <div class="section-content">
                    <!-- EMPTY - Add your research questions here -->
                </div>
            </div>

            <div class="section">
                <h2 class="section-title">Datasets</h2>
                <div class="section-content">
                    <!-- EMPTY - Add your datasets information here -->
                </div>
            </div>

            <div class="section">
                <h2 class="section-title">Methodology</h2>
                <div class="section-content">
                    <!-- EMPTY - Add your methodology description here -->
                </div>
            </div>
        </div>
    </div>

    <!-- VISUALIZATIONS PAGE -->
    <div id="visualizationsPage" class="content-page" style="display: none;">
        <div class="nav-buttons">
            <button class="nav-button" onclick="showPage('home')">Home</button>
            <button class="nav-button" onclick="showPage('details')">Project Details</button>
            <button class="nav-button" onclick="showPage('visualizations')">Visualizations</button>
        </div>

        <div class="page-container viz-container">
            <h1 class="page-title">Visualizations</h1>

            <!-- Daily Rhythm Visualizations -->
            <div class="viz-block">
                <h2 class="viz-title">Daily Rhythm Visualizations</h2>
                <div class="chart-placeholder" id="chart1">
                    <p class="chart-info"><!-- INSERT CHART HERE --></p>
                </div>
                <div class="explanation-area">
                    <!-- EMPTY - Add chart explanation here -->
                </div>
            </div>

            <!-- Transportation & Mobility -->
            <div class="viz-block">
                <h2 class="viz-title">Transportation & Mobility</h2>
                <div class="chart-placeholder" id="chart2">
                    <p class="chart-info"><!-- INSERT CHART HERE --></p>
                </div>
                <div class="explanation-area">
                    <!-- EMPTY - Add chart explanation here -->
                </div>
            </div>

            <!-- Noise & Social Activity -->
            <div class="viz-block">
                <h2 class="viz-title">Noise & Social Activity</h2>
                <div class="chart-placeholder" id="chart3">
                    <p class="chart-info"><!-- INSERT CHART HERE --></p>
                </div>
                <div class="explanation-area">
                    <!-- EMPTY - Add chart explanation here -->
                </div>
            </div>

            <!-- Hot & Cold Zones -->
            <div class="viz-block">
                <h2 class="viz-title">Hot & Cold Zones</h2>
                <div class="chart-placeholder" id="chart4">
                    <p class="chart-info"><!-- INSERT CHART HERE --></p>
                </div>
                <div class="explanation-area">
                    <!-- EMPTY - Add chart explanation here -->
                </div>
            </div>
        </div>
    </div>

    <script>
        // Page Navigation
        function showPage(pageName) {
            // Hide all pages
            document.getElementById('homePage').style.display = 'none';
            document.getElementById('detailsPage').style.display = 'none';
            document.getElementById('visualizationsPage').style.display = 'none';

            // Show selected page
            if (pageName === 'home') {
                document.getElementById('homePage').style.display = 'block';
            } else if (pageName === 'details') {
                document.getElementById('detailsPage').style.display = 'block';
            } else if (pageName === 'visualizations') {
                document.getElementById('visualizationsPage').style.display = 'block';
            }
        }


