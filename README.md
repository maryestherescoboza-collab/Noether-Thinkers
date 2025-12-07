<!doctype html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Beneficios Thinkers</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        /* Paleta de Colores de la Imagen (Vibrante) */
        :root {
            /* Fondo General (Oscuro, como la imagen) */
            --bg-deep: #0A0F17; 
            --text-light: #E0E7FF;
            
            /* Glassmorphism (Encabezado) */
            --glass-bg: rgba(255, 255, 255, 0.05);
            --glass-border: rgba(255, 255, 255, 0.1);

            /* Degradados Vibrantes de las Tarjetas (Basados en la imagen) */
            --card-grad-1: linear-gradient(145deg, #A564BB, #F5B170); /* Púrpura/Melocotón */
            --card-grad-2: linear-gradient(145deg, #76D7C4, #FAD7E2); /* Turquesa/Rosa Claro */
            --card-grad-3: linear-gradient(145deg, #EA9889, #F9E79F); /* Coral/Crema */
            --card-grad-4: linear-gradient(145deg, #6FA8DC, #D5DBB1); /* Azul/Verde Lima */

            /* Degradado del Botón CTA (Verde a Azul, muy suave) */
            --cta-grad: linear-gradient(90deg, #6EE7B7, #74C0E3);
        }
        
        body {
            background-color: var(--bg-deep);
            color: var(--text-light);
            font-family: 'Inter', sans-serif;
            min-height: 100vh;
        }

        /* 1. Glassmorphism para el Encabezado */
        .header-content {
            background-color: var(--glass-bg);
            backdrop-filter: blur(15px);
            -webkit-backdrop-filter: blur(15px);
            border: 1px solid var(--glass-border);
            box-shadow: 0 8px 32px 0 rgba(0, 0, 0, 0.37);
        }

        /* 2. Botón CTA con Degradado y Movimiento */
        .cta-btn {
            background-image: var(--cta-grad);
            color: var(--bg-deep); /* Texto oscuro para contraste */
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .cta-btn:hover {
            transform: scale(1.03); /* Más movimiento */
            box-shadow: 0 5px 20px rgba(110, 231, 183, 0.5);
        }

        /* 3. Estilos de las Tarjetas y Aplicación de Degradados */
        .benefit-card {
            border-radius: 18px; /* Bordes más redondeados */
            padding: 30px;
            color: #1F2937; /* Texto oscuro para alto contraste en fondos claros */
            box-shadow: 0 6px 15px rgba(0, 0, 0, 0.3);
            transition: transform 0.4s cubic-bezier(0.25, 0.8, 0.25, 1);
            position: relative;
            overflow: hidden;
        }
        
        .card-1 { background: var(--card-grad-1); }
        .card-2 { background: var(--card-grad-2); }
        .card-3 { background: var(--card-grad-3); }
        .card-4 { background: var(--card-grad-4); }

        .benefit-card:hover {
            transform: translateY(-8px) scale(1.02); /* Movimiento y zoom fluidos */
        }
        
        /* Aseguramos que el texto dentro de la tarjeta sea legible */
        .benefit-card h3 {
            color: #1F2937;
        }
        .benefit-card p {
            color: #374151;
        }

        /* 4. Estilo de los iconos (usaremos círculos de acento para representar la fluidez) */
        .icon-placeholder {
            width: 30px;
            height: 30px;
            border-radius: 50%;
            display: inline-block;
            margin-bottom: 10px;
        }
        .icon-1 { background: #6F42C1; } /* Púrpura */
        .icon-2 { background: #059669; } /* Verde */
        .icon-3 { background: #FACC15; } /* Amarillo */
        .icon-4 { background: #3B82F6; } /* Azul */

    </style>
</head>
<body class="p-4 sm:p-8">

    <header class="header-content max-w-4xl mx-auto rounded-3xl p-8 text-center mt-6">
        <h1 class="text-4xl sm:text-5xl font-extrabold mb-4 text-white">
            Beneficios exclusivos Thinkers
        </h1>
        
        <p class="text-lg text-gray-300 max-w-2xl mx-auto mb-8">
            Los productos Thinkers son una suite de herramientas y recursos digitales especializados en el ámbito de la gestión y la evaluación. Su formato principal se centra en plantillas de Excel y sistemas de gestión diseñados para todos los que buscan ordenar un aspecto de su vida.
        </p>
        
        <a href="#unirse" class="cta-btn inline-block px-8 py-3 text-xl font-bold rounded-full uppercase tracking-wider shadow-lg">
            ¡Quiero Ser Miembro Ahora! →
        </a>
    </header>

    <main class="max-w-5xl mx-auto mt-12 mb-16">
        
        <div class="grid grid-cols-1 md:grid-cols-2 gap-10">

            <div class="benefit-card card-1 p-6">
                <div class="icon-placeholder icon-1"></div>
                <h3 class="text-2xl font-extrabold mt-2">Acceso total a Proyectos</h3>
                <p class="mt-2 text-lg">Obtenga acceso inmediato a todos los proyectos actuales y futuros.</p>
            </div>

            <div class="benefit-card card-2 p-6">
                <div class="icon-placeholder icon-2"></div>
                <h3 class="text-2xl font-extrabold mt-2">Mejoras continuas</h3>
                <p class="mt-2 text-lg">Reciba mejoras y nuevos módulos para sus plantillas sin incurrir en ningún costo adicional.</p>
            </div>

            <div class="benefit-card card-3 p-6">
                <div class="icon-placeholder icon-3"></div>
                <h3 class="text-2xl font-extrabold mt-2">Acceso de por vida</h3>
                <p class="mt-2 text-lg">Asegure su Acceso de por vida a todas las versiones futuras (del libro de Excel "Evaluación por Competencias") y sus evoluciones.</p>
            </div>

            <div class="benefit-card card-4 p-6">
                <div class="icon-placeholder icon-4"></div>
                <h3 class="text-2xl font-extrabold mt-2">Comunidad Thinkers</h3>
                <p class="mt-2 text-lg">Acceso a comunidad exclusiva, donde podrá descargar el libro de trabajo, recibir notificaciones de actualizaciones y obtener soporte directo.</p>
            </div>

        </div>
    </main>
</body>
</html>
