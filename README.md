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
        .audio-player-container {
            margin: 30px 0;
            font-family: 'Segoe UI', Arial, sans-serif;
        }
    <!-- ===== Voice Introduction Player ===== -->
<div style="background: linear-gradient(135deg, #667eea, #764ba2); border-radius: 20px; padding: 20px; margin: 20px; text-align: center; color: white; box-shadow: 0 10px 25px rgba(0,0,0,0.1);">
    <h3 style="margin: 0 0 10px 0;">🎙️ Audio: What is Hypertension?</h3>
    <p style="margin: 0 0 15px 0; opacity: 0.9;">Listen to the introduction about high blood pressure</p>
    <audio controls style="width: 100%; max-width: 350px; margin: 0 auto; display: block; border-radius: 10px;">
        <source src="images/A.m4a" type="audio/mp4">
        Your browser does not support the audio element.
    </audio>
</div>        
        @keyframes pulse {
            0% { transform: scale(1); opacity: 1; }
            50% { transform: scale(1.1); opacity: 0.8; }
            100% { transform: scale(1); opacity: 1; }
        }
        </style>
     .audio-card {
        background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
        border-radius: 20px;
        padding: 20px;
        box-shadow: 0 10px 30px rgba(0,0,0,0.2);
        transition: transform 0.3s ease;
    }
   .audio-card {
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    border-radius: 20px;
    padding: 20px;
    margin: 20px;
    box-shadow: 0 10px 30px rgba(0,0,0,0.2);
    transition: transform 0.3s ease;
}

.audio-card:hover {
    transform: translateY(-3px);
}

.audio-icon {
    text-align: center;
    margin-bottom: 15px;
    color: #ffd700;
}

.audio-icon svg {
    animation: pulse 2s infinite;
}

@keyframes pulse {
    0% { transform: scale(1); opacity: 1; }
    50% { transform: scale(1.1); opacity: 0.8; }
    100% { transform: scale(1); opacity: 1; }
}

.audio-info {
    text-align: center;
    margin-bottom: 20px;
}

.audio-title {
    color: white;
    font-size: 1.2em;
    margin: 0 0 8px 0;
    font-weight: 600;
}

.audio-description {
    color: rgba(255,255,255,0.9);
    font-size: 0.9em;
    margin: 0;
}

.custom-player {
    display: flex;
    align-items: center;
    gap: 15px;
    background: rgba(255,255,255,0.2);
    padding: 12px 18px;
    border-radius: 50px;
    backdrop-filter: blur(10px);
}

.play-btn {
    background: #ffd700;
    border: none;
    width: 45px;
    height: 45px;
    border-radius: 50%;
    cursor: pointer;
    display: flex;
    align-items: center;
    justify-content: center;
    transition: all 0.3s ease;
    box-shadow: 0 2px 10px rgba(0,0,0,0.2);
}

.play-btn:hover {
    transform: scale(1.05);
    background: #ffed4a;
    box-shadow: 0 4px 15px rgba(0,0,0,0.3);
}

.play-btn svg {
    margin-left: 3px;
}

.progress-container {
    flex: 1;
}

.progress-bar {
    background: rgba(255,255,255,0.3);
    height: 6px;
    border-radius: 3px;
    cursor: pointer;
    position: relative;
    overflow: hidden;
}

.progress-fill {
    background: #ffd700;
    height: 100%;
    width: 0%;
    border-radius: 3px;
    transition: width 0.1s linear;
}

.time-info {
    display: flex;
    justify-content: space-between;
    margin-top: 8px;
    color: white;
    font-size: 0.75em;
    font-weight: 500;
}

.volume-btn {
    background: rgba(255,255,255,0.2);
    border: none;
    width: 35px;
    height: 35px;
    border-radius: 50%;
    cursor: pointer;
    display: flex;
    align-items: center;
    justify-content: center;
    color: white;
    transition: all 0.3s ease;
}

.volume-btn:hover {
    background: rgba(255,255,255,0.3);
    transform: scale(1.05);
}

@media (max-width: 600px) {
    .custom-player {
        flex-direction: column;
        border-radius: 20px;
    }
    .progress-container {
        width: 100%;
    }
    .play-btn {
        width: 55px;
        height: 55px;
    }
    .audio-title {
        font-size: 1em;
    }
}
</style>

