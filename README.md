<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CEB Alfonso Molina Rugama</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <style>
        /* CSS Integrado para facilidad */
        :root {
            --azul-primario: #1a4a7a;
            --azul-oscuro: #0d2c4a;
            --dorado: #d4af37;
            --blanco: #ffffff;
            --gris-fondo: #f4f7f6;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            margin: 0;
            background-color: var(--gris-fondo);
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
        }

        /* --- Estilos Login --- */
        #login-section {
            background: var(--blanco);
            padding: 2rem;
            border-radius: 15px;
            box-shadow: 0 10px 25px rgba(0,0,0,0.1);
            text-align: center;
            width: 100%;
            max-width: 350px;
        }

        .logo-placeholder {
            font-size: 50px;
            color: var(--azul-primario);
            margin-bottom: 10px;
        }

        input {
            width: 100%;
            padding: 12px;
            margin: 10px 0;
            border: 1px solid #ddd;
            border-radius: 5px;
            box-sizing: border-box;
        }

        button {
            width: 100%;
            padding: 12px;
            background-color: var(--azul-primario);
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-weight: bold;
            transition: 0.3s;
        }

        button:hover { background-color: var(--azul-oscuro); }

        /* --- Estilos Panel (Oculto al inicio) --- */
        #main-panel {
            display: none; /* Se activa con JS */
            width: 90%;
            max-width: 1000px;
            padding: 20px;
        }

        .header-panel {
            text-align: center;
            margin-bottom: 30px;
        }

        .grid-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
        }

        .card {
            background: var(--blanco);
            padding: 30px;
            border-radius: 12px;
            text-align: center;
            transition: transform 0.3s, box-shadow 0.3s;
            cursor: pointer;
            border-bottom: 4px solid var(--azul-primario);
        }

        .card:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 20px rgba(0,0,0,0.15);
        }

        .card i {
            font-size: 40px;
            color: var(--azul-primario);
            margin-bottom: 15px;
        }

        .card h3 {
            margin: 0;
            font-size: 1.1rem;
            color: #333;
        }
    </style>
</head>
<body>

    <section id="login-section">
        <div class="logo-placeholder"><i class="fas fa-university"></i></div>
        <h2>CEB Alfonso Molina Rugama</h2>
        <p>Ingrese sus credenciales</p>
        <input type="text" placeholder="Usuario">
        <input type="password" placeholder="Contraseña">
        <button onclick="mostrarPanel()">Iniciar Sesión</button>
    </section>

    <section id="main-panel">
        <div class="header-panel">
            <h1>Bienvenido al Portal Escolar</h1>
            <p>Seleccione una categoría para continuar</p>
        </div>

        <div class="grid-container">
            <div class="card">
                <i class="fas fa-book-open"></i>
                <h3>Historia</h3>
            </div>
            <div class="card">
                <i class="fas fa-graduation-cap"></i>
                <h3>Grados (1° - 9°)</h3>
            </div>
            <div class="card">
                <i class="fas fa-bullseye"></i>
                <h3>Misión y Visión</h3>
            </div>
            <div class="card">
                <i class="fas fa-heart"></i>
                <h3>Valores</h3>
            </div>
            <div class="card">
                <i class="fas fa-file-invoice-dollar"></i>
                <h3>Transparencia</h3>
            </div>
            <div class="card">
                <i class="fas fa-users"></i>
                <h3>Eventos Sociales</h3>
            </div>
        </div>
        <div style="text-align: center; margin-top: 40px;">
            <button onclick="location.reload()" style="width: auto; padding: 10px 25px;">Cerrar Sesión</button>
        </div>
    </section>

    <script>
        function mostrarPanel() {
            document.getElementById('login-section').style.display = 'none';
            document.getElementById('main-panel').style.display = 'block';
        }
    </script>
</body>
</html>
