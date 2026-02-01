<!DOCTYPE html><html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Raj Kumar Verma</title>
  <style>
    * { box-sizing: border-box; }
    html, body {
      margin: 0;
      padding: 0;
      height: 100%;
      font-family: 'Segoe UI', system-ui, -apple-system, sans-serif;
      color: #fff;
      overflow: hidden;
    }/* Animated background */
.bg {
  position: fixed;
  inset: 0;
  background: linear-gradient(120deg, #0f0f0f, #1a1a2e, #0f3460);
  background-size: 400% 400%;
  animation: gradientMove 12s ease infinite;
  z-index: -2;
}

@keyframes gradientMove {
  0% { background-position: 0% 50%; }
  50% { background-position: 100% 50%; }
  100% { background-position: 0% 50%; }
}

/* Samurai silhouette */
.samurai {
  position: fixed;
  bottom: -40px;
  right: 5%;
  width: 420px;
  max-width: 90vw;
  opacity: 0.25;
  animation: float 6s ease-in-out infinite;
  z-index: -1;
}

@keyframes float {
  0%, 100% { transform: translateY(0); }
  50% { transform: translateY(-20px); }
}

.card {
  min-height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 24px;
}

.content {
  backdrop-filter: blur(10px);
  background: rgba(0,0,0,0.45);
  border-radius: 20px;
  padding: 32px 40px;
  max-width: 420px;
  width: 100%;
  box-shadow: 0 20px 50px rgba(0,0,0,0.6);
}

h1 {
  margin-top: 0;
  font-size: 2rem;
  letter-spacing: 1px;
}

.info {
  margin-top: 20px;
  line-height: 1.8;
  font-size: 1.05rem;
}

.label { opacity: 0.75; }
.value { font-weight: 600; }

.social {
  margin-top: 24px;
  display: flex;
  gap: 14px;
  flex-wrap: wrap;
}

.social a {
  text-decoration: none;
  color: #fff;
  padding: 10px 16px;
  border-radius: 999px;
  background: linear-gradient(135deg, #e94560, #533483);
  font-weight: 600;
  transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.social a:hover {
  transform: translateY(-2px) scale(1.03);
  box-shadow: 0 10px 25px rgba(0,0,0,0.5);
}

  </style>
</head>
<body>
  <div class="bg"></div>  <!-- Samurai SVG -->  <svg class="samurai" viewBox="0 0 512 512" fill="white" xmlns="http://www.w3.org/2000/svg">
    <path d="M256 32c-40 0-72 32-72 72 0 18 6 34 16 46l-40 66-78 30 14 38 72-18-22 40-84 44 18 36 78-32 6 68h192l6-68 78 32 18-36-84-44-22-40 72 18 14-38-78-30-40-66c10-12 16-28 16-46 0-40-32-72-72-72z"/>
  </svg>  <div class="card">
    <div class="content">
      <h1>Raj Kumar Verma</h1>
      <div class="info">
        <div><span class="label">Date of Birth:</span> <span class="value">15 February</span></div>
        <div><span class="label">Age:</span> <span class="value">18</span></div>
        <div><span class="label">Instagram:</span> <span class="value">@rajxverma15</span></div>
        <div><span class="label">Snapchat:</span> <span class="value">@rajxverma15</span></div>
      </div><div class="social">
    <a href="https://instagram.com/rajxverma15" target="_blank">Instagram</a>
    <a href="#" onclick="alert('Snapchat usernames open in the app')">Snapchat</a>
  </div>
</div>

  </div>
</body>
</html>
