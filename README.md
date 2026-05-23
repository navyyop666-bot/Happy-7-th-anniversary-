# Happy-7-th anniversary
<!DOCTYPE html>
<html lang="hi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>7 Months Love Book - Teena & Navu</title>
    <!-- Premium Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Cinzel:wght@400;700&family=Playfair+Display:ital,wght@0,400;0,700;1,400&family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">
    
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Poppins', sans-serif;
            background-color: #fcf8f7;
            color: #2c2c2c;
            overflow-x: hidden;
        }

        /* Smooth Scroll */
        html {
            scroll-behavior: smooth;
        }

        /* Magazine Layout Container */
        .magazine-container {
            max-width: 900px;
            margin: 0 auto;
            padding: 20px;
        }

        /* Page/Section Styling */
        .magazine-page {
            min-height: 95vh;
            background: #ffffff;
            margin: 40px 0;
            padding: 60px;
            box-shadow: 0 20px 40px rgba(0,0,0,0.06);
            border: 1px solid #f1e4e4;
            position: relative;
            display: flex;
            flex-direction: column;
            justify-content: center;
            border-radius: 4px;
        }

        /* Book Spine Effect */
        .magazine-page::before {
            content: '';
            position: absolute;
            left: 0;
            top: 0;
            bottom: 0;
            width: 10px;
            background: linear-gradient(to right, rgba(0,0,0,0.05), transparent);
        }

        /* Premium Magazine Borders */
        .page-border {
            border: 1px solid #dfc3c3;
            height: 100%;
            width: 100%;
            position: absolute;
            top: 0;
            left: 0;
            pointer-events: none;
            transform: scale(0.95);
        }

        /* Page Numbering */
        .page-number {
            position: absolute;
            bottom: 25px;
            font-family: 'Cinzel', serif;
            font-size: 0.9rem;
            color: #a38181;
            letter-spacing: 2px;
        }
        .page-left { left: 40px; }
        .page-right { right: 40px; }

        /* --- PAGE 1: MAGAZINE COVER --- */
        .cover {
            background: linear-gradient(rgba(255, 255, 255, 0.85), rgba(255, 255, 255, 0.85)), url('https://picsum.photos/900/1200?romantic') no-repeat center center/cover;
            text-align: center;
            border: 8px double #dfc3c3;
        }

        .magazine-header {
            font-family: 'Cinzel', serif;
            font-size: 1.2rem;
            letter-spacing: 6px;
            color: #5a5a5a;
            text-transform: uppercase;
            margin-bottom: 20px;
        }

        .magazine-title {
            font-family: 'Playfair Display', serif;
            font-size: 4.5rem;
            font-style: italic;
            color: #bc4749;
            line-height: 5rem;
            margin: 30px 0;
            font-weight: 700;
        }

        .issue-info {
            font-family: 'Cinzel', serif;
            border-top: 1px solid #2c2c2c;
            border-bottom: 1px solid #2c2c2c;
            padding: 10px 0;
            width: 60%;
            margin: 0 auto 40px auto;
            font-size: 0.9rem;
            letter-spacing: 3px;
        }

        .cover-tagline {
            font-size: 1.2rem;
            font-weight: 300;
            color: #666;
            max-width: 500px;
            margin: 0 auto;
            line-height: 1.8rem;
        }

        /* --- PAGE 2: EDITORIAL / SHAYARI --- */
        .editorial-title {
            font-family: 'Playfair Display', serif;
            font-size: 2.8rem;
            color: #2c2c2c;
            margin-bottom: 40px;
            text-align: left;
        }

        .editorial-layout {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 40px;
            text-align: left;
        }

        .dropcap {
            font-family: 'Playfair Display', serif;
            font-size: 4.5rem;
            float: left;
            line-height: 3.5rem;
            padding-right: 10px;
            color: #bc4749;
            font-weight: bold;
        }

        .shayari-box {
            grid-column: 1 / -1;
            background: #fff9f9;
            padding: 30px;
            border-left: 3px solid #bc4749;
            font-family: 'Playfair Display', serif;
            font-size: 1.4rem;
            font-style: italic;
            line-height: 2.5rem;
            text-align: center;
            color: #444;
            margin-top: 20px;
        }

        /* --- PAGE 3: INTERACTIVE FEATURE --- */
        .interactive-title {
            font-family: 'Cinzel', serif;
            font-size: 2rem;
            color: #bc4749;
            margin-bottom: 15px;
            letter-spacing: 2px;
        }

        .game-card {
            border: 1px solid #eee;
            padding: 40px 20px;
            border-radius: 4px;
            background: #fafafa;
            margin-top: 20px;
        }

        .action-btn {
            background-color: #2c2c2c;
            color: white;
            border: none;
            padding: 12px 35px;
            font-family: 'Cinzel', serif;
            font-size: 0.9rem;
            letter-spacing: 2px;
            cursor: pointer;
            transition: all 0.3s ease;
            margin-top: 20px;
        }

        .action-btn:hover {
            background-color: #bc4749;
            transform: translateY(-2px);
        }

        .love-meter-bar {
            width: 100%;
            height: 8px;
            background: #eee;
            margin-top: 30px;
            border-radius: 4px;
            overflow: hidden;
            display: none;
        }

        .love-meter-fill {
            height: 100%;
            width: 0%;
            background: #bc4749;
            transition: width 2s ease-in-out;
        }

        .result-text {
            font-family: 'Playfair Display', serif;
            font-size: 1.5rem;
            margin-top: 20px;
            color: #bc4749;
            font-style: italic;
        }

        /* --- PAGE 4: BACK COVER / SUPREME COURT --- */
        .back-cover {
            text-align: center;
            background: #fffaf9;
        }

        .final-quote {
            font-family: 'Playfair Display', serif;
            font-size: 2.5rem;
            color: #2c2c2c;
            margin-bottom: 20px;
            font-weight: 700;
        }

        .supreme-court-badge {
            font-family: 'Cinzel', serif;
            font-size: 1.5rem;
            color: #bc4749;
            letter-spacing: 4px;
            margin: 40px 0;
            font-weight: 700;
            border-top: 1px solid #dfc3c3;
            border-bottom: 1px solid #dfc3c3;
            padding: 15px 0;
            display: inline-block;
            width: 80%;
        }

        .signature {
            font-family: 'Playfair Display', serif;
            font-size: 1.2rem;
            font-style: italic;
            color: #777;
        }

        /* Navigation Buttons between pages */
        .nav-arrow {
            display: inline-block;
            margin-top: 30px;
            color: #a38181;
            text-decoration: none;
            font-family: 'Cinzel', serif;
            font-size: 0.8rem;
            letter-spacing: 2px;
            transition: color 0.3s;
        }
        .nav-arrow:hover {
            color: #bc4749;
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .magazine-page { padding: 30px; }
            .magazine-title { font-size: 3rem; line-height: 3.5rem; }
            .editorial-layout { grid-template-columns: 1fr; gap: 20px; }
            .final-quote { font-size: 1.8rem; }
        }
    </style>
