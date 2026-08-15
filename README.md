<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Amasha | Software Engineer</title>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;800&display=swap" rel="stylesheet">
    <style>
        :root {
            --bg-color: #050505;
            --text-main: #ffffff;
            --text-muted: #a0a0a0;
            --accent: #ffffff;
            --card-bg: rgba(20, 20, 20, 0.7);
            --card-border: rgba(255, 255, 255, 0.1);
        }

        body {
            font-family: 'Inter', sans-serif;
            margin: 0;
            padding: 0;
            background-color: var(--bg-color);
            color: var(--text-main);
            line-height: 1.6;
            overflow-x: hidden;
            position: relative;
        }

        /* Shiny Background Effect matching the line-art vibe */
        .background-glow {
            position: fixed;
            top: -20%;
            left: -10%;
            width: 50vw;
            height: 50vw;
            background: radial-gradient(circle, rgba(255,255,255,0.05) 0%, rgba(0,0,0,0) 70%);
            border-radius: 50%;
            z-index: -1;
            pointer-events: none;
        }
        
        .background-glow-2 {
            position: fixed;
            bottom: -20%;
            right: -10%;
            width: 60vw;
            height: 60vw;
            background: radial-gradient(circle, rgba(255,255,255,0.03) 0%, rgba(0,0,0,0) 70%);
            border-radius: 50%;
            z-index: -1;
            pointer-events: none;
        }

        .container {
            max-width: 900px;
            margin: 0 auto;
            padding: 40px 20px;
            position: relative;
            z-index: 1;
        }

        header {
            text-align: center;
            margin-bottom: 60px;
            animation: fadeInDown 1s ease-out;
        }

        h1 {
            font-size: 3rem;
            font-weight: 800;
            margin-bottom: 10px;
            letter-spacing: 2px;
            text-transform: uppercase;
        }

        .subtitle {
            font-size: 1.2rem;
            color: var(--text-muted);
            font-weight: 300;
        }

        .badges {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 10px;
            margin: 30px 0;
        }

        .badges img {
            border-radius: 4px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.3);
            transition: transform 0.3s ease;
        }

        .badges img:hover {
            transform: translateY(-3px);
        }

        section {
            margin-bottom: 50px;
            animation: fadeInUp 1s ease-out both;
        }

        h2 {
            font-size: 2rem;
            border-bottom: 1px solid var(--card-border);
            padding-bottom: 15px;
            margin-bottom: 30px;
            font-weight: 600;
        }

        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 25px;
        }

        .card {
            background: var(--card-bg);
            border: 1px solid var(--card-border);
            border-radius: 12px;
            padding: 25px;
            backdrop-filter: blur(10px);
            transition: all 0.4s ease;
            display: flex;
            flex-direction: column;
            justify-content: space-between;
        }

        .card:hover {
            transform: translateY(-5px);
            border-color: rgba(255, 255, 255, 0.3);
            box-shadow: 0 10px 30px rgba(0,0,0,0.5), 0 0 20px rgba(255,255,255,0.05);
        }

        .card h3 {
            margin: 0 0 10px 0;
            font-size: 1.3rem;
        }

        .card p {
            color: var(--text-muted);
            font-size: 0.95rem;
            margin-bottom: 20px;
        }

        .tech-stack {
            font-size: 0.85rem;
            color: #d0d0d0;
            font-weight: 600;
            margin-bottom: 20px;
        }

        .btn {
            display: inline-block;
            padding: 10px 20px;
            background: transparent;
            color: var(--text-main);
            text-decoration: none;
            border: 1px solid var(--text-main);
            border-radius: 30px;
            font-size: 0.9rem;
            font-weight: 600;
            text-align: center;
            transition: all 0.3s ease;
            align-self: flex-start;
        }

        .btn:hover {
            background: var(--text-main);
            color: var(--bg-color);
            box-shadow: 0 0 15px rgba(255,255,255,0.3);
        }

        .footer {
            text-align: center;
            margin-top: 80px;
            padding-top: 30px;
            border-top: 1px solid var(--card-border);
            color: var(--text-muted);
        }

        .footer a {
            color: var(--text-main);
            text-decoration: none;
            font-weight: 600;
        }

        .footer a:hover {
            text-decoration: underline;
        }

        @keyframes fadeInDown {
            from { opacity: 0; transform: translateY(-30px); }
            to { opacity: 1; transform: translateY(0); }
        }

        @keyframes fadeInUp {
            from { opacity: 0; transform: translateY(30px); }
            to { opacity: 1; transform: translateY(0); }
        }

        @media (max-width: 768px) {
            h1 { font-size: 2.2rem; }
            .grid { grid-template-columns: 1fr; }
        }
    </style>
