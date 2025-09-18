<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GME | Grúas y Maniobras</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.1.1/css/all.min.css">
    <style>
        body {
            font-family: 'Inter', sans-serif;
            overflow-x: hidden;
            background-color: #f4f7f9;
            color: #1e293b;
        }
        .bg-gme-blue { background-color: #1e293b; }
        .bg-gme-red { background-color: #ef4444; }
        .text-gme-red { color: #ef4444; }
        .text-gme-blue { color: #1e293b; }
        .service-card {
            transition: transform 0.3s ease, box-shadow 0.3s ease, border-color 0.3s ease;
            border: 2px solid transparent;
            cursor: pointer;
        }
        .service-card:hover {
            transform: translateY(-10px) scale(1.02);
            box-shadow: 0 20px 40px rgba(0,0,0,0.1);
            border-color: #ef4444;
        }
        .btn-primary {
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        .btn-primary:hover {
            transform: translateY(-3px);
            box-shadow: 0 10px 20px rgba(0,0,0,0.2);
        }
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(30px); }
            to { opacity: 1; transform: translateY(0); }
        }
        .animate-fade-in { animation: fadeIn 0.8s ease-out; }
        .toast {
            position: fixed;
            bottom: 20px;
            left: 50%;
            transform: translateX(-50%);
            padding: 14px 28px;
            background-color: rgba(30, 41, 59, 0.95);
            color: white;
            border-radius: 9999px;
            box-shadow: 0 6px 12px rgba(0, 0, 0, 0.2);
            opacity: 0;
            visibility: hidden;
            transition: opacity 0.4s ease, visibility 0.4s ease;
            z-index: 1000;
        }
        .toast.show {
            opacity: 1;
            visibility: visible;
        }
        .service-icon {
            font-size: 3.5rem;
            margin-bottom: 1rem;
            color: #ef4444;
        }
        .section-header {
            position: relative;
            padding-bottom: 1rem;
        }
        .section-header::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 80px;
            height: 4px;
            background-color: #ef4444;
            border-radius: 2px;
        }
        /* New Hero Section Styling */
        .hero-section {
            background-image: url('Grupo GME (1).jpg');
            background-position: center;
            background-repeat: no-repeat;
            background-size: cover;
            position: relative;
            height: 500px; /* Adjust height as needed */
            width: 100%;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            border-radius: 0 0 40px 40px;
            box-shadow: 0 20px 40px rgba(0,0,0,0.3);
        }
        .hero-section::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.4); /* Overlay to make text readable */
            border-radius: inherit;
        }
        .hero-content {
            position: relative;
            z-index: 10;
            color: white;
            padding: 2rem;
            max-width: 800px;
        }
    </style>