</head>
<body>

    <div class="magazine-container">

        <!-- PAGE 1: THE COVER -->
        <section class="magazine-page cover" id="page1">
            <div class="page-border"></div>
            <div class="magazine-header">Special Anniversary Edition</div>
            <h1 class="magazine-title">The 7 Months<br>Love Book</h1>
            <div class="issue-info">ISSUE NO. 07 • TEENA SONI</div>
            <p class="cover-tagline">
                Aapke sath beeta har ek lamha, har ek din meri zindagi ka sabse haseen panna ban gaya hai. 
            </p>
            <a href="#page2" class="nav-arrow">Read Magazine →</a>
        </section>


        <!-- PAGE 2: EDITORIAL & SHAYARI -->
        <section class="magazine-page" id="page2">
            <div class="page-border"></div>
            <h2 class="editorial-title">Humara Haseen Safar...</h2>
            
            <div class="editorial-layout">
                <div>
                    <p><span class="dropcap">A</span>apke sath bitaye in 7 mahino mein maine jana ki sacha pyaar kya hota hai. Aapka meri zindagi mein hona kisi tohfe se kam nahi hai. Aapki har baat, aapki fikr mere liye sabse khaas hai.</p>
                </div>
                <div>
                    <p>Zindagi ki is kitaab mein, yeh 7 mahine sabse khubsoorat chapter hain. Navu ka waada hai aap se, yeh mohabbat har guzarte din ke sath aur gehri aur pakki hoti jayegi.</p>
                </div>
                
                <div class="shayari-box">
                    "Aapki muskurahat se shuru hoti hai meri har subah,<br>
                    Aap sath ho toh har manzil lagti hai aasan.<br>
                    7 mahine ka yeh safar toh bas ek shuruat hai,<br>
                    Aap hi toh ho meri duniya, meri jaan."
                </div>
            </div>

            <div class="page-number page-left">VOL I</div>
            <div class="page-number page-right">PAGE 02</div>
            <center><a href="#page3" class="nav-arrow">Next Feature →</a></center>
        </section>


        <!-- PAGE 3: THE LOVE INTERACTIVE INTERVIEW -->
        <section class="magazine-page" id="page3">
            <div class="page-border"></div>
            <div style="text-align: center;">
                <div class="magazine-header" style="font-size: 0.9rem;">Exclusive Feature</div>
                <h2 class="interactive-title">The Compatibility Index</h2>
                <p style="color: #666; max-width: 500px; margin: 0 auto;">Navu aur Teena Bhabhi ke rishte ki gehrai ko napne ka ek chota sa magazine test.</p>
                
                <div class="game-card">
                    <p style="font-size: 1.1rem; font-weight: 600;">Pyaar Ki Intensity Check Karein</p>
                    <button class="action-btn" onclick="startLoveMeter()">Analyze Now</button>
                    
                    <div class="love-meter-bar" id="meterBar">
                        <div class="love-meter-fill" id="meterFill"></div>
                    </div>
                    <div class="result-text" id="analysisResult"></div>
                </div>
            </div>

            <div class="page-number page-left">VOL I</div>
            <div class="page-number page-right">PAGE 03</div>
            <center><a href="#page4" class="nav-arrow">The Back Cover →</a></center>
        </section>


        <!-- PAGE 4: BACK COVER (FINAL MESSAGE) -->
        <section class="magazine-page back-cover" id="page4">
            <div class="page-border"></div>
            <div class="magazine-header" style="color: #bc4749;">The Final Word</div>
            
            <h2 class="final-quote">I Love You Teena</h2>
            <p style="font-size: 1.2rem; max-width: 600px; margin: 0 auto; line-height: 2rem; color: #444;">
                Aap kal bhi meri thi, aaj bhi meri ho aur hamesha meri rahogi. Humara yeh safar zindagi bhar aise hi chalta rahega.
            </p>
            
            <div class="supreme-court-badge">
                ✨ MY SUPREME COURT ✨
            </div>
            
            <div class="signature">
                Hamesha Ke Liye Aapka,<br>
                <strong style="color: #2c2c2c; font-size: 1.4rem; font-family: 'Playfair Display', serif;">Navu</strong>
            </div>

            <div class="page-number page-left">END</div>
            <div class="page-number page-right">ISSUE 07</div>
            <center><a href="#page1" class="nav-arrow" style="margin-top: 40px;">← Back to Cover</a></center>
        </section>

    </div>

    <!-- JavaScript For Magazine Features -->
    <script>
        function startLoveMeter() {
            const bar = document.getElementById('meterBar');
            const fill = document.getElementById('meterFill');
            const result = document.getElementById('analysisResult');
            
            bar.style.display = 'block';
            fill.style.width = '0%';
            result.innerHTML = "Analyzing relationship dynamics... ✨";
            
            setTimeout(() => {
                fill.style.width = '100%';
            }, 100);

            setTimeout(() => {
                result.innerHTML = "💝 Result: 100% Infinite Compatibility! Yeh Rishta Sabse Bemisaal Hai! 💝";
            }, 2100);
        }
    </script>

</body>
</html>