</head>
<body>

    <div class="background-glow"></div>
    <div class="background-glow-2"></div>

    <div class="container">
        <header>
            <h1>WELCOME</h1>
            <p class="subtitle">Hi there, I'm Amasha! 👋<br>Software Engineering Student | Mobile, Web, IoT & AI</p>
            
            <div class="badges">
                <img src="https://img.shields.io/badge/Kotlin-0095D5?style=for-the-badge&logo=kotlin&logoColor=white" alt="Kotlin">
                <img src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=java&logoColor=white" alt="Java">
                <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python">
                <img src="https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB" alt="React">
                <img src="https://img.shields.io/badge/Laravel-FF2D20?style=for-the-badge&logo=laravel&logoColor=white" alt="Laravel">
                <img src="https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white" alt="TensorFlow">
            </div>
        </header>

        <section style="animation-delay: 0.2s;">
            <h2>📱 Mobile & Application Development</h2>
            <div class="grid">
                <div class="card">
                    <div>
                        <h3>AgriScout: Smart Agriculture System</h3>
                        <p>A mobile application designed to assist farmers with crop health tracking and disease detection, utilizing an offline-first architecture for rural connectivity.</p>
                        <div class="tech-stack">Kotlin • Firebase • Room</div>
                    </div>
                    <a href="https://github.com/AmashaKThenuwara/AgriScout_androidapp" target="_blank" class="btn">View Repository</a>
                </div>
                <div class="card">
                    <div>
                        <h3>PharmaCare: Pharmacy System</h3>
                        <p>A robust Windows desktop application for pharmacies to manage drug inventory, process prescriptions, and handle patient billing securely.</p>
                        <div class="tech-stack">C# • .NET • SQL Server</div>
                    </div>
                    <a href="https://github.com/AmashaKThenuwara/GUI-project" target="_blank" class="btn">View Repository</a>
                </div>
            </div>
        </section>

        <section style="animation-delay: 0.4s;">
            <h2>🌐 Web & E-Commerce</h2>
            <div class="grid">
                <div class="card">
                    <div>
                        <h3>StyleAura: Clothing E-Commerce</h3>
                        <p>A dedicated online retail web application featuring dynamic catalogs, secure authentication, and an admin dashboard.</p>
                        <div class="tech-stack">PHP • Laravel • MySQL</div>
                    </div>
                    <a href="https://github.com/AmashaKThenuwara/Clothing_brand_ecommerce_platform" target="_blank" class="btn">View Repository</a>
                </div>
                <div class="card">
                    <div>
                        <h3>MediaConnect: Media Club Website</h3>
                        <p>The official dynamic web platform for the NIBM Media Club to manage events, registrations, and media galleries.</p>
                        <div class="tech-stack">HTML • CSS • JS • PHP</div>
                    </div>
                    <a href="https://github.com/AmashaKThenuwara/WEB-project" target="_blank" class="btn">View Repository</a>
                </div>
                <div class="card">
                    <div>
                        <h3>TwinTrek: Interactive Memory Game</h3>
                        <p>A fun, responsive browser-based memory matching game utilizing modern CSS features and event-driven JavaScript logic.</p>
                        <div class="tech-stack">JavaScript • HTML5 • CSS3</div>
                    </div>
                    <a href="https://github.com/AmashaKThenuwara/TwinTrek-flip-game" target="_blank" class="btn">View Repository</a>
                </div>
            </div>
        </section>

        <section style="animation-delay: 0.6s;">
            <h2>🤖 Industry 4.0, IoT & Hardware</h2>
            <div class="grid">
                <div class="card">
                    <div>
                        <h3>TexyShield: Factory Safety System</h3>
                        <p>A massive AI-driven safety ecosystem integrating IoT sensors, YOLOv8 computer vision for PPE detection, Blockchain attendance, and AR machine maintenance.</p>
                        <div class="tech-stack">Kotlin • Python • YOLO • ESP32 • AR</div>
                    </div>
                    <a href="https://github.com/AmashaKThenuwara/texyshield" target="_blank" class="btn">View Repository</a>
                </div>
                <div class="card">
                    <div>
                        <h3>SmartLink: IoT Environment Monitor</h3>
                        <p>A hardware-to-cloud IoT system utilizing MQTT to monitor physical environments in real-time and trigger automated responses.</p>
                        <div class="tech-stack">C/C++ • Python • Microcontrollers</div>
                    </div>
                    <a href="https://github.com/AmashaKThenuwara/IoT-project" target="_blank" class="btn">View Repository</a>
                </div>
            </div>
        </section>

        <section style="animation-delay: 0.8s;">
            <h2>📊 Data Science & Analytics</h2>
            <div class="grid">
                <div class="card">
                    <div>
                        <h3>SafeDrive: Accident Prediction App</h3>
                        <p>Machine learning models predicting road accident severity and likelihood based on historical crash data and environmental factors.</p>
                        <div class="tech-stack">Python • Scikit-Learn • TensorFlow</div>
                    </div>
                    <a href="https://github.com/AmashaKThenuwara/ML-project" target="_blank" class="btn">View Repository</a>
                </div>
                <div class="card">
                    <div>
                        <h3>InsightWare: Data Warehousing & BI</h3>
                        <p>An automated ETL and Data Warehousing solution utilizing Star/Snowflake schemas to fuel interactive BI dashboards.</p>
                        <div class="tech-stack">SQL • PowerBI/Tableau</div>
                    </div>
                    <a href="https://github.com/AmashaKThenuwara/DWBI-project" target="_blank" class="btn">View Repository</a>
                </div>
                <div class="card">
                    <div>
                        <h3>StatSense: Statistical Analysis</h3>
                        <p>Mathematical modeling and rigorous hypothesis testing (ANOVA, T-tests, Chi-square) applied to complex datasets.</p>
                        <div class="tech-stack">R • Python • Pandas</div>
                    </div>
                    <a href="https://github.com/AmashaKThenuwara/Statistics-project" target="_blank" class="btn">View Repository</a>
                </div>
            </div>
        </section>

        <section style="animation-delay: 1.0s;">
            <h2>⚙️ Enterprise & Algorithms</h2>
            <div class="grid">
                <div class="card">
                    <div>
                        <h3>StockFlow: Inventory Management</h3>
                        <p>An enterprise-level system tracking stock levels, suppliers, and automating order workflows with strict RBAC.</p>
                        <div class="tech-stack">Java • Spring/Java EE • MySQL</div>
                    </div>
                    <a href="https://github.com/AmashaKThenuwara/EAD-project" target="_blank" class="btn">View Repository</a>
                </div>
                <div class="card">
                    <div>
                        <h3>AlgoSolve: DSA Implementation</h3>
                        <p>A deep-dive repository featuring custom implementations of complex data structures and optimized algorithms.</p>
                        <div class="tech-stack">JS • Java • C++</div>
                    </div>
                    <a href="https://github.com/AmashaKThenuwara/PDSA-project" target="_blank" class="btn">View Repository</a>
                </div>
            </div>
        </section>

        <div class="footer">
            <h3>📫 Let's Connect!</h3>
            <p>
                <a href="https://www.linkedin.com/in/amasha-thenuwara-487765407" target="_blank">LinkedIn Profile</a>
            </p>
            <p style="font-size: 0.8rem; margin-top: 30px;">Generated dynamically with the custom Social Preview graphics featured across my repositories.</p>
        </div>
    </div>
</body>
</html>
