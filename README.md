[index.html](https://github.com/user-attachments/files/23292712/index.html)
<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Estrategias de Aprendizaje</title>
<style>
  body {
    font-family: 'Segoe UI', sans-serif;
    text-align: center;
    background: linear-gradient(to right, #e3f2fd, #fce4ec);
    margin: 0;
    padding: 0;
  }

  h1 {
    background-color: #4a148c;
    color: white;
    padding: 15px;
    margin: 0;
    box-shadow: 0 2px 5px rgba(0,0,0,0.3);
  }

  .menu, .submenu {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    margin-top: 40px;
    gap: 20px;
  }

  button {
    background-color: #6a1b9a;
    color: white;
    border: none;
    padding: 15px;
    border-radius: 15px;
    font-size: 16px;
    cursor: pointer;
    transition: 0.3s;
    width: 260px;
    height: auto;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    box-shadow: 0 4px 8px rgba(0,0,0,0.2);
  }

  button:hover {
    background-color: #8e24aa;
    transform: scale(1.05);
  }

  button img {
    width: 60px;
    height: 60px;
    margin-bottom: 8px;
  }

  .submenu {
    display: none;
  }

  .volver {
    background-color: #283593;
    color: white;
    border: none;
    padding: 10px 20px;
    margin-top: 20px;
    border-radius: 10px;
    cursor: pointer;
  }

  .volver:hover {
    background-color: #1a237e;
  }
</style>
</head>
<body>

<h1>💡 Estrategias de Aprendizaje 💡</h1>

<!-- Menú principal -->
<div class="menu" id="menuPrincipal">
  <button onclick="mostrarSubmenu('motivacion')">
    <img src="https://cdn-icons-png.flaticon.com/512/616/616408.png" alt="Motivación">
    Estrategia de aprendizaje motivado
  </button>
  <button onclick="mostrarSubmenu('organizacion')">
    <img src="https://cdn-icons-png.flaticon.com/512/3062/3062634.png" alt="Organización">
    Estrategia de organización
  </button>
  <button onclick="mostrarSubmenu('memorizacion')">
    <img src="https://cdn-icons-png.flaticon.com/512/2921/2921222.png" alt="Memorización">
    Estrategia de memorización
  </button>
  <button onclick="mostrarSubmenu('colaboracion')">
    <img src="https://cdn-icons-png.flaticon.com/512/681/681392.png" alt="Colaboración">
    Estrategia de aprendizaje colaborativo
  </button>
</div>

<!-- Submenús -->
<div id="motivacion" class="submenu">
  <button><img src="https://cdn-icons-png.flaticon.com/512/3209/3209265.png">Establece metas claras y alcanzables para mantenerte enfocado.</button>
  <button><img src="https://cdn-icons-png.flaticon.com/512/992/992700.png">Celebra cada logro, por pequeño que sea, para mantener alta tu energía.</button>
  <button><img src="https://cdn-icons-png.flaticon.com/512/4144/4144517.png">Relaciona lo que aprendes con tus intereses o metas personales.</button>
  <button><img src="https://cdn-icons-png.flaticon.com/512/1048/1048944.png">Crea un ambiente positivo y libre de distracciones.</button>
  <button class="volver" onclick="volverMenu()">⬅ Volver</button>
</div>

<div id="organizacion" class="submenu">
  <button><img src="https://cdn-icons-png.flaticon.com/512/1055/1055644.png">Utiliza una agenda o app para planificar tus tareas diarias.</button>
  <button><img src="https://cdn-icons-png.flaticon.com/512/478/478543.png">Organiza tus materiales y recursos antes de estudiar.</button>
  <button><img src="https://cdn-icons-png.flaticon.com/512/4727/4727493.png">Divide tus objetivos grandes en pasos pequeños.</button>
  <button><img src="https://cdn-icons-png.flaticon.com/512/3267/3267473.png">Cumple con horarios fijos para crear hábitos estables.</button>
  <button class="volver" onclick="volverMenu()">⬅ Volver</button>
</div>

<div id="memorizacion" class="submenu">
  <button><img src="https://cdn-icons-png.flaticon.com/512/3715/3715183.png">Repite en voz alta o escribe lo aprendido para reforzarlo.</button>
  <button><img src="https://cdn-icons-png.flaticon.com/512/2645/2645897.png">Usa mapas mentales o tarjetas para repasar conceptos.</button>
  <button><img src="https://cdn-icons-png.flaticon.com/512/3787/3787392.png">Asocia ideas con imágenes, sonidos o experiencias.</button>
  <button><img src="https://cdn-icons-png.flaticon.com/512/4144/4144429.png">Estudia en bloques de 25 minutos con descansos breves.</button>
  <button class="volver" onclick="volverMenu()">⬅ Volver</button>
</div>

<div id="colaboracion" class="submenu">
  <button><img src="https://cdn-icons-png.flaticon.com/512/1256/1256650.png">Trabaja en grupo para compartir puntos de vista.</button>
  <button><img src="https://cdn-icons-png.flaticon.com/512/4712/4712062.png">Escucha y respeta las opiniones de tus compañeros.</button>
  <button><img src="https://cdn-icons-png.flaticon.com/512/3652/3652269.png">Aprende explicando los temas a otros.</button>
  <button><img src="https://cdn-icons-png.flaticon.com/512/3050/3050525.png">Utiliza plataformas digitales para colaborar y debatir.</button>
  <button class="volver" onclick="volverMenu()">⬅ Volver</button>
</div>

<script>
  function mostrarSubmenu(id) {
    document.getElementById('menuPrincipal').style.display = 'none';
    document.querySelectorAll('.submenu').forEach(m => m.style.display = 'none');
    document.getElementById(id).style.display = 'flex';
  }

  function volverMenu() {
    document.querySelectorAll('.submenu').forEach(m => m.style.display = 'none');
    document.getElementById('menuPrincipal').style.display = 'flex';
  }
</script>

</body>
</html>
