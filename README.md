<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GhostTrack - OSINT Location & Mobile Tracker</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background: linear-gradient(135deg, #0c0c0c 0%, #1a1a2e 50%, #16213e 100%);
            color: #e0e0e0;
            line-height: 1.6;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }
        
        header {
            text-align: center;
            padding: 40px 0;
            background: rgba(10, 10, 10, 0.8);
            border-radius: 10px;
            margin-bottom: 30px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.5);
            border: 1px solid #333;
        }
        
        .logo {
            display: flex;
            align-items: center;
            justify-content: center;
            margin-bottom: 20px;
        }
        
        .logo i {
            font-size: 40px;
            color: #6a11cb;
            margin-right: 15px;
        }
        
        h1 {
            font-size: 3.5rem;
            background: linear-gradient(90deg, #6a11cb 0%, #2575fc 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            text-shadow: 0 0 10px rgba(106, 17, 203, 0.3);
            margin-bottom: 10px;
        }
        
        .tagline {
            font-size: 1.2rem;
            color: #aaa;
            margin-bottom: 20px;
        }
        
        .banner {
            width: 100%;
            border-radius: 10px;
            margin: 20px 0;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
        }
        
        .update-badge {
            display: inline-block;
            background: linear-gradient(90deg, #ff8a00 0%, #da1b60 100%);
            color: white;
            padding: 8px 15px;
            border-radius: 20px;
            font-size: 0.9rem;
            margin: 10px 0;
            box-shadow: 0 0 10px rgba(218, 27, 96, 0.5);
        }
        
        .section {
            background: rgba(15, 15, 15, 0.8);
            border-radius: 10px;
            padding: 25px;
            margin-bottom: 30px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
            border: 1px solid #333;
        }
        
        h2 {
            color: #6a11cb;
            margin-bottom: 20px;
            font-size: 1.8rem;
            display: flex;
            align-items: center;
        }
        
        h2 i {
            margin-right: 10px;
        }
        
        .features {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
            margin-top: 30px;
        }
        
        .feature-card {
            background: rgba(30, 30, 46, 0.7);
            border-radius: 10px;
            padding: 20px;
            transition: transform 0.3s, box-shadow 0.3s;
            border: 1px solid #444;
        }
        
        .feature-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
        }
        
        .feature-card h3 {
            color: #2575fc;
            margin-bottom: 15px;
            display: flex;
            align-items: center;
        }
        
        .feature-card h3 i {
            margin-right: 10px;
        }
        
        .code-block {
            background: #1a1a2e;
            border-left: 4px solid #6a11cb;
            padding: 15px;
            margin: 15px 0;
            border-radius: 5px;
            overflow-x: auto;
            font-family: monospace;
        }
        
        .screenshot {
            width: 100%;
            border-radius: 10px;
            margin: 15px 0;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
        }
        
        .details {
            background: rgba(30, 30, 46, 0.7);
            border-radius: 10px;
            padding: 15px;
            margin-top: 15px;
            border-left: 4px solid #2575fc;
        }
        
        .author {
            text-align: center;
            padding: 20px;
            margin-top: 30px;
            background: rgba(10, 10, 10, 0.8);
            border-radius: 10px;
        }
        
        .author a {
            color: #6a11cb;
            text-decoration: none;
            font-weight: bold;
        }
        
        .copyright {
            text-align: center;
            margin-top: 20px;
            padding: 15px;
            font-size: 0.9rem;
            color: #777;
            border-top: 1px solid #333;
        }
        
        @media (max-width: 768px) {
            h1 {
                font-size: 2.5rem;
            }
            
            .features {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <div class="logo">
                <i class="fas fa-ghost"></i>
                <h1>GhostTrack</h1>
            </div>
            <p class="tagline">Advanced OSINT Tool for Location & Mobile Number Tracking</p>
            <div class="update-badge">New Update: Version 2.2</div>
        </header>
        
        <div class="section">
            <h2><i class="fas fa-download"></i> Installation</h2>
            
            <div class="features">
                <div class="feature-card">
                    <h3><i class="fab fa-linux"></i> Linux (Debian)</h3>
                    <div class="code-block">
                        sudo apt-get install git<br>
                        sudo apt-get install python3
                    </div>
                </div>
                
                <div class="feature-card">
                    <h3><i class="fas fa-mobile-alt"></i> Termux</h3>
                    <div class="code-block">
                        pkg install git<br>
                        pkg install python3
                    </div>
                </div>
            </div>
            
            <div class="code-block">
                git clone https://github.com/HunxByts/GhostTrack.git<br>
                cd GhostTrack<br>
                pip3 install -r requirements.txt<br>
                python3 GhostTR.py
            </div>
        </div>
        
        <div class="section">
            <h2><i class="fas fa-map-marker-alt"></i> IP Tracker</h2>
            <p>Track location information using an IP address. Combine with Seeker tool for enhanced targeting.</p>
            
            <div class="details">
                <strong>Install Seeker:</strong>
                <div class="code-block">
                    <a href="https://github.com/thewhiteh4t/seeker" target="_blank">Get Seeker</a>
                </div>
            </div>
            
            <img src="https://github.com/HunxByts/GhostTrack/blob/main/asset/ip.png" alt="IP Tracker Screenshot" class="screenshot">
        </div>
        
        <div class="section">
            <h2><i class="fas fa-phone"></i> Phone Tracker</h2>
            <p>Gather information from a target phone number with advanced tracking capabilities.</p>
            <img src="https://github.com/HunxByts/GhostTrack/blob/main/asset/phone.png" alt="Phone Tracker Screenshot" class="screenshot">
        </div>
        
        <div class="section">
            <h2><i class="fas fa-user"></i> Username Tracker</h2>
            <p>Search for information across social media platforms using a target username.</p>
            <img src="https://github.com/HunxByts/GhostTrack/blob/main/asset/User.png" alt="Username Tracker Screenshot" class="screenshot">
        </div>
        
        <div class="author">
            <h2><i class="fas fa-user-tie"></i> Author</h2>
            <p>Created by <a href="https://github.com/HunxByts" target="_blank">HunxByts</a></p>
        </div>
        
        <div class="copyright">
            NO COPYRIGHT ©️𝐋𝐮𝐜𝐢𝐟𝐞𝐫....!!🌈™
        </div>
    </div>

    <script>
        // Simple animation for feature cards on scroll
        document.addEventListener('DOMContentLoaded', function() {
            const featureCards = document.querySelectorAll('.feature-card');
            
            const observer = new IntersectionObserver((entries) => {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        entry.target.style.opacity = 1;
                        entry.target.style.transform = 'translateY(0)';
                    }
                });
            }, { threshold: 0.1 });
            
            featureCards.forEach(card => {
                card.style.opacity = 0;
                card.style.transform = 'translateY(20px)';
                card.style.transition = 'opacity 0.5s, transform 0.5s';
                observer.observe(card);
            });
        });
    </script>
</body>
</html>