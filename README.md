<!DOCTYPE html>
<html lang="de">
<head>
<meta charset="UTF-8">
<title>Press Start 🎂</title>
<style>
  body {
    margin: 0;
    font-family: "Courier New", monospace;
    background: black;
    color: #00ffcc;
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
  }
  .screen { display: none; }
  .active { display: block; }
  button {
    margin-top: 2rem;
    padding: 1rem 2rem;
    font-size: 1.2rem;
    background: #00ffcc;
    border: none;
    cursor: pointer;
  }
</style>
</head>
<body>

<div id="screen1" class="screen active">
  <h1>▶ PRESS START</h1>
  <button onclick="next(2)">START</button>
</div>

<div id="screen2" class="screen">
  <h1>🎉 HAPPY BIRTHDAY 🎉</h1>
  <p>Heute ist dein Tag.</p>
  <button onclick="next(3)">Weiter</button>
</div>

<div id="screen3" class="screen">
  <h1>🖌️ Geschenk freigeschaltet</h1>
  <p><strong>Keramik bemalen</strong><br>⏰ 14:00 Uhr</p>
  <button onclick="next(4)">Weiter</button>
</div>

<div id="screen4" class="screen">
  <h1>🎁 Gutschein</h1>
  <p style="font-size:2rem;"><strong>200 €</strong></p>
  <p>für einen Garmin Board Computer</p>
  <button onclick="next(5)">Finale</button>
</div>

<div id="screen5" class="screen">
  <h1>❤️ Gespeichert</h1>
  <p>Dieser Moment bleibt.</p>
  <p>Für immer.</p>
</div>

<script>
function next(n) {
  document.querySelectorAll('.screen').forEach(s => s.classList.remove('active'));
  document.getElementById('screen' + n).classList.add('active');
}
</script>

</body>
</html>
# Birthday-gift