<!-- ===== HTML پلیر صوتی با فایل A.m4a ===== -->
<div class="audio-card">
    <div class="audio-icon">
        <svg width="50" height="50" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M3 10H7L12 5V19L7 14H3V10Z" fill="#ffd700" stroke="#ffd700" stroke-width="1.5"/>
            <path d="M15.5 8.5C16.5 9.5 17 10.5 17 12C17 13.5 16.5 14.5 15.5 15.5" stroke="#ffd700" stroke-width="1.5" stroke-linecap="round"/>
            <path d="M18 5.5C19.5 7 20.5 9 20.5 12C20.5 15 19.5 17 18 18.5" stroke="#ffd700" stroke-width="1.5" stroke-linecap="round"/>
        </svg>
    </div>
    <div class="audio-info">
        <h3 class="audio-title">🎙️ Audio: What is Hypertension?</h3>
        <p class="audio-description">Listen to the audio explanation about high blood pressure</p>
    </div>
    <audio controls style="width: 100%; border-radius: 10px; margin-top: 10px;">
        <source src="images/A.m4a" type="audio/mp4">
        Your browser does not support the audio element.
    </audio>
</div> 
    .audio-card:hover {
        transform: translateY(-3px);
    }
    
    .audio-icon {
        text-align: center;
        margin-bottom: 15px;
        color: #ffd700;
    }
    
    .audio-icon svg {
        animation: pulse 2s infinite;
    }
    
    @keyframes pulse {
        0% { transform: scale(1); opacity: 1; }
        50% { transform: scale(1.1); opacity: 0.8; }
        100% { transform: scale(1); opacity: 1; }
    }
    
    .audio-info {
        text-align: center;
        margin-bottom: 20px;
    }
    
    .audio-title {
        color: white;
        font-size: 1.2em;
        margin: 0 0 8px 0;
        font-weight: 600;
    }
    
    .audio-description {
        color: rgba(255,255,255,0.9);
        font-size: 0.9em;
        margin: 0;
    }
    
    .custom-player {
        display: flex;
        align-items: center;
        gap: 15px;
        background: rgba(255,255,255,0.2);
        padding: 12px 18px;
        border-radius: 50px;
        backdrop-filter: blur(10px);
    }
    
    .play-btn {
        background: #ffd700;
        border: none;
        width: 45px;
        height: 45px;
        border-radius: 50%;
        cursor: pointer;
        display: flex;
        align-items: center;
        justify-content: center;
        transition: all 0.3s ease;
        box-shadow: 0 2px 10px rgba(0,0,0,0.2);
    }
    
    .play-btn:hover {
        transform: scale(1.05);
        background: #ffed4a;
        box-shadow: 0 4px 15px rgba(0,0,0,0.3);
    }
    
    .play-btn svg {
        margin-left: 3px;
    }
    
    .progress-container {
        flex: 1;
    }
    
    .progress-bar {
        background: rgba(255,255,255,0.3);
        height: 6px;
        border-radius: 3px;
        cursor: pointer;
        position: relative;
        overflow: hidden;
    }
    
    .progress-fill {
        background: #ffd700;
        height: 100%;
        width: 0%;
        border-radius: 3px;
        transition: width 0.1s linear;
    }
    
    .time-info {
        display: flex;
        justify-content: space-between;
        margin-top: 8px;
        color: white;
        font-size: 0.75em;
        font-weight: 500;
    }
    
    .volume-btn {
        background: rgba(255,255,255,0.2);
        border: none;
        width: 35px;
        height: 35px;
        border-radius: 50%;
        cursor: pointer;
        display: flex;
        align-items: center;
        justify-content: center;
        color: white;
        transition: all 0.3s ease;
    }
    
    .volume-btn:hover {
        background: rgba(255,255,255,0.3);
        transform: scale(1.05);
    }

