# Proyecto-Erick-
Proyecto Erick stranger things
<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<title>STRANGER THINGS</title>
<link href="https://fonts.googleapis.com/css2?family=Oswald:wght@700&family=VT323&display=swap" rel="stylesheet">
<style>
  *{margin:0;padding:0;box-sizing:border-box}
  body{background:#080005;color:#c8a8a8;font-family:'VT323',monospace;min-height:100vh;cursor:crosshair}
  body::before{content:'';position:fixed;inset:0;background:repeating-linear-gradient(0deg,transparent,transparent 3px,rgba(0,0,0,.12) 3px,rgba(0,0,0,.12) 4px);pointer-events:none;z-index:999}
  h1{font-family:'Oswald',sans-serif;font-size:clamp(3.5rem,11vw,8rem);letter-spacing:.18em;color:#cc0000;text-shadow:0 0 20px #ff0000,0 0 80px #aa000066;animation:flicker 5s infinite;text-align:center;padding:50px 20px 6px}
  .sub{text-align:center;letter-spacing:.6em;color:#7a4a4a;font-size:1.3rem;margin-bottom:30px}
  nav{display:flex;justify-content:center;border-top:1px solid #2a0808;border-bottom:1px solid #2a0808}
  nav a{color:#aa4444;text-decoration:none;font-size:1.4rem;letter-spacing:.2em;padding:14px 28px;border-right:1px solid #2a0808;transition:all .25s}
  nav a:first-child{border-left:1px solid #2a0808}
  nav a:hover{background:#1a0008;color:#ff2200;text-shadow:0 0 12px #ff2200}
  nav a.active{background:#120005;color:#ff3333;border-bottom:2px solid #cc0000}
  .panels{display:none;padding:40px 20px;max-width:960px;margin:0 auto;animation:fadein .4s ease}
  .panels.show{display:block}
  .panels h2{font-family:'Oswald',sans-serif;color:#cc2222;font-size:2rem;letter-spacing:.12em;border-bottom:1px solid #2a0808;padding-bottom:10px;margin-bottom:20px}
  .row{display:grid;grid-template-columns:repeat(auto-fit,minmax(220px,1fr));gap:1px;background:#1a0808}
  .item{background:#0d0005;padding:22px 18px}
  .item h3{color:#cc3333;font-size:1.3rem;letter-spacing:.08em;margin-bottom:8px}
  .item p{color:#7a5555;font-size:1.15rem;line-height:1.45}
  .tag{color:#552222;font-size:1rem;margin-top:10px;letter-spacing:.1em}
  .lights{display:flex;justify-content:center;gap:10px;padding:18px;flex-wrap:wrap}
  .b{width:18px;height:18px;border-radius:50%;animation:blink var(--d) var(--delay) infinite alternate}
  footer{text-align:center;padding:40px 20px;color:#3a1a1a;font-size:1.1rem;letter-spacing:.4em;border-top:1px solid #1a0808;margin-top:40px}
  @keyframes flicker{0%,100%{opacity:1}91%{opacity:1}92%{opacity:.3}93%{opacity:1}97%{opacity:.7}98%{opacity:1}}
  @keyframes blink{from{opacity:.08;box-shadow:none}to{opacity:1;box-shadow:0 0 10px var(--c),0 0 22px var(--c)}}
  @keyframes fadein{from{opacity:0;transform:translateY(8px)}to{opacity:1;transform:none}}
</style>
</head>
<body>
<h1>STRANGER THINGS</h1>
<p class="sub">HAWKINS, INDIANA · 1983</p>
<div class="lights" id="lights"></div>
<nav>
  <a href="#" class="active" onclick="return show('hawkins',this)">HAWKINS</a>
  <a href="#" onclick="return show('personajes',this)">PERSONAJES</a>
  <a href="#" onclick="return show('reves',this)">EL REVÉS</a>
  <a href="#" onclick="return show('criaturas',this)">CRIATURAS</a>
</nav>
<div id="hawkins" class="panels show"><h2>HAWKINS, INDIANA</h2><div class="row"><div class="item"><h3>LABORATORIO</h3><p>Proyecto MKUltra encubierto. Sus experimentos abrieron la puerta al Mundo del Revés.</p><p class="tag">// CLASIFICADO</p></div><div class="item"><h3>INSTITUTO HAWKINS</h3><p>Donde todo comenzó. Pasadizos ocultos conectan con el lado oscuro de la realidad.</p><p class="tag">// SECTOR 7-G</p></div><div class="item"><h3>BYERS RESIDENCE</h3><p>Joyce usó luces navideñas para comunicarse con Will atrapado en otra dimensión.</p><p class="tag">// A·B·C·D</p></div></div></div>
<div id="personajes" class="panels"><h2>PERSONAJES</h2><div class="row"><div class="item"><h3>ONCE — 011</h3><p>Poderes telekinéticos. Escapó del laboratorio y encontró una familia inesperada en Hawkins.</p><p class="tag">// SUJETO 011</p></div><div class="item"><h3>WILL BYERS</h3><p>Desapareció en 1983. Sobrevivió el Mundo del Revés pero sus cicatrices son invisibles.</p><p class="tag">// DESAPARECIDO</p></div><div class="item"><h3>JIM HOPPER</h3><p>Sheriff de Hawkins. Protector feroz de Eleven y guardián de los secretos de la ciudad.</p><p class="tag">// JEFE DE POLICÍA</p></div></div></div>
<div id="reves" class="panels"><h2>EL MUNDO DEL REVÉS</h2><div class="row"><div class="item"><h3>LA DIMENSIÓN</h3><p>Reflejo oscuro del mundo real. Sin luz, sin vida. Solo ceniza, venas y oscuridad eterna.</p><p class="tag">// ACCESO RESTRINGIDO</p></div><div class="item"><h3>EL PORTAL</h3><p>Abierto por Eleven durante un experimento. Ubicado en el sótano del Laboratorio Hawkins.</p><p class="tag">// BRECHA ACTIVA</p></div><div class="item"><h3>LA COLMENA</h3><p>Red neuronal que conecta a todos los seres del Revés bajo la voluntad del Mind Flayer.</p><p class="tag">// RED NEURAL</p></div></div></div>
<div id="criaturas" class="panels"><h2>CRIATURAS</h2><div class="row"><div class="item"><h3>DEMOGORGON</h3><p>Sin ojos. Detecta sangre. Aterrorizó Hawkins en 1983. Primera amenaza del Mundo del Revés.</p><p class="tag">// PELIGRO EXTREMO</p></div><div class="item"><h3>MIND FLAYER</h3><p>La Sombra. Inteligencia superior que controla su ejército y amenaza con invadir el mundo real.</p><p class="tag">// AMENAZA NIVEL S</p></div><div class="item"><h3>DEMODOGS</h3><p>Fase intermedia del Demogorgon. Operan en manada bajo órdenes directas del Mind Flayer.</p><p class="tag">// PACK ACTIVO</p></div></div></div>
<footer>EL MUNDO DEL REVÉS TE OBSERVA · ████████</footer>
<script>
  const cols=['#ff0000','#ff6600','#ffff00','#00ff00','#00aaff','#aa00ff','#ff00aa'];
  const L=document.getElementById('lights');
  for(let i=0;i<14;i++){const b=document.createElement('div');b.className='b';b.style.cssText=`--c:${cols[i%7]};background:${cols[i%7]};--d:${(.5+Math.random()*.9).toFixed(2)}s;--delay:${(Math.random()*1.4).toFixed(2)}s`;L.appendChild(b)}
  function show(id,el){document.querySelectorAll('.panels').forEach(p=>p.classList.remove('show'));document.getElementById(id).classList.add('show');document.querySelectorAll('nav a').forEach(a=>a.classList.remove('active'));el.classList.add('active');return false}
</script>
</body>
</html>
