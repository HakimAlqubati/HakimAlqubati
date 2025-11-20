<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hakim Qubati | Nexus Architect [2240 CE]</title>
    <meta name="description" content="Interfacing advanced sentient networks and crafting hyper-scalable quantum architectures.">
    
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@400;700;900&family=Share+Tech+Mono&display=swap" rel="stylesheet">
    
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

    <style>
        /* --- إعدادات الصفحة الأساسية (Canvas) --- */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Orbitron', sans-serif;
            background-color: #05070a; /* أسود فضائي عميق */
            color: #00E8FF; /* توهج سماوي */
            height: 100vh;
            width: 100vw;
            overflow: hidden;
            display: flex;
            justify-content: center;
            align-items: center;
            position: relative;
            perspective: 1500px; /* عمق ثلاثي الأبعاد */
        }

        /* --- خلفية متحركة (سديم فضائي) --- */
        body::before, body::after {
            content: '';
            position: absolute;
            border-radius: 50%;
            filter: blur(100px);
            z-index: 0;
            opacity: 0.4;
            animation: floatNebula 10s infinite alternate;
        }
        body::before {
            width: 600px;
            height: 600px;
            background: #7000ff; /* بنفسجي */
            top: -10%;
            left: -10%;
        }
        body::after {
            width: 500px;
            height: 500px;
            background: #00ffff; /* سماوي */
            bottom: -10%;
            right: -10%;
            animation-delay: 5s;
        }

        @keyframes floatNebula {
            0% { transform: translate(0, 0) scale(1); }
            100% { transform: translate(50px, 50px) scale(1.1); }
        }

        /* --- البطاقة الرئيسية (الواجهة العصبية) --- */
        .neural-interface {
            position: relative;
            z-index: 10;
            /* خلفية زجاجية شفافة */
            background: rgba(15, 23, 42, 0.6); 
            backdrop-filter: blur(12px);
            -webkit-backdrop-filter: blur(12px);
            border: 1px solid rgba(0, 232, 255, 0.3);
            border-radius: 24px;
            padding: 4rem 3rem;
            max-width: 600px;
            width: 90%;
            
            /* الظل والإضاءة */
            box-shadow: 
                0 0 40px rgba(0, 232, 255, 0.1),
                inset 0 0 20px rgba(0, 232, 255, 0.05);
            
            /* إعدادات الحركة ثلاثية الأبعاد */
            transform-style: preserve-3d;
            transform: rotateX(0) rotateY(0);
            /* الانتقال ناعم جداً */
            transition: transform 0.1s ease-out; 
        }

        /* تأثير شبكة البيانات المتحركة فوق البطاقة */
        .neural-interface::after {
            content: '';
            position: absolute;
            inset: 0;
            background: linear-gradient(transparent 50%, rgba(0, 232, 255, 0.05) 50%);
            background-size: 100% 4px;
            z-index: -1;
            border-radius: 24px;
            pointer-events: none;
            animation: scanlines 6s linear infinite;
        }

        @keyframes scanlines {
            0% { background-position: 0 0; }
            100% { background-position: 0 100%; }
        }

        /* --- النصوص والعناوين --- */
        h1 {
            font-size: 3.5rem;
            font-weight: 900;
            text-transform: uppercase;
            letter-spacing: 2px;
            margin-bottom: 10px;
            background: linear-gradient(90deg, #fff, #00E8FF);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            text-shadow: 0 0 20px rgba(0, 232, 255, 0.5);
            transform: translateZ(50px); /* يبرز النص للأمام */
        }

        .role-badge {
            display: inline-block;
            padding: 8px 20px;
            border: 1px solid #00E8FF;
            color: #00E8FF;
            font-family: 'Share Tech Mono', monospace;
            font-size: 1rem;
            letter-spacing: 1px;
            border-radius: 50px;
            background: rgba(0, 232, 255, 0.1);
            margin-bottom: 2rem;
            box-shadow: 0 0 15px rgba(0, 232, 255, 0.4);
            transform: translateZ(40px);
        }

        .bio {
            color: #a5b4fc;
            font-family: 'Share Tech Mono', monospace;
            font-size: 1.1rem;
            line-height: 1.6;
            margin-bottom: 3rem;
            text-shadow: 0 0 5px rgba(165, 180, 252, 0.3);
            transform: translateZ(30px);
        }

        /* --- الأزرار (الروابط الكمومية) --- */
        .links-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 15px;
            transform: translateZ(60px); /* الأزرار تبرز أكثر */
        }

        .btn {
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 10px;
            padding: 14px;
            text-decoration: none;
            font-weight: bold;
            border-radius: 12px;
            font-size: 0.9rem;
            transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
            position: relative;
            overflow: hidden;
            border: 1px solid transparent;
            backdrop-filter: blur(4px);
        }

        /* تأثير اللمعان عند مرور الماوس */
        .btn::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255,255,255,0.2), transparent);
            transition: 0.5s;
        }
        .btn:hover::before {
            left: 100%;
        }

        /* WhatsApp */
        .btn-whatsapp {
            background: rgba(37, 211, 102, 0.1);
            color: #25D366;
            border-color: rgba(37, 211, 102, 0.3);
        }
        .btn-whatsapp:hover {
            background: rgba(37, 211, 102, 0.2);
            box-shadow: 0 0 20px rgba(37, 211, 102, 0.6);
            transform: scale(1.05);
        }

        /* Email */
        .btn-email {
            background: rgba(248, 113, 113, 0.1);
            color: #f87171;
            border-color: rgba(248, 113, 113, 0.3);
        }
        .btn-email:hover {
            background: rgba(248, 113, 113, 0.2);
            box-shadow: 0 0 20px rgba(248, 113, 113, 0.6);
            transform: scale(1.05);
        }

        /* LinkedIn */
        .btn-linkedin {
            background: rgba(10, 102, 194, 0.1);
            color: #0a66c2;
            border-color: rgba(10, 102, 194, 0.3);
        }
        .btn-linkedin:hover {
            background: rgba(10, 102, 194, 0.2);
            box-shadow: 0 0 20px rgba(10, 102, 194, 0.6);
            transform: scale(1.05);
        }

        /* Facebook */
        .btn-facebook {
            background: rgba(24, 119, 242, 0.1);
            color: #1877f2;
            border-color: rgba(24, 119, 242, 0.3);
        }
        .btn-facebook:hover {
            background: rgba(24, 119, 242, 0.2);
            box-shadow: 0 0 20px rgba(24, 119, 242, 0.6);
            transform: scale(1.05);
        }

        /* --- نقاط البيانات (Data Dots) --- */
        .data-dots {
            display: flex;
            justify-content: center;
            gap: 10px;
            margin-top: 2.5rem;
            transform: translateZ(20px);
        }
        .dot {
            width: 8px;
            height: 8px;
            border-radius: 50%;
            background: #00E8FF;
            animation: pulseDot 1.5s infinite alternate;
        }
        .dot:nth-child(2) { animation-delay: 0.2s; background: #7000ff; }
        .dot:nth-child(3) { animation-delay: 0.4s; background: #fff; }

        @keyframes pulseDot {
            0% { transform: scale(1); opacity: 0.5; box-shadow: 0 0 0 rgba(0, 232, 255, 0); }
            100% { transform: scale(1.5); opacity: 1; box-shadow: 0 0 10px rgba(0, 232, 255, 0.8); }
        }

        @media (max-width: 500px) {
            .links-grid { grid-template-columns: 1fr; }
            h1 { font-size: 2.5rem; }
            .neural-interface { padding: 2rem; }
        }

        /* لمعان خفيف عشوائي على البطاقة */
        .glare {
            position: absolute;
            width: 100%;
            height: 100%;
            top: 0;
            left: 0;
            background: radial-gradient(circle at 50% 50%, rgba(255,255,255,0.1), transparent 60%);
            opacity: 0;
            pointer-events: none;
            border-radius: 24px;
            z-index: 15;
            transition: opacity 0.1s;
        }

    </style>
</head>
<body>

    <div class="neural-interface" id="card">
        <div class="glare" id="glare"></div>

        <h1>Hakim Qubati</h1>
        
        <div class="role-badge">
            &lt;Nexus Architect /&gt;
        </div>

        <p class="bio">
            [SYSTEM ONLINE]: Interfacing sentient networks. <br>
            Building hyper-scalable SaaS architectures & Quantum Data Flows.
        </p>

        <div class="links-grid">
            <a href="https://wa.me/967773030069" target="_blank" class="btn btn-whatsapp">
                <i class="fab fa-whatsapp"></i> WhatsApp // Net
            </a>

            <a href="mailto:hakimahmed123321@gmail.com" class="btn btn-email">
                <i class="fas fa-envelope"></i> Email // Uplink
            </a>

            <a href="https://www.linkedin.com/in/hakim-ahmed-165106214/" target="_blank" class="btn btn-linkedin">
                <i class="fab fa-linkedin-in"></i> LinkedIn // Node
            </a>

            <a href="https://www.facebook.com/alqubatiabdulhakim" target="_blank" class="btn btn-facebook">
                <i class="fab fa-facebook-f"></i> Meta // Verse
            </a>
        </div>

        <div class="data-dots">
            <div class="dot"></div>
            <div class="dot"></div>
            <div class="dot"></div>
        </div>
    </div>

    <script>
        const card = document.getElementById('card');
        const glare = document.getElementById('glare');
        const body = document.body;

        // حساسية الحركة (كلما زاد الرقم قلت الحركة)
        const sensitivity = 25;

        body.addEventListener('mousemove', (e) => {
            const x = e.clientX;
            const y = e.clientY;
            
            const w = window.innerWidth;
            const h = window.innerHeight;

            // حساب زاوية الدوران بناءً على موقع الماوس
            // الماوس يمين -> دوران محور Y موجب
            // الماوس تحت -> دوران محور X سالب (ليبدأ من الأعلى)
            
            const rotateY = ((x - w / 2) / w) * sensitivity;
            const rotateX = ((y - h / 2) / h) * -sensitivity;

            // تطبيق الحركة على البطاقة
            card.style.transform = `
                rotateX(${rotateX}deg) 
                rotateY(${rotateY}deg)
            `;

            // تحريك لمعان الإضاءة (Glare Effect) عكس اتجاه الماوس لزيادة الواقعية
            const glareX = ((x / w) * 100);
            const glareY = ((y / h) * 100);
            
            glare.style.background = `radial-gradient(circle at ${glareX}% ${glareY}%, rgba(255,255,255,0.15), transparent 50%)`;
            glare.style.opacity = '1';
        });

        body.addEventListener('mouseleave', () => {
            // إعادة البطاقة لوضعها الطبيعي عند خروج الماوس
            card.style.transform = `rotateX(0) rotateY(0)`;
            glare.style.opacity = '0';
        });
    </script>

</body>
</html>