@media (max-width: 600px) {
    .custom-player {
        flex-direction: column;
        border-radius: 20px;
    }

    .progress-container {
        width: 100%;
    }
    
    .play-btn {
        width: 55px;
        height: 55px;
    }
    
    .audio-title {
        font-size: 1em;
    }
}

    
</style>   
        
        .custom-player {
            display: flex;
            align-items: center;
            gap: 15px;
            background: rgba(255,255,255,0.2);
            padding: 12px 18px;
            border-radius: 50px;
            backdrop-filter: blur(10px);
        }
        
        .play-btn {
            background: #ffd700;
            border: none;
            width: 45px;
            height: 45px;
            border-radius: 50%;
            cursor: pointer;
            display: flex;
            align-items: center;
            justify-content: center;
            transition: all 0.3s ease;
            box-shadow: 0 2px 10px rgba(0,0,0,0.2);
        }
        
        .play-btn:hover {
            transform: scale(1.05);
            background: #ffed4a;
            box-shadow: 0 4px 15px rgba(0,0,0,0.3);
        }
        
        .play-btn svg {
            margin-left: 3px;
        }
        
        .progress-container {
            flex: 1;
        }
        
        .progress-bar {
            background: rgba(255,255,255,0.3);
            height: 6px;
            border-radius: 3px;
            cursor: pointer;
            position: relative;
            overflow: hidden;
        }
        
        .progress-fill {
            background: #ffd700;
            height: 100%;
            width: 0%;
            border-radius: 3px;
            transition: width 0.1s linear;
        }
        
        .time-info {
            display: flex;
            justify-content: space-between;
            margin-top: 8px;
            color: white;
            font-size: 0.75em;
            font-weight: 500;
        }
        
        .volume-btn {
            background: rgba(255,255,255,0.2);
            border: none;
            width: 35px;
            height: 35px;
            border-radius: 50%;
            cursor: pointer;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            transition: all 0.3s ease;
        }
        
        .volume-btn:hover {
            background: rgba(255,255,255,0.3);
            transform: scale(1.05);
        }

    @media (max-width: 600px) {
        .custom-player {
            flex-direction: column;
            border-radius: 20px;
        }
    
        .progress-container {
            width: 100%;
        }
        
        .play-btn {
            width: 55px;
            height: 55px;
        }
        
        .audio-title {
            font-size: 1em;
        }
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
                <img src="https://share.google/Xlf88MRw5pqtyx0iV" alt="Blood pressure measurement">
                <img src="images/2.jpg" alt="Blood pressure measurement">

                <div class="image-caption">Measuring blood pressure - First step to diagnosis</div>
            </div>
            <div class="intro-box">
                <h2>📌 What is Hypertension?</h2>
                <p>Hypertension, commonly known as high blood pressure, is a long-term medical condition in which the blood pressure in the arteries is persistently elevated. It is often called the <strong>"silent killer"</strong> because it usually has no warning signs or symptoms, but can lead to serious health problems like heart attack, stroke, and kidney failure.</p>
                <p>The disease occurs mainly in adults over 40, but younger people can also be affected. According to WHO, <strong>1.28 billion adults worldwide</strong> have hypertension, and nearly half are unaware of their condition.</p>
            </div>

<div class="audio-player-container">
    <div class="audio-card">
        <div class="audio-icon">
            <svg viewBox="0 0 24 24" width="32" height="32" fill="currentColor">
                <path d="M12 3v10.55c-.59-.34-1.27-.55-2-.55-2.21 0-4 1.79-4 4s1.79 4 4 4 4-1.79 4-4V7h4V3h-6z"/>
            </svg>
        </div>
        <div class="audio-info">
            <h3 class="audio-title">🎙️ اطلاعات صوتی: فشار خون چیست؟</h3>
            <p class="audio-description">به توضیحات صوتی درباره بیماری فشار خون گوش دهید</p>
        </div>
        <div class="audio-controls">
            <audio id="customAudio" controls style="display:none;">
                <source src="audio/hypertension-guide.mp3" type="audio/mpeg">
                مرورگر شما از پخش صوت پشتیبانی نمی‌کند.
            </audio>
            <div class="custom-player">
                <button class="play-btn" id="playBtn">
                    <svg viewBox="0 0 24 24" width="24" height="24" fill="currentColor">
                        <path d="M8 5v14l11-7z"/>
                    </svg>
                </button>
                <div class="progress-container">
                    <div class="progress-bar" id="progressBar">
                        <div class="progress-fill" id="progressFill"></div>
                    </div>
                    <div class="time-info">
                        <span id="currentTime">0:00</span>
                        <span id="duration">0:00</span>
                    </div>
                </div>
                <button class="volume-btn" id="volumeBtn">
                    <svg viewBox="0 0 24 24" width="20" height="20" fill="currentColor">
                        <path d="M3 9v6h4l5 5V4L7 9H3z"/>
                    </svg>
                </button>
            </div>
        </div>
    </div>
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

            <!-- ===== بخش پخش‌کننده صوتی ===== -->
<div class="audio-player-container">
    <div class="audio-card">
        <div class="audio-icon">
            <svg viewBox="0 0 24 24" width="32" height="32" fill="currentColor">
                <path d="M12 3v10.55c-.59-.34-1.27-.55-2-.55-2.21 0-4 1.79-4 4s1.79 4 4 4 4-1.79 4-4V7h4V3h-6z"/>
            </svg>
        </div>
        <div class="audio-info">
            <h3 class="audio-title">🎙️ اطلاعات صوتی: فشار خون چیست؟</h3>
            <p class="audio-description">به توضیحات صوتی درباره بیماری فشار خون گوش دهید</p>
        </div>
        <div class="audio-controls">
            <audio id="customAudio" controls style="display:none;">
                <source src="audio/hypertension-guide.mp3" type="audio/mpeg">
                مرورگر شما از پخش صوت پشتیبانی نمی‌کند.
            </audio>
            <div class="custom-player">
                <button class="play-btn" id="playBtn">
                    <svg viewBox="0 0 24 24" width="24" height="24" fill="currentColor">
                        <path d="M8 5v14l11-7z"/>
                    </svg>
                </button>
                <div class="progress-container">
                    <div class="progress-bar" id="progressBar">
                        <div class="progress-fill" id="progressFill"></div>
                    </div>
                    <div class="time-info">
                        <span id="currentTime">0:00</span>
                        <span id="duration">0:00</span>
                    </div>
                </div>
                <button class="volume-btn" id="volumeBtn">
                    <svg viewBox="0 0 24 24" width="20" height="20" fill="currentColor">
                        <path d="M3 9v6h4l5 5V4L7 9H3z"/>
                    </svg>
                </button>
            </div>
        </div>
    </div>
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

            <!-- ===== بخش پخش‌کننده صوتی ===== -->
<div class="audio-player-container">
    <div class="audio-card">
        <div class="audio-icon">
            <svg viewBox="0 0 24 24" width="32" height="32" fill="currentColor">
                <path d="M12 3v10.55c-.59-.34-1.27-.55-2-.55-2.21 0-4 1.79-4 4s1.79 4 4 4 4-1.79 4-4V7h4V3h-6z"/>
            </svg>
        </div>
        <div class="audio-info">
            <h3 class="audio-title">🎙️ اطلاعات صوتی: فشار خون چیست؟</h3>
            <p class="audio-description">به توضیحات صوتی درباره بیماری فشار خون گوش دهید</p>
        </div>
        <div class="audio-controls">
            <audio id="customAudio" controls style="display:none;">
                <source src="audio/hypertension-guide.mp3" type="audio/mpeg">
                مرورگر شما از پخش صوت پشتیبانی نمی‌کند.
            </audio>
            <div class="custom-player">
                <button class="play-btn" id="playBtn">
                    <svg viewBox="0 0 24 24" width="24" height="24" fill="currentColor">
                        <path d="M8 5v14l11-7z"/>
                    </svg>
                </button>
                <div class="progress-container">
                    <div class="progress-bar" id="progressBar">
                        <div class="progress-fill" id="progressFill"></div>
                    </div>
                    <div class="time-info">
                        <span id="currentTime">0:00</span>
                        <span id="duration">0:00</span>
                    </div>
                </div>
                <button class="volume-btn" id="volumeBtn">
                    <svg viewBox="0 0 24 24" width="20" height="20" fill="currentColor">
                        <path d="M3 9v6h4l5 5V4L7 9H3z"/>
                    </svg>
                </button>
            </div>
        </div>
    </div>
</div>
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

            <!-- ===== بخش پخش‌کننده صوتی ===== -->
<div class="audio-player-container">
    <div class="audio-card">
        <div class="audio-icon">
            <svg viewBox="0 0 24 24" width="32" height="32" fill="currentColor">
                <path d="M12 3v10.55c-.59-.34-1.27-.55-2-.55-2.21 0-4 1.79-4 4s1.79 4 4 4 4-1.79 4-4V7h4V3h-6z"/>
            </svg>
        </div>
        <div class="audio-info">
            <h3 class="audio-title">🎙️ اطلاعات صوتی: فشار خون چیست؟</h3>
            <p class="audio-description">به توضیحات صوتی درباره بیماری فشار خون گوش دهید</p>
        </div>
        <div class="audio-controls">
            <audio id="customAudio" controls style="display:none;">
                <source src="audio/hypertension-guide.mp3" type="audio/mpeg">
                مرورگر شما از پخش صوت پشتیبانی نمی‌کند.
            </audio>
            <div class="custom-player">
                <button class="play-btn" id="playBtn">
                    <svg viewBox="0 0 24 24" width="24" height="24" fill="currentColor">
                        <path d="M8 5v14l11-7z"/>
                    </svg>
                </button>
                <div class="progress-container">
                    <div class="progress-bar" id="progressBar">
                        <div class="progress-fill" id="progressFill"></div>
                    </div>
                    <div class="time-info">
                        <span id="currentTime">0:00</span>
                        <span id="duration">0:00</span>
                    </div>
                </div>
                <button class="volume-btn" id="volumeBtn">
                    <svg viewBox="0 0 24 24" width="20" height="20" fill="currentColor">
                        <path d="M3 9v6h4l5 5V4L7 9H3z"/>
                    </svg>
                </button>
            </div>
        </div>
    </div>
</div>
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

            <!-- ===== بخش پخش‌کننده صوتی ===== -->
<div class="audio-player-container">
    <div class="audio-card">
        <div class="audio-icon">
            <svg viewBox="0 0 24 24" width="32" height="32" fill="currentColor">
                <path d="M12 3v10.55c-.59-.34-1.27-.55-2-.55-2.21 0-4 1.79-4 4s1.79 4 4 4 4-1.79 4-4V7h4V3h-6z"/>
            </svg>
        </div>
        <div class="audio-info">
            <h3 class="audio-title">🎙️ اطلاعات صوتی: فشار خون چیست؟</h3>
            <p class="audio-description">به توضیحات صوتی درباره بیماری فشار خون گوش دهید</p>
        </div>
        <div class="audio-controls">
            <audio id="customAudio" controls style="display:none;">
                <source src="audio/hypertension-guide.mp3" type="audio/mpeg">
                مرورگر شما از پخش صوت پشتیبانی نمی‌کند.
            </audio>
            <div class="custom-player">
                <button class="play-btn" id="playBtn">
                    <svg viewBox="0 0 24 24" width="24" height="24" fill="currentColor">
                        <path d="M8 5v14l11-7z"/>
                    </svg>
                </button>
                <div class="progress-container">
                    <div class="progress-bar" id="progressBar">
                        <div class="progress-fill" id="progressFill"></div>
                    </div>
                    <div class="time-info">
                        <span id="currentTime">0:00</span>
                        <span id="duration">0:00</span>
                    </div>
                </div>
                <button class="volume-btn" id="volumeBtn">
                    <svg viewBox="0 0 24 24" width="20" height="20" fill="currentColor">
                        <path d="M3 9v6h4l5 5V4L7 9H3z"/>
                    </svg>
                </button>
            </div>
        </div>
    </div>
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

            <!-- ===== بخش پخش‌کننده صوتی ===== -->
<div class="audio-player-container">
    <div class="audio-card">
        <div class="audio-icon">
            <svg viewBox="0 0 24 24" width="32" height="32" fill="currentColor">
                <path d="M12 3v10.55c-.59-.34-1.27-.55-2-.55-2.21 0-4 1.79-4 4s1.79 4 4 4 4-1.79 4-4V7h4V3h-6z"/>
            </svg>
        </div>
        <div class="audio-info">
            <h3 class="audio-title">🎙️ اطلاعات صوتی: فشار خون چیست؟</h3>
            <p class="audio-description">به توضیحات صوتی درباره بیماری فشار خون گوش دهید</p>
        </div>
        <div class="audio-controls">
            <audio id="customAudio" controls style="display:none;">
                <source src="audio/hypertension-guide.mp3" type="audio/mpeg">
                مرورگر شما از پخش صوت پشتیبانی نمی‌کند.
            </audio>
            <div class="custom-player">
                <button class="play-btn" id="playBtn">
                    <svg viewBox="0 0 24 24" width="24" height="24" fill="currentColor">
                        <path d="M8 5v14l11-7z"/>
                    </svg>
                </button>
                <div class="progress-container">
                    <div class="progress-bar" id="progressBar">
                        <div class="progress-fill" id="progressFill"></div>
                    </div>
                    <div class="time-info">
                        <span id="currentTime">0:00</span>
                        <span id="duration">0:00</span>
                    </div>
                </div>
                <button class="volume-btn" id="volumeBtn">
                    <svg viewBox="0 0 24 24" width="20" height="20" fill="currentColor">
                        <path d="M3 9v6h4l5 5V4L7 9H3z"/>
                    </svg>
                </button>
            </div>
        </div>
    </div>
</div>

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

        <!-- ===== بخش پخش‌کننده صوتی ===== -->
<div class="audio-player-container">
    <div class="audio-card">
        <div class="audio-icon">
            <svg viewBox="0 0 24 24" width="32" height="32" fill="currentColor">
                <path d="M12 3v10.55c-.59-.34-1.27-.55-2-.55-2.21 0-4 1.79-4 4s1.79 4 4 4 4-1.79 4-4V7h4V3h-6z"/>
            </svg>
        </div>
        <div class="audio-info">
            <h3 class="audio-title">🎙️ اطلاعات صوتی: فشار خون چیست؟</h3>
            <p class="audio-description">به توضیحات صوتی درباره بیماری فشار خون گوش دهید</p>
        </div>
        <div class="audio-controls">
            <audio id="customAudio" controls style="display:none;">
                <source src="audio/hypertension-guide.mp3" type="audio/mpeg">
                مرورگر شما از پخش صوت پشتیبانی نمی‌کند.
            </audio>
            <div class="custom-player">
                <button class="play-btn" id="playBtn">
                    <svg viewBox="0 0 24 24" width="24" height="24" fill="currentColor">
                        <path d="M8 5v14l11-7z"/>
                    </svg>
                </button>
                <div class="progress-container">
                    <div class="progress-bar" id="progressBar">
                        <div class="progress-fill" id="progressFill"></div>
                    </div>
                    <div class="time-info">
                        <span id="currentTime">0:00</span>
                        <span id="duration">0:00</span>
                    </div>
                </div>
                <button class="volume-btn" id="volumeBtn">
                    <svg viewBox="0 0 24 24" width="20" height="20" fill="currentColor">
                        <path d="M3 9v6h4l5 5V4L7 9H3z"/>
                    </svg>
                </button>
            </div>
        </div>
    </div>
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

  
// ===== کنترل‌کننده پخش صوتی =====
const audio = document.getElementById('customAudio');
const playBtn = document.getElementById('playBtn');
const progressBar = document.getElementById('progressBar');
const progressFill = document.getElementById('progressFill');
const currentTimeSpan = document.getElementById('currentTime');
const durationSpan = document.getElementById('duration');
const volumeBtn = document.getElementById('volumeBtn');

let isPlaying = false;

// آپدیت دکمه پخش
function updatePlayButton() {
    const svg = playBtn.querySelector('svg');
    if (isPlaying) {
        svg.innerHTML = '<path d="M6 19h4V5H6v14zm8-14v14h4V5h-4z"/>';
    } else {
        svg.innerHTML = '<path d="M8 5v14l11-7z"/>';
    }
}

// پخش/توقف
playBtn.addEventListener('click', () => {
    if (isPlaying) {
        audio.pause();
    } else {
        audio.play();
    }
    isPlaying = !isPlaying;
    updatePlayButton();
});

// آپدیت زمان و پیشرفت
audio.addEventListener('timeupdate', () => {
    const percent = (audio.currentTime / audio.duration) * 100;
    progressFill.style.width = percent + '%';
    
    const currentMin = Math.floor(audio.currentTime / 60);
    const currentSec = Math.floor(audio.currentTime % 60);
    currentTimeSpan.textContent = `${currentMin}:${currentSec.toString().padStart(2, '0')}`;
});

// دریافت مدت زمان فایل
audio.addEventListener('loadedmetadata', () => {
    const durMin = Math.floor(audio.duration / 60);
    const durSec = Math.floor(audio.duration % 60);
    durationSpan.textContent = `${durMin}:${durSec.toString().padStart(2, '0')}`;
});

// کلیک روی نوار پیشرفت
progressBar.addEventListener('click', (e) => {
    const rect = progressBar.getBoundingClientRect();
    const percent = (e.clientX - rect.left) / rect.width;
    audio.currentTime = percent * audio.duration;
});

// کنترل صدا (mute/unmute)
let isMuted = false;
let lastVolume = 1;

volumeBtn.addEventListener('click', () => {
    if (isMuted) {
        audio.volume = lastVolume;
        isMuted = false;
        volumeBtn.style.opacity = '1';
    } else {
        lastVolume = audio.volume;
        audio.volume = 0;
        isMuted = true;
        volumeBtn.style.opacity = '0.5';
    }
});

// پایان آهنگ
audio.addEventListener('ended', () => {
    isPlaying = false;
    updatePlayButton();
    progressFill.style.width = '0%';
    currentTimeSpan.textContent = '0:00';
});
</script>

</body>
</html>
