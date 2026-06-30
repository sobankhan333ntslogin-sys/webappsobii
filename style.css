// ===== Particle Background =====
function createParticles() {
  const container = document.getElementById('particles');
  const colors = ['rgba(139, 92, 246, 0.4)', 'rgba(244, 114, 182, 0.3)', 'rgba(99, 102, 241, 0.3)', 'rgba(167, 139, 250, 0.35)'];
  
  for (let i = 0; i < 30; i++) {
    const particle = document.createElement('div');
    particle.classList.add('particle');
    const size = Math.random() * 5 + 2;
    const color = colors[Math.floor(Math.random() * colors.length)];
    
    particle.style.width = size + 'px';
    particle.style.height = size + 'px';
    particle.style.background = color;
    particle.style.left = Math.random() * 100 + '%';
    particle.style.animationDuration = (Math.random() * 15 + 10) + 's';
    particle.style.animationDelay = (Math.random() * 10) + 's';
    
    container.appendChild(particle);
  }
}
createParticles();
// ===== Step Transitions =====
function goToStep2() {
  const step1 = document.getElementById('step1');
  const step2 = document.getElementById('step2');
  
  step1.classList.remove('active');
  step1.classList.add('exit');
  
  setTimeout(() => {
    step2.classList.add('active');
    initNoButton();
  }, 400);
}
function goToStep3() {
  const step2 = document.getElementById('step2');
  const step3 = document.getElementById('step3');
  
  step2.classList.remove('active');
  step2.classList.add('exit');
  
  setTimeout(() => {
    step3.classList.add('active');
    launchConfetti();
  }, 400);
}
// ===== Step 2: The Sneaky No Button =====
const noMessages = [
  "Haha, nice try! 😄",
  "You can't click No! 😏",
  "Nope, not happening! 🙅‍♀️",
  "The No button is scared! 😱",
  "Try again... just kidding! 😂",
  "No is not an option! 💁‍♀️",
  "That button is too fast! 🏃‍♂️",
  "Just say Yes already! 😊"
];
let noMoveCount = 0;
function initNoButton() {
  const noBtn = document.getElementById('noBtn');
  const card = document.getElementById('step2');
  
  // Position the No button initially
  const friendshipBtns = document.querySelector('.friendship-buttons');
  friendshipBtns.style.position = 'relative';
  friendshipBtns.style.minHeight = '80px';
  
  noBtn.style.position = 'relative';
  noBtn.style.left = '0';
  noBtn.style.top = '0';
  
  noBtn.addEventListener('mouseenter', handleNoHover);
  noBtn.addEventListener('touchstart', handleNoHover);
  noBtn.addEventListener('click', handleNoHover);
}
function handleNoHover(e) {
  e.preventDefault();
  const noBtn = document.getElementById('noBtn');
  const card = document.getElementById('step2');
  const cardRect = card.getBoundingClientRect();
  
  // Calculate safe bounds within the card
  const btnWidth = noBtn.offsetWidth;
  const btnHeight = noBtn.offsetHeight;
  const padding = 20;
  
  // Get a random position within the card
  const maxX = cardRect.width - btnWidth - padding * 2;
  const maxY = cardRect.height - btnHeight - padding * 2;
  
  const randomX = Math.random() * maxX - maxX / 2;
  const randomY = Math.random() * maxY - maxY / 2;
  
  noBtn.style.position = 'absolute';
  noBtn.style.left = `calc(50% + ${randomX}px)`;
  noBtn.style.top = `calc(50% + ${randomY}px)`;
  noBtn.style.transform = 'translate(-50%, -50%)';
  noBtn.style.zIndex = '100';
  noBtn.style.transition = 'left 0.15s ease-out, top 0.15s ease-out';
  
  // Show funny message
  noMoveCount++;
  const hintText = document.getElementById('hintText');
  hintText.textContent = noMessages[(noMoveCount - 1) % noMessages.length];
  hintText.classList.add('show');
}
// ===== Yes Button =====
function sayYes() {
  goToStep3();
}
// ===== Confetti =====
function launchConfetti() {
  const container = document.getElementById('confetti');
  const emojis = ['🎉', '🎊', '✨', '⭐', '🌟', '🙌', '🥳', '🎈', '👏', '🤝'];
  
  for (let i = 0; i < 40; i++) {
    setTimeout(() => {
      const piece = document.createElement('div');
      piece.classList.add('confetti-piece');
      piece.textContent = emojis[Math.floor(Math.random() * emojis.length)];
      piece.style.left = Math.random() * 100 + '%';
      piece.style.fontSize = (Math.random() * 16 + 12) + 'px';
      piece.style.animationDuration = (Math.random() * 2 + 1.5) + 's';
      piece.style.animationDelay = '0s';
      container.appendChild(piece);
      
      // Remove after animation
      setTimeout(() => piece.remove(), 3500);
    }, i * 80);
  }
  
  // Second wave
  setTimeout(() => {
    for (let i = 0; i < 20; i++) {
      setTimeout(() => {
        const piece = document.createElement('div');
        piece.classList.add('confetti-piece');
        piece.textContent = emojis[Math.floor(Math.random() * emojis.length)];
        piece.style.left = Math.random() * 100 + '%';
        piece.style.fontSize = (Math.random() * 16 + 12) + 'px';
        piece.style.animationDuration = (Math.random() * 2 + 1.5) + 's';
        container.appendChild(piece);
        
        setTimeout(() => piece.remove(), 3500);
      }, i * 100);
    }
  }, 1500);
}
// ===== Pulse Animation for Proceed Button =====
const styleSheet = document.createElement('style');
styleSheet.textContent = `
  @keyframes pulseBtn {
    0% { transform: scale(1); }
    50% { transform: scale(1.05); }
    100% { transform: scale(1); }
  }
`;
document.head.appendChild(styleSheet);
