[index.html](https://github.com/user-attachments/files/23027660/index.html)
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Centro de Educación Básica Alfonso Molina Rugama</title>
  <style>
    /* Estilos generales */
    body {
      margin: 0;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background-color: #f4f8ff;
      color: #002855;
    }

    header {
      background-color: #003b8e;
      color: white;
      padding: 20px 0;
      text-align: center;
      box-shadow: 0 2px 5px rgba(0,0,0,0.2);
    }

    header h1 {
      margin: 0;
      font-size: 1.8rem;
    }

    nav {
      background-color: #0056d6;
      text-align: center;
      padding: 10px 0;
    }

    nav a {
      color: white;
      text-decoration: none;
      margin: 0 15px;
      font-weight: bold;
      transition: color 0.3s;
    }

    nav a:hover {
      color: #ffd700;
    }

    section {
      padding: 40px 20px;
      max-width: 1000px;
      margin: auto;
      background-color: white;
      margin-top: 20px;
      border-radius: 8px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.1);
    }

    h2 {
      color: #003b8e;
      border-bottom: 3px solid #0056d6;
      display: inline-block;
      margin-bottom: 15px;
    }

    .docentes, .estudiantes {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
      gap: 15px;
    }

    .card {
      background-color: #f0f6ff;
      border: 1px solid #cbd7f3;
      border-radius: 10px;
      padding: 15px;
      text-align: center;
    }

    footer {
      background-color: #003b8e;
      color: white

