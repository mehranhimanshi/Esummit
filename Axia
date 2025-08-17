<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AXIA Dating App - UI/UX Mockups</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 50%, #f093fb 100%);
            background-attachment: fixed;
            min-height: 100vh;
            overflow-x: auto;
            color: #1a1a1a;
        }
        
        .floating-particles {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: -1;
        }
        
        .particle {
            position: absolute;
            background: rgba(255, 255, 255, 0.1);
            border-radius: 50%;
            animation: float 6s ease-in-out infinite;
        }
        
        .particle:nth-child(1) { left: 20%; animation-delay: 0s; width: 10px; height: 10px; }
        .particle:nth-child(2) { left: 50%; animation-delay: 2s; width: 15px; height: 15px; }
        .particle:nth-child(3) { left: 80%; animation-delay: 4s; width: 8px; height: 8px; }
        
        @keyframes float {
            0%, 100% { transform: translateY(0px) rotate(0deg); opacity: 0.3; }
            50% { transform: translateY(-30px) rotate(180deg); opacity: 0.8; }
        }
        
        .container {
            max-width: 1400px;
            margin: 0 auto;
            padding: 40px 20px;
        }
        
        .header {
            text-align: center;
            margin-bottom: 60px;
            padding: 40px;
            background: rgba(255, 255, 255, 0.15);
            backdrop-filter: blur(20px);
            border-radius: 30px;
            border: 1px solid rgba(255, 255, 255, 0.2);
            box-shadow: 0 20px 40px rgba(0,0,0,0.1);
        }
        
        .app-title {
            font-size: 4rem;
            font-weight: 900;
            color: white;
            text-shadow: 0 8px 16px rgba(0,0,0,0.3);
            letter-spacing: 3px;
            margin-bottom: 15px;
            background: linear-gradient(135deg, #ffffff, #f0f0f0);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }
        
        .tagline {
            font-size: 2rem;
            font-style: italic;
            font-weight: 300;
            color: white;
            text-shadow: 0 4px 8px rgba(0,0,0,0.3);
            letter-spacing: 1px;
        }
        
        .section-title {
            font-size: 2.5rem;
            font-weight: 700;
            text-align: center;
            margin-bottom: 50px;
            color: white;
            text-shadow: 0 4px 8px rgba(0,0,0,0.3);
            position: relative;
        }
        
        .section-title::after {
            content: '';
            position: absolute;
            bottom: -15px;
            left: 50%;
            transform: translateX(-50%);
            width: 100px;
            height: 4px;
            background: linear-gradient(90deg, #ff6b9d, #ffb3d1);
            border-radius: 2px;
        }
        
        .mockups-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 40px;
            margin-bottom: 80px;
        }
        
        .phone-mockup {
            background: linear-gradient(145deg, #2a2a2a, #1a1a1a);
            border-radius: 40px;
            padding: 25px;
            width: 350px;
            height: 700px;
            margin: 0 auto;
            box-shadow: 0 30px 60px rgba(0,0,0,0.4), 0 0 0 1px rgba(255,255,255,0.1);
            position: relative;
            overflow: hidden;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        
        .phone-mockup::before {
            content: '';
            position: absolute;
            top: 15px;
            left: 50%;
            transform: translateX(-50%);
            width: 60px;
            height: 6px;
            background: #333;
            border-radius: 3px;
        }
        
        .phone-mockup::after {
            content: '';
            position: absolute;
            bottom: 15px;
            left: 50%;
            transform: translateX(-50%);
            width: 40px;
            height: 4px;
            background: #333;
            border-radius: 2px;
        }
        
        .phone-mockup:hover {
            transform: translateY(-10px) scale(1.02);
            box-shadow: 0 40px 80px rgba(0,0,0,0.5), 0 0 0 1px rgba(255,255,255,0.2);
        }
        
        .phone-screen {
            background: linear-gradient(180deg, #ffffff 0%, #f8f9fa 100%);
            border-radius: 25px;
            width: 100%;
            height: 100%;
            overflow: hidden;
            position: relative;
            box-shadow: inset 0 1px 3px rgba(0,0,0,0.1);
        }
        
        .status-bar {
            height: 50px;
            background: rgba(248, 249, 250, 0.9);
            backdrop-filter: blur(10px);
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 0 25px;
            font-size: 0.9rem;
            font-weight: 600;
            border-bottom: 1px solid rgba(0,0,0,0.05);
            color: #333;
        }
        
        .screen-content {
            height: calc(100% - 50px);
            padding: 25px;
            overflow-y: auto;
            background: linear-gradient(180deg, rgba(255,255,255,0.9) 0%, rgba(248,249,250,0.9) 100%);
        }
        
        .feature-title {
            font-size: 1.3rem;
            font-weight: 700;
            margin-bottom: 20px;
            color: #2c3e50;
            text-align: center;
            background: linear-gradient(135deg, #667eea, #764ba2);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }
        
        /* Screenshot Protection Styles */
        .screenshot-alert {
            background: linear-gradient(135deg, #ff6b9d, #ff8fab);
            color: white;
            padding: 25px;
            border-radius: 20px;
            text-align: center;
            box-shadow: 0 10px 30px rgba(255, 107, 157, 0.3);
            margin-bottom: 20px;
        }
        
        .shield-icon {
            font-size: 3rem;
            margin-bottom: 15px;
            filter: drop-shadow(0 4px 8px rgba(0,0,0,0.2));
        }
        
        .alert-text {
            font-size: 1.2rem;
            font-weight: 700;
            margin-bottom: 10px;
        }
        
        .alert-subtext {
            font-size: 0.9rem;
            opacity: 0.9;
        }
        
        /* Bot Detection Styles */
        .bot-detection {
            text-align: center;
            padding: 25px;
            background: linear-gradient(135deg, #ff9a9e, #fecfef);
            border-radius: 20px;
            box-shadow: 0 10px 30px rgba(255, 154, 158, 0.3);
            margin-bottom: 20px;
        }
        
        .scan-animation {
            width: 80px;
            height: 80px;
            border: 4px solid rgba(255,255,255,0.3);
            border-top: 4px solid white;
            border-radius: 50%;
            animation: spin 2s linear infinite;
            margin: 0 auto 20px;
        }
        
        @keyframes spin {
            0% { transform: rotate(0deg); }
            100% { transform: rotate(360deg); }
        }
        
        .detection-result {
            margin-top: 20px;
            padding: 15px;
            background: rgba(255,255,255,0.2);
            border-radius: 12px;
            backdrop-filter: blur(10px);
        }
        
        /* Verification Styles */
        .verification-steps {
            margin-bottom: 25px;
        }
        
        .step {
            display: flex;
            align-items: center;
            padding: 20px;
            margin-bottom: 15px;
            background: rgba(255,255,255,0.7);
            border-radius: 15px;
            border-left: 4px solid #e0e0e0;
            box-shadow: 0 4px 15px rgba(0,0,0,0.05);
            transition: all 0.3s ease;
        }
        
        .step.completed {
            border-left-color: #4caf50;
            background: rgba(76, 175, 80, 0.1);
        }
        
        .step-number {
            width: 40px;
            height: 40px;
            border-radius: 50%;
            background: #e0e0e0;
            color: white;
            display: flex;
            align-items: center;
            justify-content: center;
            font-weight: bold;
            margin-right: 15px;
        }
        
        .step.completed .step-number {
            background: linear-gradient(135deg, #4caf50, #66bb6a);
        }
        
        .verified-badge {
            text-align: center;
            padding: 15px;
            background: linear-gradient(135deg, #4caf50, #66bb6a);
            color: white;
            border-radius: 12px;
            font-weight: 600;
            box-shadow: 0 8px 20px rgba(76, 175, 80, 0.3);
        }
        
        /* Plan Card Styles */
        .plan-card {
            background: linear-gradient(135deg, #667eea, #764ba2);
            color: white;
            padding: 25px;
            border-radius: 20px;
            margin-bottom: 20px;
            box-shadow: 0 15px 35px rgba(102, 126, 234, 0.3);
            transition: transform 0.3s ease;
        }
        
        .plan-card:hover {
            transform: translateY(-5px);
        }
        
        .plan-card h3 {
            font-size: 1.4rem;
            margin-bottom: 10px;
            text-align: center;
        }
        
        .plan-price {
            font-size: 2.5rem;
            font-weight: 700;
            text-align: center;
            margin-bottom: 20px;
        }
        
        .plan-features {
            list-style: none;
        }
        
        .plan-features li {
            padding: 8px 0;
            padding-left: 25px;
            position: relative;
        }
        
        .plan-features li::before {
            content: '✓';
            position: absolute;
            left: 0;
            color: #4caf50;
            font-weight: bold;
        }
        
        .plan-lite {
            background: linear-gradient(135deg, #f093fb, #f5576c);
        }
        
        /* Chat Interface Styles */
        .chat-interface {
            background: white;
            border-radius: 20px;
            overflow: hidden;
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
            height: 400px;
            display: flex;
            flex-direction: column;
        }
        
        .chat-header {
            background: linear-gradient(135deg, #667eea, #764ba2);
            color: white;
            padding: 15px 20px;
            font-weight: 600;
            text-align: center;
        }
        
        .ghost-warning {
            background: linear-gradient(135deg, #ffd54f, #ff8f00);
            color: #333;
            padding: 12px 20px;
            text-align: center;
            font-size: 0.9rem;
            font-weight: 600;
        }
        
        .chat-actions {
            padding: 15px;
            background: #f8f9fa;
            display: flex;
            gap: 10px;
        }
        
        .action-btn {
            flex: 1;
            padding: 12px;
            border: none;
            border-radius: 12px;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s ease;
        }
        
        .remind-btn {
            background: linear-gradient(135deg, #4caf50, #66bb6a);
            color: white;
        }
        
        .polite-exit {
            background: linear-gradient(135deg, #ff7043, #ff8a65);
            color: white;
        }
        
        /* Just Friend Mode Styles */
        .friend-mode-toggle {
            background: white;
            border-radius: 20px;
            padding: 20px;
            margin-bottom: 20px;
            box-shadow: 0 8px 25px rgba(0,0,0,0.1);
        }
        
        .toggle-header {
            text-align: center;
            font-weight: 600;
            margin-bottom: 15px;
            color: #666;
        }
        
        .mode-options {
            display: flex;
            gap: 10px;
        }
        
        .mode-option {
            flex: 1;
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 15px 10px;
            border-radius: 12px;
            background: #f8f9fa;
            cursor: pointer;
            transition: all 0.3s ease;
        }
        
        .mode-option.active {
            background: linear-gradient(135deg, #4caf50, #66bb6a);
            color: white;
            transform: scale(1.05);
        }
        
        .mode-icon {
            font-size: 1.5rem;
            margin-bottom: 8px;
        }
        
        .friend-benefits {
            background: rgba(76, 175, 80, 0.1);
            border-radius: 15px;
            padding: 20px;
            margin-bottom: 20px;
        }
        
        .benefit-item {
            display: flex;
            align-items: center;
            margin-bottom: 12px;
            font-size: 0.9rem;
        }
        
        .benefit-icon {
            margin-right: 12px;
            font-size: 1.2rem;
        }
        
        /* AI Matchmaking Styles */
        .ai-analysis {
            display: flex;
            align-items: center;
            background: linear-gradient(135deg, #667eea, #764ba2);
            color: white;
            padding: 20px;
            border-radius: 20px;
            margin-bottom: 25px;
            text-align: center;
        }
        
        .ai-brain {
            font-size: 3rem;
            margin-right: 15px;
            animation: pulse 2s infinite;
        }
        
        @keyframes pulse {
            0%, 100% { transform: scale(1); }
            50% { transform: scale(1.1); }
        }
        
        .compatibility-score {
            background: white;
            border-radius: 20px;
            padding: 25px;
            text-align: center;
            box-shadow: 0 8px 25px rgba(0,0,0,0.1);
            margin-bottom: 20px;
        }
        
        .score-circle {
            width: 100px;
            height: 100px;
            border-radius: 50%;
            background: conic-gradient(from 0deg, #4caf50 0deg 338.4deg, #e0e0e0 338.4deg 360deg);
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            margin: 0 auto 20px;
            position: relative;
        }
        
        .score-circle::before {
            content: '';
            position: absolute;
            width: 70px;
            height: 70px;
            background: white;
            border-radius: 50%;
        }
        
        .score-number {
            font-size: 1.8rem;
            font-weight: bold;
            color: #4caf50;
            z-index: 1;
        }
        
        .score-label {
            font-size: 0.8rem;
            color: #666;
            z-index: 1;
        }
        
        .score-details {
            text-align: left;
        }
        
        .detail-item {
            margin-bottom: 10px;
        }
        
        .progress-bar {
            width: 100%;
            height: 8px;
            background: #e0e0e0;
            border-radius: 4px;
            overflow: hidden;
            margin-top: 4px;
        }
        
        .progress {
            height: 100%;
            background: linear-gradient(90deg, #4caf50, #66bb6a);
            border-radius: 4px;
            transition: width 2s ease;
        }
        
        /* Safe Meetup Mode Styles */
        .meetup-planning {
            background: white;
            border-radius: 20px;
            padding: 25px;
            box-shadow: 0 8px 25px rgba(0,0,0,0.1);
            margin-bottom: 20px;
        }
        
        .meetup-header {
            text-align: center;
            padding: 15px;
            background: linear-gradient(135deg, #ff6b9d, #ffb3d1);
            color: white;
            border-radius: 12px;
            margin-bottom: 20px;
        }
        
        .safety-features {
            margin-bottom: 25px;
        }
        
        .safety-item {
            display: flex;
            align-items: center;
            margin-bottom: 15px;
            padding: 15px;
            background: rgba(102, 126, 234, 0.1);
            border-radius: 12px;
        }
        
        .safety-icon {
            font-size: 1.8rem;
            margin-right: 15px;
            width: 40px;
            text-align: center;
        }
        
        .meetup-btn {
            width: 100%;
            padding: 15px;
            background: linear-gradient(135deg, #4caf50, #66bb6a);
            color: white;
            border: none;
            border-radius: 15px;
            font-size: 1.1rem;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s ease;
        }
        
        .meetup-btn:hover {
            transform: translateY(-2px);
            box-shadow: 0 8px 20px rgba(76, 175, 80, 0.3);
        }
        
        /* Enhanced boxes and alerts */
        .info-box {
            padding: 20px;
            border-radius: 15px;
            margin: 15px 0;
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255,255,255,0.2);
        }
        
        .success-box {
            background: rgba(76, 175, 80, 0.15);
            border-left: 4px solid #4caf50;
        }
        
        .warning-box {
            background: rgba(255, 193, 7, 0.15);
            border-left: 4px solid #ffc107;
        }
        
        .premium-box {
            background: rgba(103, 58, 183, 0.15);
            border-left: 4px solid #673ab7;
        }
    </style>
</head>
<body>
    <div class="floating-particles">
        <div class="particle"></div>
        <div class="particle"></div>
        <div class="particle"></div>
    </div>
    
    <div class="container">
        <div class="header">
            <div class="app-title">AXIA</div>
            <div class="tagline">Swipe less. Connect more.</div>
            <!-- Just Friend Mode -->
            <div class="phone-mockup">
                <div class="phone-screen">
                    <div class="status-bar">
                        <span>9:41</span>
                        <span>🔋 100%</span>
                    </div>
                    <div class="screen-content">
                        <div class="feature-title">Just Friend Mode</div>
                        
                        <div class="friend-mode-toggle">
                            <div class="toggle-header">Looking for:</div>
                            <div class="mode-options">
                                <div class="mode-option">
                                    <div class="mode-icon">💕</div>
                                    <span>Dating</span>
                                </div>
                                <div class="mode-option active">
                                    <div class="mode-icon">👥</div>
                                    <span>Friends</span>
                                </div>
                                <div class="mode-option">
                                    <div class="mode-icon">💼</div>
                                    <span>Networking</span>
                                </div>
                            </div>
                        </div>
                        
                        <div class="friend-benefits">
                            <div class="benefit-item">
                                <span class="benefit-icon">🎯</span>
                                <span>Platonic connections only</span>
                            </div>
                            <div class="benefit-item">
                                <span class="benefit-icon">🏃‍♀️</span>
                                <span>Find workout buddies</span>
                            </div>
                            <div class="benefit-item">
                                <span class="benefit-icon">🎨</span>
                                <span>Connect over hobbies</span>
                            </div>
                            <div class="benefit-item">
                                <span class="benefit-icon">🌍</span>
                                <span>Meet locals & travelers</span>
                            </div>
                        </div>
                        
                        <div class="info-box success-box" style="text-align: center;">
                            <strong>🤝 Pure Friendship Zone</strong>
                        </div>
                    </div>
                </div>
            </div>
            
            <!-- AI Matchmaking -->
            <div class="phone-mockup">
                <div class="phone-screen">
                    <div class="status-bar">
                        <span>9:41</span>
                        <span>🔋 100%</span>
                    </div>
                    <div class="screen-content">
                        <div class="feature-title">AI Matchmaking</div>
                        
                        <div class="ai-analysis">
                            <div class="ai-brain">🧠</div>
                            <div class="analysis-text">
                                <strong>AI analyzing your preferences...</strong><br>
                                <small>Processing 127 compatibility factors</small>
                            </div>
                        </div>
                        
                        <div class="compatibility-score">
                            <div class="score-circle">
                                <div class="score-number">94%</div>
                                <div class="score-label">Match</div>
                            </div>
                            <div class="score-details">
                                <div class="detail-item">
                                    <span>Shared Interests:</span>
                                    <div class="progress-bar">
                                        <div class="progress" style="width: 85%"></div>
                                    </div>
                                </div>
                                <div class="detail-item">
                                    <span>Lifestyle:</span>
                                    <div class="progress-bar">
                                        <div class="progress" style="width: 92%"></div>
                                    </div>
                                </div>
                                <div class="detail-item">
                                    <span>Values:</span>
                                    <div class="progress-bar">
                                        <div class="progress" style="width: 78%"></div>
                                    </div>
                                </div>
                            </div>
                        </div>
                        
                        <div class="info-box premium-box">
                            <strong>🤖 Smart Learning:</strong> Gets better with every interaction
                        </div>
                    </div>
                </div>
            </div>
            
            <!-- Safe Meetup Mode -->
            <div class="phone-mockup">
                <div class="phone-screen">
                    <div class="status-bar">
                        <span>9:41</span>
                        <span>🔋 100%</span>
                    </div>
                    <div class="screen-content">
                        <div class="feature-title">Safe Meetup Mode</div>
                        
                        <div class="meetup-planning">
                            <div class="meetup-header">
                                <strong>📍 First Date with Aarav</strong>
                            </div>
                            
                            <div class="safety-features">
                                <div class="safety-item">
                                    <div class="safety-icon">👥</div>
                                    <div class="safety-text">
                                        <strong>Verified Public Location</strong><br>
                                        <small>Coffee shops, restaurants only</small>
                                    </div>
                                </div>
                                
                                <div class="safety-item">
                                    <div class="safety-icon">🕐</div>
                                    <div class="safety-text">
                                        <strong>Time-Limited Meetup</strong><br>
                                        <small>Auto check-in every 30 mins</small>
                                    </div>
                                </div>
                                
                                <div class="safety-item">
                                    <div class="safety-icon">📞</div>
                                    <div class="safety-text">
                                        <strong>Emergency Contacts</strong><br>
                                        <small>Share location with trusted friends</small>
                                    </div>
                                </div>
                            </div>
                            
                            <button class="meetup-btn">
                                🛡️ Activate Safe Mode
                            </button>
                        </div>
                        
                        <div class="info-box success-box">
                            <strong>✅ 99.8% Safe Meetup Rate</strong>
                        </div>
                    </div>
                </div>
            </div>
        
        <h2 class="section-title">Core Safety Features</h2>
        
        <div class="mockups-grid">
            <!-- Screenshot Protection -->
            <div class="phone-mockup">
                <div class="phone-screen">
                    <div class="status-bar">
                        <span>9:41</span>
                        <span>🔋 100%</span>
                    </div>
                    <div class="screen-content">
                        <div class="feature-title">Screenshot Protection</div>
                        <div class="screenshot-alert">
                            <div class="shield-icon">🛡️</div>
                            <div class="alert-text">Screenshot Blocked!</div>
                            <div class="alert-subtext">Aarav was notified that someone tried to screenshot your conversation</div>
                        </div>
                        <div class="info-box success-box">
                            <strong>✅ Privacy Protected</strong><br>
                            <small>Your photos and messages are safe from unauthorized screenshots</small>
                        </div>
                    </div>
                </div>
            </div>
            
            <!-- AI Bot Detection -->
            <div class="phone-mockup">
                <div class="phone-screen">
                    <div class="status-bar">
                        <span>9:41</span>
                        <span>🔋 100%</span>
                    </div>
                    <div class="screen-content">
                        <div class="feature-title">AI Bot Detection</div>
                        <div class="bot-detection">
                            <div class="scan-animation"></div>
                            <div style="text-align: center; color: white;">
                                <strong>Scanning Profile...</strong><br>
                                <small>Analyzing messaging patterns & suspicious links</small>
                            </div>
                            <div class="detection-result">
                                <strong>⚠️ Bot Detected!</strong><br>
                                <small>This profile has been automatically removed for suspicious activity</small>
                            </div>
                        </div>
                        <div class="info-box success-box" style="text-align: center;">
                            <strong>Real humans only! 🎯</strong>
                        </div>
                    </div>
                </div>
            </div>
            
            <!-- Multi-Step Verification -->
            <div class="phone-mockup">
                <div class="phone-screen">
                    <div class="status-bar">
                        <span>9:41</span>
                        <span>🔋 100%</span>
                    </div>
                    <div class="screen-content">
                        <div class="feature-title">Profile Verification</div>
                        <div class="verification-steps">
                            <div class="step completed">
                                <div class="step-number">1</div>
                                <div>
                                    <strong>Live Selfie Video</strong><br>
                                    <small>Record a 5-second selfie video</small>
                                </div>
                            </div>
                            <div class="step completed">
                                <div class="step-number">2</div>
                                <div>
                                    <strong>ID Verification</strong><br>
                                    <small>Upload government-issued ID</small>
                                </div>
                            </div>
                            <div class="step">
                                <div class="step-number">3</div>
                                <div>
                                    <strong>Manual Review</strong><br>
                                    <small>Our team verifies your submission</small>
                                </div>
                            </div>
                        </div>
                        <div class="verified-badge">
                            ✅ Verified Profile - 3x more visibility!
                        </div>
                    </div>
                </div>
            </div>
        </div>
        
        <h2 class="section-title">Enhanced User Experience</h2>
        
        <div class="mockups-grid">
            <!-- Cheaper Premium Plans -->
            <div class="phone-mockup">
                <div class="phone-screen">
                    <div class="status-bar">
                        <span>9:41</span>
                        <span>🔋 100%</span>
                    </div>
                    <div class="screen-content">
                        <div class="feature-title">Affordable Premium</div>
                        
                        <div class="plan-card plan-lite">
                            <h3>AXIA Lite</h3>
                            <div class="plan-price">₹99/mo</div>
                            <ul class="plan-features">
                                <li>5 Super Likes daily</li>
                                <li>3 Boosts per month</li>
                                <li>See who likes you</li>
                                <li>Ad-free experience</li>
                            </ul>
                        </div>
                        
                        <div class="info-box premium-box">
                            <strong>🎓 Student Discount: 50% OFF</strong><br>
                            <small>Verify with your .edu email</small>
                        </div>
                        
                        <div class="plan-card">
                            <h3>AXIA Premium</h3>
                            <div class="plan-price">₹199/mo</div>
                            <small>Everything in Lite + unlimited likes & rewinds</small>
                        </div>
                    </div>
                </div>
            </div>
            
            <!-- Anti-Ghosting Mode -->
            <div class="phone-mockup">
                <div class="phone-screen">
                    <div class="status-bar">
                        <span>9:41</span>
                        <span>🔋 100%</span>
                    </div>
                    <div class="screen-content">
                        <div class="feature-title">Anti-Ghosting Mode</div>
                        
                        <div class="chat-interface">
                            <div class="chat-header">
                                Chat with Aarav
                            </div>
                            <div class="ghost-warning">
                                ⏰ No reply in 2 days - Chat expires in 3 days
                            </div>
                            <div style="flex: 1; padding: 15px;">
                                <div style="background: linear-gradient(135deg, #e3f2fd, #bbdefb); padding: 15px; border-radius: 20px; margin: 10px 0; box-shadow: 0 4px 15px rgba(0,0,0,0.1);">
                                    Hey! How's your weekend going?
                                </div>
                                <div style="text-align: center; color: #999; margin: 20px 0;">
                                    <small>Waiting for response...</small>
                                </div>
                            </div>
                            <div class="chat-actions">
                                <button class="action-btn remind-btn">Send Reminder</button>
                                <button class="action-btn polite-exit">Polite Exit</button>
                            </div>
                        </div>
                        
                        <div class="info-box warning-box" style="font-size: 0.9rem;">
                            💡 <strong>Ghosting Score:</strong> Hidden metric affects match priority
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</body>
</html>
