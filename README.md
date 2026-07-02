<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>TriggerPoint Alpha</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Share+Tech+Mono&family=Urbanist:wght@300;400;700&display=swap" rel="stylesheet">
    
    <style>
        :root {
            --bg-color: #0b0c10;
            --container-bg: #1f2833;
            --primary-glow: #66fcf1;
            --secondary-glow: #45a29e;
            --text-main: #c5c6c7;
            --text-bright: #ffffff;
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        body {
            font-family: 'Urbanist', sans-serif;
            background-color: var(--bg-color);
            color: var(--text-main);
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: space-between;
            align-items: center;
            padding: 2rem 1rem;
            /* Crosshair grid background effect */
            background-image: 
                linear-gradient(rgba(102, 252, 241, 0.03) 1px, transparent 1px),
                linear-gradient(90deg, rgba(102, 252, 241, 0.03) 1px, transparent 1px);
            background-size: 40px 40px;
            background-position: center;
        }

        /* Centered Container Box */
        .main-container {
            background-color: var(--container-bg);
            border: 1px solid rgba(102, 252, 241, 0.2);
            border-radius: 12px;
            padding: 3rem 2rem;
            max-width: 650px;
            width: 100%;
            text-align: center;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.7), 
                        0 0 20px rgba(102, 252, 241, 0.05);
            margin: auto;
            position: relative;
            overflow: hidden;
        }

        /* Decorative Corner Targets */
        .main-container::before {
            content: '';
            position: absolute;
            top: 15px;
            left: 15px;
            width: 10px;
            height: 10px;
            border-top: 2px solid var(--primary-glow);
            border-left: 2px solid var(--primary-glow);
        }

        .main-container::after {
            content: '';
            position: absolute;
            bottom: 15px;
            right: 15px;
            width: 10px;
            height: 10px;
            border-bottom: 2px solid var(--primary-glow);
            border-right: 2px solid var(--primary-glow);
        }

        /* Main Header */
        h1 {
            font-family: 'Share Tech Mono', monospace;
            font-size: 2.5rem;
            color: var(--text-bright);
            margin-bottom: 1.5rem;
            text-transform: uppercase;
            letter-spacing: 2px;
            word-spacing: 4px;
        }

        h1 span {
            color: var(--primary-glow);
            text-shadow: 0 0 10px rgba(102, 252, 241, 0.5);
        }

        /* Project Intro Paragraph */
        p {
            font-size: 1.1rem;
            line-height: 1.7;
            margin-bottom: 2rem;
            color: var(--text-main);
        }

        /* Custom UI Accent Element */
        .hud-status {
            font-family: 'Share Tech Mono', monospace;
            display: inline-block;
            padding: 0.5rem 1.5rem;
            font-size: 0.9rem;
            color: var(--primary-glow);
            border: 1px solid var(--primary-glow);
            background: rgba(102, 252, 241, 0.05);
            border-radius: 4px;
            letter-spacing: 1px;
        }

        /* Footer */
        footer {
            font-size: 0.9rem;
            color: var(--secondary-glow);
            text-align: center;
            letter-spacing: 1px;
            margin-top: 2rem;
        }
    </style>
</head>
<body>

    <div class="main-container">
        <h1>Welcome to <span>TriggerPoint Alpha</span></h1>
        <p>
            This is my master coding hub, serving as the central command center for my shooting game development project. Here, game logic, responsive mechanics, and tactical gameplay architectures are conceptualized, built, and optimized.
        </p>
        <div class="hud-status">SYSTEMS: ENGAGED</div>
    </div>

    <footer>
        Created by Matthew tang in 2026
    </footer>

</body>
</html>
