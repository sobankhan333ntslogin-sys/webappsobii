/* ===== CSS Reset & Base ===== */
*,
*::before,
*::after {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
:root {
  --bg-primary: #0a0a0f;
  --bg-secondary: #12121a;
  --bg-card: rgba(18, 18, 30, 0.85);
  --border-card: rgba(139, 92, 246, 0.15);
  --text-primary: #f0f0f5;
  --text-secondary: #9898b0;
  --accent-purple: #a78bfa;
  --accent-pink: #f472b6;
  --accent-violet: #8b5cf6;
  --accent-indigo: #6366f1;
  --gradient-main: linear-gradient(135deg, #8b5cf6, #a78bfa, #f472b6);
  --gradient-btn: linear-gradient(135deg, #8b5cf6, #6366f1);
  --gradient-yes: linear-gradient(135deg, #10b981, #34d399);
  --gradient-no: linear-gradient(135deg, #ef4444, #f87171);
  --shadow-glow: 0 0 40px rgba(139, 92, 246, 0.15);
  --shadow-card: 0 25px 60px rgba(0, 0, 0, 0.5);
  --radius-lg: 24px;
  --radius-md: 16px;
  --radius-sm: 12px;
  --transition-smooth: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
}
body {
  font-family: 'Outfit', sans-serif;
  background: var(--bg-primary);
  color: var(--text-primary);
  min-height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
  overflow: hidden;
  position: relative;
}
body::before {
  content: '';
  position: fixed;
  top: -50%;
  left: -50%;
  width: 200%;
  height: 200%;
  background: 
    radial-gradient(circle at 20% 30%, rgba(139, 92, 246, 0.08) 0%, transparent 50%),
    radial-gradient(circle at 80% 70%, rgba(244, 114, 182, 0.06) 0%, transparent 50%),
    radial-gradient(circle at 50% 50%, rgba(99, 102, 241, 0.04) 0%, transparent 60%);
  animation: bgDrift 20s ease-in-out infinite alternate;
  z-index: 0;
}
@keyframes bgDrift {
  0% { transform: translate(0, 0) rotate(0deg); }
  100% { transform: translate(-30px, -20px) rotate(3deg); }
}
/* ===== Floating Particles ===== */
.particles {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  z-index: 0;
  pointer-events: none;
}
.particle {
  position: absolute;
  border-radius: 50%;
  opacity: 0;
  animation: floatParticle linear infinite;
}
@keyframes floatParticle {
  0% {
    opacity: 0;
    transform: translateY(100vh) scale(0);
  }
  10% {
    opacity: 1;
  }
  90% {
    opacity: 1;
  }
  100% {
    opacity: 0;
    transform: translateY(-10vh) scale(1);
  }
}
/* ===== Card Container ===== */
.card {
  position: relative;
  z-index: 10;
  background: var(--bg-card);
  border: 1px solid var(--border-card);
  border-radius: var(--radius-lg);
  padding: 48px 40px;
  max-width: 520px;
  width: 90vw;
  text-align: center;
  backdrop-filter: blur(20px);
  box-shadow: var(--shadow-card), var(--shadow-glow);
  position: absolute;
}
.card::before {
  content: '';
  position: absolute;
  top: 0;
  left: 50%;
  transform: translateX(-50%);
  width: 60%;
  height: 1px;
  background: linear-gradient(90deg, transparent, var(--accent-purple), transparent);
}
/* ===== Step Transitions ===== */
.step {
  opacity: 0;
  transform: translateY(30px) scale(0.95);
  pointer-events: none;
  transition: opacity 0.6s cubic-bezier(0.4, 0, 0.2, 1),
              transform 0.6s cubic-bezier(0.4, 0, 0.2, 1);
}
.step.active {
  opacity: 1;
  transform: translateY(0) scale(1);
  pointer-events: all;
}
.step.exit {
  opacity: 0;
  transform: translateY(-30px) scale(0.95);
  pointer-events: none;
}
/* ===== Typography ===== */
.sparkle-icon {
  font-size: 48px;
  margin-bottom: 16px;
  animation: sparkleFloat 3s ease-in-out infinite;
}
.big-icon {
  font-size: 64px;
}
@keyframes sparkleFloat {
  0%, 100% { transform: translateY(0); }
  50% { transform: translateY(-8px); }
}
.title {
  font-size: 2rem;
  font-weight: 700;
  margin-bottom: 8px;
  letter-spacing: -0.5px;
  line-height: 1.2;
}
.fancy-title {
  font-size: 2.2rem;
}
.congrats-title {
  font-size: 2.4rem;
  background: var(--gradient-main);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}
.highlight {
  background: var(--gradient-main);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
  font-weight: 800;
}
.subtitle {
  color: var(--text-secondary);
  font-size: 1rem;
  font-weight: 400;
  margin-bottom: 28px;
  line-height: 1.5;
}
/* ===== Rules Box ===== */
.rules-box {
  background: rgba(139, 92, 246, 0.06);
  border: 1px solid rgba(139, 92, 246, 0.1);
  border-radius: var(--radius-md);
  padding: 20px 24px;
  margin-bottom: 28px;
  text-align: left;
}
.rule {
  display: flex;
  align-items: center;
  gap: 14px;
  padding: 10px 0;
}
.rule + .rule {
  border-top: 1px solid rgba(139, 92, 246, 0.07);
}
.rule-number {
  font-size: 0.75rem;
  font-weight: 700;
  color: var(--accent-purple);
  background: rgba(139, 92, 246, 0.12);
  width: 32px;
  height: 32px;
  border-radius: 8px;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-shrink: 0;
}
.rule-text {
  color: var(--text-secondary);
  font-size: 0.92rem;
  font-weight: 400;
}
/* ===== Option Buttons ===== */
.choose-text {
  color: var(--text-secondary);
  font-size: 0.9rem;
  margin-bottom: 14px;
  font-weight: 500;
}
.options-grid {
  display: flex;
  gap: 12px;
  margin-bottom: 24px;
  justify-content: center;
}
.option-btn {
  flex: 1;
  max-width: 140px;
  background: rgba(139, 92, 246, 0.06);
  border: 2px solid rgba(139, 92, 246, 0.12);
  border-radius: var(--radius-sm);
  padding: 18px 12px;
  cursor: pointer;
  transition: var(--transition-smooth);
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 8px;
  color: var(--text-primary);
  font-family: 'Outfit', sans-serif;
}
.option-btn:hover {
  border-color: var(--accent-purple);
  background: rgba(139, 92, 246, 0.1);
  transform: translateY(-3px);
  box-shadow: 0 8px 25px rgba(139, 92, 246, 0.15);
}
.option-btn.selected {
  border-color: var(--accent-purple);
  background: rgba(139, 92, 246, 0.15);
  box-shadow: 0 0 20px rgba(139, 92, 246, 0.2);
}
.option-emoji {
  font-size: 1.6rem;
}
.option-label {
  font-size: 0.85rem;
  font-weight: 500;
  color: var(--text-secondary);
}
.option-btn.selected .option-label {
  color: var(--accent-purple);
}
/* ===== Proceed Button ===== */
.proceed-btn {
  display: inline-flex;
  align-items: center;
  gap: 10px;
  padding: 14px 36px;
  border: none;
  border-radius: 50px;
  font-family: 'Outfit', sans-serif;
  font-size: 1rem;
  font-weight: 600;
  color: white;
  background: var(--gradient-btn);
  cursor: pointer;
  transition: var(--transition-smooth);
  position: relative;
  overflow: hidden;
}
.proceed-btn::before {
  content: '';
  position: absolute;
  top: 0;
  left: -100%;
  width: 100%;
  height: 100%;
  background: linear-gradient(90deg, transparent, rgba(255,255,255,0.15), transparent);
  transition: left 0.5s;
}
.proceed-btn:hover::before {
  left: 100%;
}
.proceed-btn:hover {
  transform: translateY(-2px);
  box-shadow: 0 12px 30px rgba(139, 92, 246, 0.35);
}
.proceed-btn.disabled {
  opacity: 0.4;
  cursor: not-allowed;
  pointer-events: none;
}
/* ===== Friendship Buttons ===== */
.friendship-buttons {
  display: flex;
  gap: 20px;
  justify-content: center;
  margin-top: 10px;
  margin-bottom: 16px;
}
.yes-btn,
.no-btn {
  display: flex;
  align-items: center;
  gap: 10px;
  padding: 16px 40px;
  border: none;
  border-radius: 50px;
  font-family: 'Outfit', sans-serif;
  font-size: 1.1rem;
  font-weight: 600;
  color: white;
  cursor: pointer;
  transition: var(--transition-smooth);
  position: relative;
}
.btn-emoji {
  font-size: 1.3rem;
}
.yes-btn {
  background: var(--gradient-yes);
  box-shadow: 0 6px 20px rgba(16, 185, 129, 0.25);
}
.yes-btn:hover {
  transform: translateY(-3px) scale(1.05);
  box-shadow: 0 12px 35px rgba(16, 185, 129, 0.4);
}
.yes-btn:active {
  transform: translateY(-1px) scale(1.02);
}
.no-btn {
  background: var(--gradient-no);
  box-shadow: 0 6px 20px rgba(239, 68, 68, 0.25);
  position: absolute;
  transition: none;
}
.hint-text {
  color: var(--accent-pink);
  font-size: 0.9rem;
  font-weight: 500;
  min-height: 24px;
  margin-top: 8px;
  opacity: 0;
  transition: opacity 0.3s ease;
}
.hint-text.show {
  opacity: 1;
  animation: hintPulse 2s ease-in-out infinite;
}
@keyframes hintPulse {
  0%, 100% { opacity: 0.7; }
  50% { opacity: 1; }
}
/* ===== Congratulations ===== */
.friends-badge {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 16px;
  margin: 24px 0 12px;
  padding: 20px 32px;
  background: rgba(139, 92, 246, 0.08);
  border: 1px solid rgba(139, 92, 246, 0.15);
  border-radius: 60px;
}
.friend-name {
  font-size: 1.5rem;
  font-weight: 700;
  background: var(--gradient-main);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}
.heart-icon {
  font-size: 2rem;
  animation: heartBeat 1.2s ease-in-out infinite;
}
@keyframes heartBeat {
  0%, 100% { transform: scale(1); }
  15% { transform: scale(1.25); }
  30% { transform: scale(1); }
  45% { transform: scale(1.15); }
  60% { transform: scale(1); }
}
.congrats-text {
  font-size: 1.2rem;
  color: var(--text-secondary);
  font-weight: 400;
  margin-bottom: 24px;
}
.celebration-emojis {
  display: flex;
  justify-content: center;
  gap: 16px;
  font-size: 2rem;
}
.celebration-emojis span {
  animation: celebrationBounce 0.6s ease-in-out infinite alternate;
}
.celebration-emojis span:nth-child(1) { animation-delay: 0s; }
.celebration-emojis span:nth-child(2) { animation-delay: 0.1s; }
.celebration-emojis span:nth-child(3) { animation-delay: 0.2s; }
.celebration-emojis span:nth-child(4) { animation-delay: 0.3s; }
.celebration-emojis span:nth-child(5) { animation-delay: 0.4s; }
@keyframes celebrationBounce {
  0% { transform: translateY(0); }
  100% { transform: translateY(-12px); }
}
/* ===== Confetti ===== */
.confetti-container {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  pointer-events: none;
  overflow: hidden;
  border-radius: var(--radius-lg);
}
.confetti-piece {
  position: absolute;
  top: -10px;
  opacity: 0;
  animation: confettiFall linear forwards;
}
@keyframes confettiFall {
  0% {
    opacity: 1;
    transform: translateY(0) rotate(0deg) scale(1);
  }
  100% {
    opacity: 0;
    transform: translateY(500px) rotate(720deg) scale(0.5);
  }
}
/* ===== Responsive ===== */
@media (max-width: 600px) {
  body {
    padding: 16px;
    align-items: flex-start;
    padding-top: 10vh;
  }
  .card {
    padding: 32px 20px;
    border-radius: 20px;
    width: 100%;
    max-width: 100%;
  }
  .sparkle-icon {
    font-size: 40px;
  }
  .big-icon {
    font-size: 52px;
  }
  .title {
    font-size: 1.5rem;
  }
  .fancy-title {
    font-size: 1.6rem;
  }
  .congrats-title {
    font-size: 1.8rem;
  }
  .subtitle {
    font-size: 0.9rem;
    margin-bottom: 20px;
  }
  .rules-box {
    padding: 16px 18px;
    margin-bottom: 24px;
  }
  .rule {
    padding: 8px 0;
  }
  .rule-text {
    font-size: 0.85rem;
  }
  .proceed-btn {
    width: 100%;
    justify-content: center;
    padding: 16px 32px;
    font-size: 1.05rem;
    -webkit-tap-highlight-color: transparent;
  }
  .proceed-btn:active {
    transform: scale(0.97);
  }
  .friendship-buttons {
    flex-direction: column;
    align-items: center;
    gap: 16px;
    min-height: 160px;
  }
  .yes-btn,
  .no-btn {
    width: 100%;
    justify-content: center;
    padding: 18px 36px;
    font-size: 1.1rem;
    -webkit-tap-highlight-color: transparent;
  }
  .yes-btn:active {
    transform: scale(0.97);
  }
  .friends-badge {
    padding: 16px 20px;
    gap: 12px;
    flex-wrap: wrap;
    justify-content: center;
  }
  .friend-name {
    font-size: 1.3rem;
  }
  .heart-icon {
    font-size: 1.6rem;
  }
  .congrats-text {
    font-size: 1rem;
  }
  .celebration-emojis {
    gap: 12px;
    font-size: 1.6rem;
  }
  .hint-text {
    font-size: 0.85rem;
  }
}
/* Touch device improvements */
@media (hover: none) and (pointer: coarse) {
  .proceed-btn:hover {
    transform: none;
    box-shadow: none;
  }
  .proceed-btn:active {
    transform: scale(0.96);
    box-shadow: 0 8px 20px rgba(139, 92, 246, 0.3);
  }
  .yes-btn:hover {
    transform: none;
    box-shadow: 0 6px 20px rgba(16, 185, 129, 0.25);
  }
  .yes-btn:active {
    transform: scale(0.96);
    box-shadow: 0 10px 30px rgba(16, 185, 129, 0.35);
  }
}
