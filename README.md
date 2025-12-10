<!DOCTYPE html>
<html lang="de">
<head>
<meta charset="UTF-8">
<title>OVERTHINK.EXE</title>

<style>
/* ===== BASIC LAYOUT ===== */
body {
  margin: 0;
  background: black;
  color: #00ffcc;
  font-family: monospace;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
}

/* ===== TERMINAL BLOCK ===== */
.terminal {
  text-align: center;
  font-size: 1.2rem;
  letter-spacing: 0.08em;
}

/* ===== TYPEWRITER EFFECT ===== */
.line {
  overflow: hidden;
  white-space: nowrap;
  width: 0;
  border-right: 0.15em solid #00ffcc;
  margin: 0 auto;
}

/* Line 1 */
.line.one {
  animation:
    typing-one 3s steps(15, end) forwards,
    blink 0.7s step-end 5;
}

/* Line 2 */
.line.two {
  animation:
    typing-two 2.8s steps(30, end) forwards,
    blink 0.7s step-end 8;
  animation-delay: 2s;
}

/* Line 3 */
.line.three {
  animation:
    typing-three 2s steps(15, end) forwards,
    blink 0.7s step-end 6;
  animation-delay: 5.2s;
}

/* ===== KEYFRAMES ===== */
@keyframes typing-one {
  to { width: 17ch; } /* INITIALIZING */
}

@keyframes typing-two {
  to { width: 30ch; } /* CHECKING SYSTEM INTEGRITY */
}

@keyframes typing-three {
  to { width: 18ch; } /* ACCESS GRANTED */
}

@keyframes blink {
  50% { border-color: transparent; }
}

/* ===== FLICKER FOR CYBER FEEL ===== */
.terminal {
  animation: flicker 1.5s infinite;
}

@keyframes flicker {
  0% { opacity: 1; }
  45% { opacity: 0.75; }
  50% { opacity: 0.9; }
  60% { opacity: 0.6; }
  100% { opacity: 1; }
}

/* ===== SMALL FOOTNOTE ===== */
.footer {
  font-size: 0.7rem;
  margin-top: 2rem;
  opacity: 0.6;
}
</style>
</head>

<body>

<div class="terminal">
  <div class="line one">INITIALIZING</div>
  <div class="line two">CHECKING SYSTEM INTEGRITY</div>
  <div class="line three">ACCESS DENIED</div>

  <div class="footer">
    You may try again.
  </div>
</div>

</body>
</html>


