<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hypertension - High Blood Pressure</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.7;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: #333;
        }
        .container {
            max-width: 1100px;
            margin: 0 auto;
            background: white;
            box-shadow: 0 20px 60px rgba(0,0,0,0.2);
        }
        /* Header */
        .header {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 40px 30px;
            text-align: center;
        }
        .header h1 {
            font-size: 2.5em;
            margin-bottom: 10px;
        }
        .header p {
            font-size: 1.1em;
            opacity: 0.9;
        }
        /* Navigation Tabs */
        .nav-tabs {
            background: #2c3e50;
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            list-style: none;
        }
        .nav-tabs li {
            list-style: none;
        }
        .nav-tabs button {
            background: none;
            border: none;
            padding: 15px 25px;
            font-size: 1em;
            font-weight: bold;
            color: #ecf0f1;
            cursor: pointer;
            transition: all 0.3s ease;
            font-family: inherit;
        }
        .nav-tabs button:hover {
            background: #34495e;
            color: white;
        }
        .nav-tabs button.active {
            background: #3498db;
            color: white;
        }
        /* Content Sections */
        .tab-content {
            padding: 40px;
        }
        .tab-pane {
            display: none;
            animation: fadeIn 0.5s ease;
        }
        .tab-pane.active {
            display: block;
        }
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(10px); }
            to { opacity: 1; transform: translateY(0); }
        }
        h2 {
            color: #2c3e50;
            border-left: 5px solid #3498db;
            padding-left: 15px;
            margin-bottom: 25px;
            font-size: 1.8em;
        }
        .intro-box {
            background: linear-gradient(135deg, #e8f4fd, #d1ecf9);
            padding: 25px;
            border-radius: 15px;
            margin: 20px 0;
            border-left: 5px solid #3498db;
        }
        ul {
            margin: 15px 0;
            padding-left: 25px;
        }
        li {
            margin: 10px 0;
        }
        .image-box {
            text-align: center;
            margin: 25px 0;
        }
        .image-box img {
            max-width: 100%;
            border-radius: 15px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }
        .image-caption {
            font-size: 0.85em;
            color: #7f8c8d;
            margin-top: 8px;
        }
        .bp-card {
            background: #fef9e7;
            padding: 20px;
            border-radius: 15px;
            margin: 20px 0;
            border-left: 5px solid #e67e22;
        }
        .stats {
            display: flex;
            justify-content: space-around;
            flex-wrap: wrap;
            gap: 20px;
            margin: 30px 0;
        }
        .stat-box {
            background: linear-gradient(135deg, #3498db, #2980b9);
            color: white;
            padding: 20px;
            border-radius: 15px;
            text-align: center;
            flex: 1;
            min-width: 150px;
        }
        .stat-box .number {
            font-size: 2.2em;
            font-weight: bold;
        }
        footer {
            background: #2c3e50;
            color: white;
            text-align: center;
            padding: 25px;
            font-size: 0.9em;
        }
        @media (max-width: 768px) {
            .nav-tabs button { padding: 10px 15px; font-size: 0.85em; }
            .tab-content { padding: 20px; }
            .header h1 { font-size: 1.8em; }
        }
    </style>
</head>
<body>

<div class="container">
    <div class="header">
        <h1>🩸 Hypertension (High Blood Pressure)</h1>
        <p>The Silent Killer - Know the Facts, Save Your Life</p>
    </div>

    <!-- Tabs Navigation -->
    <ul class="nav-tabs">
        <li><button class="tab-btn active" data-tab="intro">📖 Introduction</button></li>
        <li><button class="tab-btn" data-tab="causes">🩺 Causes</button></li>
        <li><button class="tab-btn" data-tab="symptoms">⚠️ Symptoms</button></li>
        <li><button class="tab-btn" data-tab="diagnosis">🔬 Diagnosis</button></li>
        <li><button class="tab-btn" data-tab="treatment">💊 Treatment</button></li>
        <li><button class="tab-btn" data-tab="prevention">🛡️ Prevention</button></li>
        <li><button class="tab-btn" data-tab="conclusion">📖 Conclusion</button></li>
    </ul>

    <!-- Tab Content -->
    <div class="tab-content">
        <!-- Introduction -->
        <div id="intro" class="tab-pane active">
            <div class="image-box">
                <img src="images/3.jpg" alt="Blood pressure measurement">
                <img src="images/2.jpg" alt="Blood pressure measurement">

                <div class="image-caption">Measuring blood pressure - First step to diagnosis</div>
            </div>
            <div class="intro-box">
                <h2>📌 What is Hypertension?</h2>
                <p>Hypertension, commonly known as high blood pressure, is a long-term medical condition in which the blood pressure in the arteries is persistently elevated. It is often called the <strong>"silent killer"</strong> because it usually has no warning signs or symptoms, but can lead to serious health problems like heart attack, stroke, and kidney failure.</p>
                <p>The disease occurs mainly in adults over 40, but younger people can also be affected. According to WHO, <strong>1.28 billion adults worldwide</strong> have hypertension, and nearly half are unaware of their condition.</p>
            </div>
        </div>

        <!-- Causes -->
        <div id="causes" class="tab-pane">
            <h2>🩺 Causes & Risk Factors</h2>
            <div class="image-box">
                <img src="images/4.jpg" alt="Blood pressure measurement">
                <div class="image-caption">Common risk factors for hypertension</div>
            </div>
            <p>Hypertension is divided into two types:</p>
            <ul>
                <li><strong>Primary (Essential) Hypertension:</strong> No single identifiable cause; develops gradually over many years. Risk factors include age, genetics, obesity, high salt intake, lack of physical activity, and stress.</li>
                <li><strong>Secondary Hypertension:</strong> Caused by an underlying condition such as kidney disease, adrenal gland tumors, thyroid problems, or use of certain medications.</li>
            </ul>
            <div class="stats">
                <div class="stat-box"><div class="number">1 in 3</div><div>Adults have hypertension</div></div>
                <div class="stat-box"><div class="number">50%</div><div>Unaware of their condition</div></div>
            </div>
        </div>

        <!-- Symptoms -->
        <div id="symptoms" class="tab-pane">
            <h2>⚠️ Warning Signs & Symptoms</h2>
            <div class="image-box">
                <img src="images/6.jpg" alt="Blood pressure measurement">
                <div class="image-caption">Severe headache and chest pain are warning signs</div>
            </div>
            <p>Most people with hypertension have no symptoms at all. However, extremely high blood pressure (hypertensive crisis) may cause:</p>
            <ul>
                <li>Severe headaches (especially at the back of the head)</li>
                <li>Shortness of breath</li>
                <li>Nosebleeds</li>
                <li>Chest pain</li>
                <li>Vision problems or blurred vision</li>
                <li>Blood in urine</li>
                <li>Ringing in the ears (tinnitus)</li>
            </ul>
            <p><strong>⚠️ Note:</strong> Regular blood pressure checks are essential because symptoms usually appear only when the condition has already caused organ damage.</p>
        </div>

        <!-- Diagnosis -->
        <div id="diagnosis" class="tab-pane">
            <h2>🔬 How is Hypertension Diagnosed?</h2>
            <div class="image-box">
                <img src="images/8.jpg" alt="Blood pressure measurement">
                <div class="image-caption">Regular monitoring at home is important</div>
            </div>
            <p>Diagnosis is made by measuring blood pressure using a sphygmomanometer (blood pressure cuff). According to standard guidelines:</p>
            <div class="bp-card">
                <p><strong>🟢 Normal:</strong> Less than 120/80 mm Hg</p>
                <p><strong>🟡 Elevated:</strong> 120-129 / less than 80 mm Hg</p>
                <p><strong>🟠 Stage 1 Hypertension:</strong> 130-139 / 80-89 mm Hg</p>
                <p><strong>🔴 Stage 2 Hypertension:</strong> 140 or higher / 90 or higher mm Hg</p>
                <p><strong>⚫ Hypertensive Crisis:</strong> Higher than 180/120 mm Hg (requires immediate medical attention)</p>
            </div>
            <p>Doctors may also order blood tests, urine tests, ECG, or echocardiogram to check for complications.</p>
        </div>

        <!-- Treatment -->
        <div id="treatment" class="tab-pane">
            <h2>💊 Treatment Options</h2>
            <div class="image-box">
                <img src="images/12.jpg" alt="Blood pressure measurement">
                <div class="image-caption">Common blood pressure medications</div>
            </div>
            <p>Treatment includes lifestyle changes and medications:</p>
            <ul>
                <li><strong>Lifestyle modifications:</strong> Reduce salt intake, eat more fruits/vegetables (DASH diet), exercise regularly (at least 30 minutes daily), maintain healthy weight, limit alcohol, and quit smoking.</li>
                <li><strong>Common medications:</strong> ACE inhibitors (Lisinopril), ARBs (Losartan), Calcium channel blockers (Amlodipine), Diuretics (Hydrochlorothiazide), Beta-blockers (Metoprolol).</li>
            </ul>
            <div class="intro-box">
                <p><strong>💡 Important Note:</strong> Most patients need to take medication for life. Never stop medication without doctor's advice. Regular follow-up is essential.</p>
            </div>
        </div>

        <!-- Prevention -->
        <div id="prevention" class="tab-pane">
            <h2>🛡️ Prevention Tips</h2>
            <div class="image-box">
                <img src="images/10.jpg" alt="Blood pressure measurement">
                <div class="image-caption">Regular exercise and healthy eating are key</div>
            </div>
            <ul>
                <li>Check your blood pressure regularly after age 18</li>
                <li>Eat a balanced, low-sodium diet (less than 5g salt per day)</li>
                <li>Exercise at least 150 minutes per week (brisk walking, swimming, cycling)</li>
                <li>Maintain a healthy BMI (18.5-24.9)</li>
                <li>Manage stress through meditation, yoga, or hobbies</li>
                <li>Limit caffeine and avoid recreational drugs</li>
                <li>Get 7-8 hours of quality sleep each night</li>
            </ul>
        </div>

        <!-- Conclusion -->
        <div id="conclusion" class="tab-pane">
            <h2>📖 Conclusion</h2>
            <div class="image-box">
                <img src="images/13.jpg" alt="Blood pressure measurement">
                <div class="image-caption">A healthy heart starts with healthy habits</div>
            </div>
            <p>Hypertension is manageable and preventable. Regular monitoring, healthy lifestyle choices, and following prescribed treatments can significantly reduce risks of heart attack, stroke, and kidney disease. Education and awareness are the first steps toward better cardiovascular health.</p>
            <p>The fight against high blood pressure demonstrates how simple changes in daily habits can save millions of lives worldwide. <strong>Check your blood pressure today!</strong></p>
            <div class="stats">
                <div class="stat-box"><div class="number">10.4M</div><div>Annual deaths from hypertension</div></div>
                <div class="stat-box"><div class="number">1.28B</div><div>People affected worldwide</div></div>
            </div>
        </div>
    </div>

    <footer>
        <p>Sources: World Health Organization (WHO) | American Heart Association | CDC | Mayo Clinic</p>
        <p>This information is for educational purposes. Always consult a healthcare provider.</p>
        <p>Created by Zahra Mahmoodi - Health Education Resource | 2025</p>
    </footer>
</div>

<script>
    // Tab switching functionality
    const tabBtns = document.querySelectorAll('.tab-btn');
    const tabPanes = document.querySelectorAll('.tab-pane');

    tabBtns.forEach(btn => {
        btn.addEventListener('click', () => {
            // Remove active class from all buttons and panes
            tabBtns.forEach(b => b.classList.remove('active'));
            tabPanes.forEach(pane => pane.classList.remove('active'));
            
            // Add active class to clicked button
            btn.classList.add('active');
            
            // Show corresponding pane
            const tabId = btn.getAttribute('data-tab');
            document.getElementById(tabId).classList.add('active');
        });
    });
</script>

</body>
</html>