</head>
<body class="flex flex-col min-h-screen">

    <!-- Header -->
    <header class="bg-gme-blue text-white shadow-xl rounded-b-[40px]">
        <div class="container mx-auto px-6 py-8 flex flex-col sm:flex-row justify-between items-center">
            <h1 class="text-5xl font-extrabold mb-4 sm:mb-0 drop-shadow-lg">GME 🏗️</h1>
            <nav class="space-x-4 sm:space-x-8 mt-4 sm:mt-0 text-lg font-medium">
                <a href="#about" class="hover:text-gme-red transition-colors duration-300">Sobre Nosotros</a>
                <a href="#services" class="hover:text-gme-red transition-colors duration-300">Servicios</a>
                <a href="#brands" class="hover:text-gme-red transition-colors duration-300">Marcas</a>
                <a href="#quote" class="hover:text-gme-red transition-colors duration-300">Cotización</a>
            </nav>
        </div>
    </header>

    <main class="flex-grow">
        <!-- Hero Section with uploaded image -->
        <section class="hero-section">
            <div class="hero-content">
                <!-- Content is part of the image, so we'll leave this section empty or with a simple CTA -->
                <a href="#quote" class="inline-block bg-gme-red text-white font-bold py-4 px-10 rounded-full shadow-lg hover:bg-red-600 transition-colors duration-300 btn-primary">
                    ¡Cotiza tu proyecto! 📝
                </a>
            </div>
        </section>

        <!-- About Us Section -->
        <section id="about" class="py-24 bg-white rounded-t-[40px] -mt-10 relative z-20 shadow-inner">
            <div class="container mx-auto px-6">
                <h3 class="text-4xl font-extrabold text-center mb-16 text-gme-blue section-header">
                    Sobre Nosotros 🤝
                </h3>
                <div class="grid grid-cols-1 md:grid-cols-2 gap-16 items-start">
                    <div>
                        <h4 class="text-2xl font-bold text-gme-blue mb-4">Misión 🎯</h4>
                        <p class="text-gray-700 leading-relaxed text-lg">Como **Gigantes de Acero**, nuestra misión es resolver los desafíos logísticos y de elevación más complejos, brindando soluciones integrales con grúas y equipos industriales de vanguardia, respaldadas por una cobertura nacional y los más altos estándares de calidad. Lo logramos mediante la sinergia con empresas líderes a nivel mundial y el compromiso inquebrantable de nuestro equipo especializado, garantizando la seguridad y la satisfacción total de nuestros clientes en cada maniobra.</p>
                    </div>
                    <div>
                        <h4 class="text-2xl font-bold text-gme-blue mb-4">Visión 🚀</h4>
                        <p class="text-gray-700 leading-relaxed text-lg">Ser la empresa líder y de referencia en México en soluciones integrales y logística de equipos industriales. Nos proyectamos como el socio estratégico indispensable para cualquier empresa o persona que requiera excelencia en el manejo de maquinaria, distinguiéndonos por una operación impecable fundamentada en la honestidad, la solidaridad y un compromiso inquebrantable con el cliente.</p>
                    </div>
                </div>
                <div class="mt-20 text-center">
                    <h4 class="text-2xl font-bold text-gme-blue mb-6">Nuestros Valores ✨</h4>
                    <ul class="flex flex-wrap justify-center gap-4 text-center text-white font-medium">
                        <li class="bg-gme-red rounded-full px-6 py-2 shadow-md hover:bg-red-500 transition-colors">Responsabilidad Social</li>
                        <li class="bg-gme-red rounded-full px-6 py-2 shadow-md hover:bg-red-500 transition-colors">Conciencia Ambiental</li>
                        <li class="bg-gme-red rounded-full px-6 py-2 shadow-md hover:bg-red-500 transition-colors">Servicio al Cliente</li>
                        <li class="bg-gme-red rounded-full px-6 py-2 shadow-md hover:bg-red-500 transition-colors">Honestidad</li>
                        <li class="bg-gme-red rounded-full px-6 py-2 shadow-md hover:bg-red-500 transition-colors">Sinceridad</li>
                        <li class="bg-gme-red rounded-full px-6 py-2 shadow-md hover:bg-red-500 transition-colors">Transparencia</li>
                        <li class="bg-gme-red rounded-full px-6 py-2 shadow-md hover:bg-red-500 transition-colors">Solidaridad</li>
                    </ul>
                </div>
            </div>
        </section>

        <!-- Services Section -->
        <section id="services" class="py-24 bg-gray-100">
            <div class="container mx-auto px-6">
                <h3 class="text-4xl font-extrabold text-center mb-4 text-gme-blue section-header">
                    Nuestros Servicios 🛠️
                </h3>
                <p class="text-center text-xl font-medium text-gray-700 mb-16">Nuestra promesa es la **excelencia en cada maniobra**.</p>
                <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-12">
                    
                    <!-- Servicio 1: Grúas Industriales -->
                    <div class="bg-white rounded-3xl shadow-lg p-10 service-card text-center" data-service="grúas industriales">
                        <i class="fas fa-truck-monster service-icon"></i>
                        <h4 class="text-2xl font-bold text-gme-blue mb-2">Grúas Industriales</h4>
                        <p class="text-gray-600">Contamos con grúas articuladas, telescópicas, tipo Titán y todo terreno. Ideales para cualquier desafío de elevación.</p>
                    </div>

                    <!-- Servicio 2: Remolque y Transporte -->
                    <div class="bg-white rounded-3xl shadow-lg p-10 service-card text-center" data-service="remolque y transporte de carga">
                        <i class="fas fa-trailer service-icon"></i>
                        <h4 class="text-2xl font-bold text-gme-blue mb-2">Remolque y Transporte de Carga</h4>
                        <p class="text-gray-600">Trailer con Plataforma, Remolque Cama Baja, Remolque LowBoy y Remolque para Carga Sobredimensionada.</p>
                    </div>

                    <!-- Servicio 3: Montacargas -->
                    <div class="bg-white rounded-3xl shadow-lg p-10 service-card text-center" data-service="montacargas">
                        <i class="fas fa-pallet service-icon"></i>
                        <h4 class="text-2xl font-bold text-gme-blue mb-2">Montacargas</h4>
                        <p class="text-gray-600">Montacargas de Pasillo, de Combustión, Eléctricos y Todo-Terreno. Soluciones de movilidad para tus equipos.</p>
                    </div>

                    <!-- Servicio 4: Plataformas -->
                    <div class="bg-white rounded-3xl shadow-lg p-10 service-card text-center" data-service="plataformas">
                        <i class="fas fa-toolbox service-icon"></i>
                        <h4 class="text-2xl font-bold text-gme-blue mb-2">Plataformas</h4>
                        <p class="text-gray-600">Plataformas articuladas, de tijera y telescópicas, tanto eléctricas como de combustión.</p>
                    </div>

                    <!-- Servicio 5: Maniobras y Cargas Especiales -->
                    <div class="bg-white rounded-3xl shadow-lg p-10 service-card text-center" data-service="maniobras y cargas especiales">
                        <i class="fas fa-route service-icon"></i>
                        <h4 class="text-2xl font-bold text-gme-blue mb-2">Maniobras y Cargas Especiales</h4>
                        <p class="text-gray-600">Movimiento de maquinaria sobredimensionada, cargas sueltas y maniobras especializadas. Somos expertos en logística.</p>
                    </div>

                    <!-- Servicio 6: Entarimado -->
                    <div class="bg-white rounded-3xl shadow-lg p-10 service-card text-center" data-service="entarimado">
                        <i class="fas fa-warehouse service-icon"></i>
                        <h4 class="text-2xl font-bold text-gme-blue mb-2">Entarimado</h4>
                        <p class="text-gray-600">Servicio especializado para el manejo seguro de mercancía y equipos sensibles.</p>
                    </div>
                    
                    <!-- NUEVO SERVICIO: Herrería -->
                    <div class="bg-white rounded-3xl shadow-lg p-10 service-card text-center" data-service="herreria">
                        <i class="fas fa-gavel service-icon"></i>
                        <h4 class="text-2xl font-bold text-gme-blue mb-2">Herrería</h4>
                        <p class="text-gray-600">Fabricación y montaje de estructuras metálicas, soldadura especializada y trabajos de metal en general.</p>
                    </div>

                    <!-- NUEVO SERVICIO: Pailería -->
                    <div class="bg-white rounded-3xl shadow-lg p-10 service-card text-center" data-service="paileria">
                        <i class="fas fa-cogs service-icon"></i>
                        <h4 class="text-2xl font-bold text-gme-blue mb-2">Pailería</h4>
                        <p class="text-gray-600">Diseño, fabricación y reparación de tanques, silos, conductos, tolvas y otros recipientes industriales.</p>
                    </div>

                </div>
            </div>
        </section>

        <!-- Brands Section -->
        <section id="brands" class="py-24 bg-white">
            <div class="container mx-auto px-6">
                <h3 class="text-4xl font-extrabold text-center mb-16 text-gme-blue section-header">
                    Nuestras Principales Marcas 🔧
                </h3>
                
                <div class="grid grid-cols-2 sm:grid-cols-3 md:grid-cols-4 lg:grid-cols-6 gap-6 text-center items-center justify-center">
                    <div class="bg-gray-100 rounded-xl p-4 shadow-inner text-lg font-semibold text-gray-800">Liebherr</div>
                    <div class="bg-gray-100 rounded-xl p-4 shadow-inner text-lg font-semibold text-gray-800">Grove</div>
                    <div class="bg-gray-100 rounded-xl p-4 shadow-inner text-lg font-semibold text-gray-800">Hiab</div>
                    <div class="bg-gray-100 rounded-xl p-4 shadow-inner text-lg font-semibold text-gray-800">Hyster</div>
                    <div class="bg-gray-100 rounded-xl p-4 shadow-inner text-lg font-semibold text-gray-800">Caterpillar</div>
                    <div class="bg-gray-100 rounded-xl p-4 shadow-inner text-lg font-semibold text-gray-800">JLG</div>
                    <div class="bg-gray-100 rounded-xl p-4 shadow-inner text-lg font-semibold text-gray-800">Genie</div>
                    <div class="bg-gray-100 rounded-xl p-4 shadow-inner text-lg font-semibold text-gray-800">Hangcha</div>
                    <div class="bg-gray-100 rounded-xl p-4 shadow-inner text-lg font-semibold text-gray-800">Yale</div>
                    <div class="bg-gray-100 rounded-xl p-4 shadow-inner text-lg font-semibold text-gray-800">Mitsubishi</div>
                    <div class="bg-gray-100 rounded-xl p-4 shadow-inner text-lg font-semibold text-gray-800">Nissan</div>
                    <div class="bg-gray-100 rounded-xl p-4 shadow-inner text-lg font-semibold text-gray-800">National</div>
                </div>
            </div>
        </section>

        <!-- Quote Form Section -->
        <section id="quote" class="py-24 bg-gray-100">
            <div class="container mx-auto px-6">
                <h3 class="text-4xl font-extrabold text-center mb-16 text-gme-blue section-header">
                    Cotiza tu Proyecto 📝
                </h3>
                <div class="max-w-3xl mx-auto bg-white p-10 rounded-3xl shadow-xl border-t-4 border-gme-red">
                    <form id="quote-form" class="space-y-6">
                        <div>
                            <label for="name" class="block text-gray-700 font-semibold mb-2">Nombre completo</label>
                            <input type="text" id="name" name="name" class="w-full p-4 rounded-xl border border-gray-300 focus:outline-none focus:ring-4 focus:ring-gme-red" required>
                        </div>
                        <div>
                            <label for="email" class="block text-gray-700 font-semibold mb-2">Correo electrónico</label>
                            <input type="email" id="email" name="email" class="w-full p-4 rounded-xl border border-gray-300 focus:outline-none focus:ring-4 focus:ring-gme-red" required>
                        </div>
                        <div>
                            <label for="phone" class="block text-gray-700 font-semibold mb-2">Número Celular</label>
                            <input type="tel" id="phone" name="phone" class="w-full p-4 rounded-xl border border-gray-300 focus:outline-none focus:ring-4 focus:ring-gme-red" required>
                        </div>
                        <div>
                            <label for="service" class="block text-gray-700 font-semibold mb-2">Tipo de Servicio</label>
                            <select id="service" name="service" class="w-full p-4 rounded-xl border border-gray-300 focus:outline-none focus:ring-4 focus:ring-gme-red" required>
                                <option value="">Selecciona un servicio... 👇</option>
                                <option value="grúas industriales">Grúas Industriales</option>
                                <option value="remolque y transporte de carga">Remolque y Transporte de Carga</option>
                                <option value="montacargas">Montacargas</option>
                                <option value="plataformas">Plataformas</option>
                                <option value="maniobras y cargas especiales">Maniobras y Cargas Especiales</option>
                                <option value="entarimado">Entarimado</option>
                                <option value="herreria">Herrería</option>
                                <option value="paileria">Pailería</option>
                            </select>
                        </div>
                        
                        <div class="space-y-4 pt-4 border-t-2 border-gray-200">
                            <h4 class="text-lg font-bold text-gray-700">Detalles del Proyecto</h4>
                            <div>
                                <label for="project-description" class="block text-gray-700 font-semibold mb-2">Descripción del proyecto</label>
                                <textarea id="project-description" name="project-description" rows="3" class="w-full p-4 rounded-xl border border-gray-300 focus:outline-none focus:ring-4 focus:ring-gme-red" placeholder="Describe brevemente la naturaleza del proyecto" required></textarea>
                            </div>
                            <div>
                                <label for="location" class="block text-gray-700 font-semibold mb-2">Ubicación y lugar</label>
                                <input type="text" id="location" name="location" class="w-full p-4 rounded-xl border border-gray-300 focus:outline-none focus:ring-4 focus:ring-gme-red" placeholder="Ej: Calle 123, Colonia XYZ, Ciudad" required>
                            </div>
                            <div>
                                <label for="dates" class="block text-gray-700 font-semibold mb-2">Fechas</label>
                                <input type="text" id="dates" name="dates" class="w-full p-4 rounded-xl border border-gray-300 focus:outline-none focus:ring-4 focus:ring-gme-red" placeholder="Ej: 15 de Octubre de 2024 o 'Flexible'" required>
                            </div>
                            <div>
                                <label for="more-details" class="block text-gray-700 font-semibold mb-2">Más detalles</label>
                                <textarea id="more-details" name="more-details" rows="3" class="w-full p-4 rounded-xl border border-gray-300 focus:outline-none focus:ring-4 focus:ring-gme-red" placeholder="Cualquier información adicional, como tipo de maquinaria, peso, etc."></textarea>
                            </div>
                        </div>

                        <button id="generate-button" type="submit" class="w-full bg-gme-red text-white font-bold py-5 px-6 rounded-full shadow-lg hover:bg-red-600 transition-colors duration-300 btn-primary text-xl">
                            <span id="button-text">Enviar Cotización por Correo ✉️</span>
                        </button>
                    </form>
                </div>
            </div>
        </section>
        
        <!-- WhatsApp Contact Section (New) -->
        <section class="py-24 bg-gme-red text-white text-center">
            <div class="container mx-auto px-6">
                <h3 class="text-4xl md:text-5xl font-extrabold mb-8 drop-shadow-lg">
                    ¡Hablemos de tu proyecto! 🗣️
                </h3>
                <p class="text-xl md:text-2xl mb-10 font-medium">
                    Envíanos un mensaje por WhatsApp para una atención inmediata.
                </p>
                <a href="https://wa.me/524623699025" target="_blank" class="inline-flex items-center space-x-4 bg-green-500 hover:bg-green-600 text-white font-bold text-lg md:text-xl py-5 px-10 rounded-full shadow-2xl transition-all duration-300 transform hover:scale-105">
                    <i class="fab fa-whatsapp text-4xl md:text-5xl"></i>
                    <span>Contactar por WhatsApp</span>
                </a>
            </div>
        </section>

        <!-- Maneuvers Yard Location Section -->
        <section id="maneuvers-yard" class="py-24 bg-white">
            <div class="container mx-auto px-6">
                <h3 class="text-4xl font-extrabold text-center mb-16 text-gme-blue section-header">
                    Ubicación de Nuestro Patio de Maniobras 📍
                </h3>
                <div class="max-w-4xl mx-auto shadow-2xl rounded-3xl overflow-hidden border-4 border-gme-red">
                    <iframe
                        src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3729.079237000201!2d-101.336888!3d20.760416!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x0%3A0x0!2zR01FIHwgUGF0aW8gZGUgTWFuaW9icmFz!5e0!3m2!1ses-419!2smx!4v1715873215286!5m2!1ses-419!2smx"
                        width="100%"
                        height="450"
                        style="border:0;"
                        allowfullscreen=""
                        loading="lazy"
                        referrerpolicy="no-referrer-when-downgrade"
                        title="Ubicación de GME - Patio de Maniobras">
                    </iframe>
                </div>
            </div>
        </section>
    </main>

    <!-- Footer -->
    <footer class="bg-gme-blue text-white py-12 mt-20 rounded-t-[40px] shadow-2xl">
        <div class="container mx-auto px-6 text-center">
            <div class="mb-6">
                <p class="font-bold text-xl">Contacto GME</p>
                <p class="text-lg">Teléfono: <a href="tel:+524623699025" class="hover:text-gme-red transition-colors duration-300">(+52) 462-369-9025</a></p>
                <p class="text-lg">Correo: <a href="mailto:ventas.gruasgme@gmail.com" class="hover:text-gme-red transition-colors duration-300">ventas.gruasgme@gmail.com</a></p>
            </div>
            <p>&copy; 2024 GME. Todos los derechos reservados. 👷‍♂️</p>
        </div>
    </footer>

    <!-- Modal para mensajes -->
    <div id="message-modal" class="fixed inset-0 bg-gray-900 bg-opacity-50 flex items-center justify-center p-4 hidden z-50">
        <div class="bg-white rounded-xl p-8 shadow-2xl max-w-sm w-full text-center transform scale-95 transition-transform duration-300">
            <p id="modal-text" class="text-lg font-semibold text-gray-800 mb-4"></p>
            <button id="modal-close" class="bg-gme-red text-white font-bold py-3 px-8 rounded-full hover:bg-red-600 transition-colors duration-300 btn-primary">Cerrar</button>
        </div>
    </div>

    <!-- Toast de notificaciones -->
    <div id="toast" class="toast"></div>

    <script type="module">
        // =========================================================================
        // SCRIPTS DE APLICACIÓN
        // =========================================================================

        document.addEventListener('DOMContentLoaded', () => {

            // =========================================================================
            // VARIABLES GLOBALES Y SELECTORES DE ELEMENTOS
            // =========================================================================
            const form = document.getElementById('quote-form');
            const serviceSelect = document.getElementById('service');
            const serviceCards = document.querySelectorAll('.service-card');
            
            // Mapeo de valores de servicio a nombres completos
            const servicesMap = {
                "grúas industriales": "Grúas Industriales",
                "remolque y transporte de carga": "Remolque y Transporte de Carga",
                "montacargas": "Montacargas",
                "plataformas": "Plataformas",
                "maniobras y cargas especiales": "Maniobras y Cargas Especiales",
                "entarimado": "Entarimado",
                "herreria": "Herrería",
                "paileria": "Pailería"
            };
            
            // =========================================================================
            // FUNCIONES DE UTILIDAD PARA LA INTERFAZ DE USUARIO
            // =========================================================================

            /**
             * Muestra un modal con un mensaje personalizado.
             * @param {string} message - El mensaje a mostrar en el modal.
             */
            const showMessageModal = (message) => {
                const messageModal = document.getElementById('message-modal');
                const modalText = document.getElementById('modal-text');
                modalText.textContent = message;
                messageModal.classList.remove('hidden');
                messageModal.querySelector('div').classList.add('scale-100');
            };

            // Cierra el modal de mensajes al hacer clic en el botón.
            document.getElementById('modal-close').addEventListener('click', () => {
                const messageModal = document.getElementById('message-modal');
                messageModal.querySelector('div').classList.remove('scale-100');
                messageModal.querySelector('div').classList.add('scale-95');
                setTimeout(() => {
                    messageModal.classList.add('hidden');
                }, 300);
            });
            
            // =========================================================================
            // MANEJADORES DE EVENTOS
            // =========================================================================
            
            // Asigna el valor del servicio al select cuando se hace clic en una tarjeta de servicio.
            serviceCards.forEach(card => {
                card.addEventListener('click', () => {
                    const serviceType = card.dataset.service;
                    serviceSelect.value = serviceType;
                    document.getElementById('quote').scrollIntoView({ behavior: 'smooth' });
                });
            });
            
            // Maneja el envío del formulario de cotización.
            form.addEventListener('submit', (e) => {
                e.preventDefault();

                const formData = new FormData(form);
                const name = formData.get('name');
                const email = formData.get('email');
                const phone = formData.get('phone');
                const service = formData.get('service');
                const projectDescription = formData.get('project-description');
                const location = formData.get('location');
                const dates = formData.get('dates');
                const moreDetails = formData.get('more-details');

                // Genera el asunto y cuerpo del correo
                const serviceName = servicesMap[service] || service;
                const subject = encodeURIComponent(`Solicitud de Cotización GME: ${serviceName}`);
                
                // Incluye toda la información del campo de detalles en el cuerpo del correo.
                const body = encodeURIComponent(
                    `Hola, \n\nHe completado el formulario de cotización en su sitio web. Aquí están mis detalles:\n\n` +
                    `Nombre: ${name}\n` +
                    `Correo electrónico: ${email}\n` +
                    `Número Celular: ${phone}\n` +
                    `Servicio solicitado: ${serviceName}\n\n` +
                    `--- Detalles del Proyecto ---\n` +
                    `Descripción: ${projectDescription}\n` +
                    `Ubicación: ${location}\n` +
                    `Fechas: ${dates}\n` +
                    `Más detalles: ${moreDetails}\n\n` +
                    `Espero su respuesta. \n\nSaludos,\n${name}`
                );

                // Abre el cliente de correo con el enlace mailto
                const mailtoLink = `mailto:ventas.gruasgme@gmail.com?subject=${subject}&body=${body}`;
                window.location.href = mailtoLink;
                
                // Muestra un modal de confirmación
                showMessageModal("Tu solicitud ha sido enviada. Se abrirá tu cliente de correo para completar el proceso.");
            });
        });
    </script>
</body>
</html>
![Grupo GME (1)](https://github.com/user-attachments/assets/2b84ec2f-33b7-4a89-a3ce-a3a35857fef1)
