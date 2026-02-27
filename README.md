<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dark Mods | Oficial</title>
    <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@700&family=Roboto:wght@400;700&display=swap" rel="stylesheet">
    
    <style>
        :root {
            --pure-black: #000000;
            --dark-gray: #0d0d0d;
            --red-neon: #FF0000;
            --white: #FFFFFF;
            --gray-text: #b3b3b3;
        }

        * { box-sizing: border-box; margin: 0; padding: 0; }

        body {
            background-color: var(--pure-black);
            color: var(--white);
            font-family: 'Roboto', sans-serif;
            min-height: 100vh;
        }

        /* --- HEADER --- */
        header {
            width: 100%;
            background-color: var(--dark-gray);
            padding: 20px;
            text-align: center;
            border-bottom: 2px solid var(--red-neon);
            box-shadow: 0 0 20px rgba(255, 0, 0, 0.4);
            position: sticky;
            top: 0;
            z-index: 100;
        }

        .logo {
            font-family: 'Orbitron', sans-serif;
            color: var(--red-neon);
            font-size: 1.8rem;
            text-transform: uppercase;
            letter-spacing: 5px;
            text-shadow: 0 0 10px rgba(255, 0, 0, 0.6);
        }

        /* --- GRID CONTAINER --- */
        .container {
            max-width: 900px;
            margin: 30px auto;
            padding: 15px;
            display: grid;
            grid-template-columns: repeat(2, 1fr); /* 2 Colunas no Mobile */
            gap: 15px;
        }

        /* --- CARD --- */
        .card {
            background: var(--dark-gray);
            border-radius: 15px;
            overflow: hidden;
            border: 1px solid #222;
            transition: 0.3s;
            display: flex;
            flex-direction: column;
            text-align: center;
        }

        .card:hover {
            border-color: var(--red-neon);
            transform: translateY(-5px);
        }

        .app-banner {
            width: 100%;
            height: 140px;
            object-fit: cover;
            border-bottom: 1px solid #222;
        }

        .card-content {
            padding: 15px;
            flex-grow: 1;
            display: flex;
            flex-direction: column;
            justify-content: space-between;
        }

        .app-title {
            font-family: 'Orbitron', sans-serif;
            font-size: 1rem;
            margin-bottom: 5px;
        }

        .version {
            color: var(--red-neon);
            font-size: 0.8rem;
            font-weight: bold;
            margin-bottom: 10px;
        }

        .rating {
            color: #ffcc00;
            font-size: 0.8rem;
            margin-bottom: 15px;
        }

        .btn-download {
            background-color: var(--red-neon);
            color: white;
            text-decoration: none;
            padding: 12px;
            border-radius: 8px;
            font-weight: bold;
            font-size: 0.75rem;
            text-transform: uppercase;
            transition: 0.2s;
        }

        .btn-download:active {
            transform: scale(0.9);
        }

        @media (max-width: 400px) {
            .app-title { font-size: 0.9rem; }
            .container { gap: 10px; padding: 10px; }
        }
    </style>
</head>
<body>

    <header>
        <div class="logo">Dark Mods</div>
    </header>

    <main class="container">
        
        <div class="card">
            <img src="https://img.editalconcursosbrasil.com.br/wp-content/uploads/2022/01/minecraft.jpg" class="app-banner" alt="Minecraft">
            <div class="card-content">
                <div>
                    <h3 class="app-title">Minecraft</h3>
                    <p class="version">Versão: 1.20</p>
                    <div class="rating">★★★★★</div>
                </div>
                <a href="https://modsfire.com/ZSDB3npMj9Ap1k2" target="_blank" class="btn-download">Baixar</a>
            </div>
        </div>

        <div class="card">
            <img src="https://play-lh.googleusercontent.com/YvVz_9S0O5S0mD-WvV0GfFwX-L5j0V9qD0v9vV9vV9vV9vV9vV9vV9vV9vV9vV9vV9v" class="app-banner" alt="Elite Auto Brasil">
            <div class="card-content">
                <div>
                    <h3 class="app-title">Elite Auto Brasil</h3>
                    <p class="version">Versão: 0.58</p>
                    <div class="rating">★★★★★</div>
                </div>
                <a href="https://modsfire.com/hxkhNbAJX5Q22sW" target="_blank" class="btn-download">Baixar</a>
            </div>
        </div>

    </main>

</body>
</html>
