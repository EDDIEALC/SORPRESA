
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Invitación San Valentín</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      height: 100vh;
      background-image: url('tu-imagen-de-fondo.jpg'); /* Cambia esta URL con la de tu imagen de fondo */
      background-size: cover;
      display: flex;
      justify-content: center;
      align-items: center;
      flex-direction: column;
    }
    .container {
      text-align: center;
      color: rgb(255, 255, 255);
    }
    h1 {
      font-size: 3em;
      margin-bottom: 20px;
    }
    .btn {
      border: none;
      padding: 15px;
      margin: 10px;
      background-color: transparent;
      font-size: 1.5em;
      cursor: pointer;
    }
    .heart-btn {
      font-size: 2em;
      background-color: transparent;
      color: #fcfcfc;
    }
    .heart-btn:hover {
      color: #ffffff;
    }
    .gif-container {
      margin-top: 20px;
    }
    .image-container {
      display: flex;
      justify-content: center;
      margin-top: 20px;
    }
    .image-container img {
      margin: 0 20px;
      width: 200px;
    }
  </style>
</head>
<body>
  <!-- Primer plano -->
  <div class="container" id="primer-plano">
    <h1>QUIERES SER MI SAN VALENTIN?</h1>
    <div class="gif-container">
      <img src="osito.gif" alt="Osito" width="200px"> <!-- Cambia esto con la URL de tu GIF de osito -->
    </div>
    <div>
      <button class="btn heart-btn" id="btn-si">SI</button>
      <button class="btn heart-btn" id="btn-no">NO</button>
    </div>
  </div>

  <!-- Segundo plano, inicialmente oculto -->
  <div class="container" id="segundo-plano" style="display: none;">
    <h1>ESTÁS INVITADA ESTE 15 DE FEBRERO A PASAR UNA NOCHE ROMÁNTICA</h1>
    <div class="gif-container">
      <img src="oso-feliz.gif" alt="Oso feliz" width="200px"> <!-- Cambia esto con la URL de tu GIF de oso feliz -->
    </div>
    <div class="image-container">
      <img src="foto1.jpeg" alt="Foto 1"> <!-- Cambia esto con la URL de tu primera foto -->
      <img src="foto2.jpeg" alt="Foto 2"> <!-- Cambia esto con la URL de tu segunda foto -->
    </div>
  </div>

  <!-- Opción NO, inicialmente oculta -->
  <div class="container" id="gif-no" style="display: none;">
    <div class="gif-container">
      <img src="oso-triste.gif" alt="Oso triste" width="200px"> <!-- Cambia esto con la URL de tu GIF de oso triste -->
    </div>
  </div>

  <script>
    document.getElementById('btn-si').addEventListener('click', function() {
      // Ocultar el primer plano
      document.getElementById('primer-plano').style.display = 'none';
      // Mostrar el segundo plano
      document.getElementById('segundo-plano').style.display = 'block';
    });

    document.getElementById('btn-no').addEventListener('click', function() {
      // Ocultar el primer plano
      document.getElementById('primer-plano').style.display = 'none';
      // Mostrar el gif de "NO"
      document.getElementById('gif-no').style.display = 'block';
    });
  </script>
</body>
</html>
