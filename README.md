<!DOCTYPE html>
<html lang="es" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>All Williams | Marketing Estratégico y Consciente</title>
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Google Fonts: Poppins -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600;700;800&display=swap" rel="stylesheet">
    <!-- Font Awesome for Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <script>
        // Custom Tailwind theme configuration
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        'sans': ['Poppins', 'sans-serif'],
                    },
                    colors: {
                        'brand-neutral': '#F5F5F5', // Light gray background
                        'brand-dark': '#1a202c',   // Dark text
                        'brand-accent': '#0891B2', // Vibrant Teal
                        'brand-accent-hover': '#06b6d4',
                    }
                }
            }
        }
    </script>
    <style>
        /* Simple animation for sections */
        .section-fade-in {
            opacity: 0;
            transform: translateY(20px);
            transition: opacity 0.6s ease-out, transform 0.6s ease-out;
        }
        .section-fade-in.visible {
            opacity: 1;
            transform: translateY(0);
        }
    </style>
</head>
<body class="bg-brand-neutral text-brand-dark">

    <!-- Header & Navigation -->
    <header id="header" class="bg-white/80 backdrop-blur-md sticky top-0 z-50 shadow-sm">
        <nav class="container mx-auto px-6 py-4 flex justify-between items-center">
            <a href="#" class="text-2xl font-bold text-brand-dark">All Williams.</a>
            <div class="hidden md:flex space-x-8 items-center">
                <a href="#sobre-mi" class="text-gray-600 hover:text-brand-accent transition-colors">Sobre mí</a>
                <a href="#servicios" class="text-gray-600 hover:text-brand-accent transition-colors">Servicios</a>
                <a href="#testimonios" class="text-gray-600 hover:text-brand-accent transition-colors">Resultados</a>
                <a href="#contacto" class="bg-brand-accent text-white px-5 py-2 rounded-full hover:bg-brand-accent-hover transition-transform transform hover:scale-105">Hablemos</a>
            </div>
            <button id="mobile-menu-button" class="md:hidden text-brand-dark">
                <i class="fas fa-bars fa-lg"></i>
            </button>
        </nav>
        <!-- Mobile Menu -->
        <div id="mobile-menu" class="hidden md:hidden">
            <a href="#sobre-mi" class="block text-center py-2 px-4 text-sm text-gray-600 hover:bg-gray-200">Sobre mí</a>
            <a href="#servicios" class="block text-center py-2 px-4 text-sm text-gray-600 hover:bg-gray-200">Servicios</a>
            <a href="#testimonios" class="block text-center py-2 px-4 text-sm text-gray-600 hover:bg-gray-200">Resultados</a>
            <a href="#contacto" class="block text-center py-3 px-4 text-sm bg-brand-accent text-white hover:bg-brand-accent-hover">Hablemos</a>
        </div>
    </header>

    <main class="container mx-auto px-6">

        <!-- 1. Hero Section (Inicio) -->
        <section id="inicio" class="text-center py-20 md:py-32 section-fade-in">
            <h1 class="text-4xl md:text-6xl font-extrabold text-brand-dark leading-tight">
                Estrategia con <span class="text-brand-accent">alma.</span><br> Conexión con <span class="text-brand-accent">sentido.</span>
            </h1>
            <p class="mt-6 max-w-2xl mx-auto text-lg text-gray-600">
                Ayudo a marcas personales y pequeñas empresas a evolucionar en el mundo digital, creando conexiones emocionales que generan resultados reales.
            </p>
            <div class="mt-8 flex justify-center gap-4">
                <a href="#servicios" class="bg-brand-accent text-white px-8 py-3 rounded-full text-lg font-semibold hover:bg-brand-accent-hover transition-transform transform hover:scale-105">Descubre mis servicios</a>
                <a href="#contacto" class="bg-gray-200 text-brand-dark px-8 py-3 rounded-full text-lg font-semibold hover:bg-gray-300 transition-transform transform hover:scale-105">Agenda una llamada</a>
            </div>
        </section>

        <!-- 2. Sobre mí Section -->
        <section id="sobre-mi" class="py-20 flex flex-col md:flex-row items-center gap-12 section-fade-in">
            <div class="md:w-1/3">
                <img src="https://placehold.co/400x400/0891B2/FFFFFF?text=AW" alt="Foto de William, asesor de marketing" class="rounded-full shadow-2xl mx-auto">
            </div>
            <div class="md:w-2/3 text-center md:text-left">
                <h2 class="text-3xl font-bold text-brand-dark">Todo comunica. <span class="text-brand-accent">Tú eliges cómo.</span></h2>
                <p class="mt-4 text-lg text-gray-600">
                    Hola, soy William. Mi misión es ir más allá del marketing tradicional. Creo en el poder de la resonancia emocional y el valor humano para construir marcas que no solo venden, sino que también inspiran y perduran.
                </p>
                <p class="mt-4 text-gray-600">
                    Con una base sólida en análisis estratégico y una pasión por la evolución digital, te guiaré para que tu marca hable el lenguaje de tu cliente, creando una presencia digital auténtica y efectiva.
                </p>
            </div>
        </section>

        <!-- 3. Servicios Section -->
        <section id="servicios" class="py-20 section-fade-in">
            <div class="text-center mb-12">
                <h2 class="text-4xl font-bold text-brand-dark">Servicios para potenciar tu marca</h2>
                <p class="mt-4 max-w-2xl mx-auto text-lg text-gray-600">Soluciones estratégicas diseñadas para cada etapa de tu crecimiento.</p>
            </div>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Service Card 1 -->
                <div class="bg-white p-8 rounded-xl shadow-lg hover:shadow-2xl hover:-translate-y-2 transition-all duration-300">
                    <i class="fas fa-search-dollar fa-2x text-brand-accent"></i>
                    <h3 class="text-2xl font-bold mt-4">Diagnóstico de Marca</h3>
                    <p class="mt-2 text-gray-600">Análisis completo de tu presencia digital y redes sociales para identificar oportunidades clave.</p>
                </div>
                <!-- Service Card 2 -->
                <div class="bg-white p-8 rounded-xl shadow-lg hover:shadow-2xl hover:-translate-y-2 transition-all duration-300">
                    <i class="fab fa-instagram-square fa-2x text-brand-accent"></i>
                    <h3 class="text-2xl font-bold mt-4">Optimización de Instagram</h3>
                    <p class="mt-2 text-gray-600">Transformamos tu perfil para atraer a tu cliente ideal y comunicar tu valor de forma efectiva.</p>
                </div>
                <!-- Service Card 3 -->
                <div class="bg-white p-8 rounded-xl shadow-lg hover:shadow-2xl hover:-translate-y-2 transition-all duration-300">
                    <i class="fas fa-palette fa-2x text-brand-accent"></i>
                    <h3 class="text-2xl font-bold mt-4">Identidad Visual Básica</h3>
                    <p class="mt-2 text-gray-600">Diseño de logo, paleta de colores y tipografías que reflejen la esencia de tu marca.</p>
                </div>
                <!-- Service Card 4 -->
                <div class="bg-white p-8 rounded-xl shadow-lg hover:shadow-2xl hover:-translate-y-2 transition-all duration-300">
                    <i class="fas fa-calendar-alt fa-2x text-brand-accent"></i>
                    <h3 class="text-2xl font-bold mt-4">Contenido Estratégico</h3>
                    <p class="mt-2 text-gray-600">Calendarios de contenido mensuales diseñados para conectar, educar y convertir.</p>
                </div>
                <!-- Service Card 5 -->
                <div class="bg-white p-8 rounded-xl shadow-lg hover:shadow-2xl hover:-translate-y-2 transition-all duration-300">
                    <i class="fas fa-bullseye fa-2x text-brand-accent"></i>
                    <h3 class="text-2xl font-bold mt-4">Planes de Marketing</h3>
                    <p class="mt-2 text-gray-600">Desde planes básicos hasta estratégicos para guiar todas tus acciones de marketing.</p>
                </div>
                <!-- Service Card 6 -->
                <div class="bg-brand-accent text-white p-8 rounded-xl shadow-lg hover:shadow-2xl hover:-translate-y-2 transition-all duration-300">
                    <i class="fas fa-user-tie fa-2x"></i>
                    <h3 class="text-2xl font-bold mt-4">Asesorías Personalizadas</h3>
                    <p class="mt-2">Sesiones 1 a 1 para resolver tus dudas y trazar un plan de acción claro y conciso.</p>
                </div>
            </div>
        </section>

        <!-- 4. Testimonios Section -->
        <section id="testimonios" class="py-20 section-fade-in">
             <div class="text-center mb-12">
                <h2 class="text-4xl font-bold text-brand-dark">Resultados que inspiran</h2>
                <p class="mt-4 max-w-2xl mx-auto text-lg text-gray-600">Lo que dicen quienes ya han transformado su marca.</p>
            </div>
            <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
                <!-- Testimonial 1 -->
                <div class="bg-white p-8 rounded-xl shadow-lg">
                    <p class="text-gray-600 italic">"William no solo me dio una estrategia, me dio claridad y confianza. Mis interacciones aumentaron un 200% en el primer mes. ¡Increíble!"</p>
                    <div class="flex items-center mt-4">
                        <img src="https://placehold.co/50x50/cccccc/FFFFFF?text=A" alt="Cliente satisfecho" class="rounded-full">
                        <div class="ml-4">
                            <p class="font-bold">Ana López</p>
                            <p class="text-sm text-gray-500">Emprendedora</p>
                        </div>
                    </div>
                </div>
                <!-- Testimonial 2 -->
                <div class="bg-white p-8 rounded-xl shadow-lg">
                    <p class="text-gray-600 italic">"La asesoría fue un antes y un después. Entendí cómo conectar realmente con mi audiencia. Lo recomiendo totalmente."</p>
                    <div class="flex items-center mt-4">
                        <img src="https://placehold.co/50x50/cccccc/FFFFFF?text=C" alt="Cliente satisfecho" class="rounded-full">
                        <div class="ml-4">
                            <p class="font-bold">Carlos Vidal</p>
                            <p class="text-sm text-gray-500">Dueño de Pequeño Negocio</p>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- 5. Lead Magnet Section -->
        <section id="guia-gratuita" class="py-20 bg-white rounded-xl shadow-xl my-20 section-fade-in">
            <div class="container mx-auto px-6 text-center">
                <h2 class="text-3xl font-bold text-brand-dark">¿Listo para empezar con el pie derecho?</h2>
                <p class="mt-4 max-w-2xl mx-auto text-lg text-gray-600">Descarga mi guía gratuita y descubre los primeros pasos para construir una marca personal con estrategia y propósito.</p>
                <form class="mt-8 max-w-md mx-auto flex flex-col sm:flex-row gap-4">
                    <input type="email" placeholder="Tu mejor correo electrónico" class="w-full px-4 py-3 rounded-full border-2 border-gray-200 focus:outline-none focus:border-brand-accent" required>
                    <button type="submit" class="bg-brand-accent text-white px-8 py-3 rounded-full text-lg font-semibold hover:bg-brand-accent-hover transition-transform transform hover:scale-105">¡La quiero!</button>
                </form>
            </div>
        </section>

        <!-- 6. Contacto Section -->
        <section id="contacto" class="py-20 section-fade-in">
            <div class="text-center">
                <h2 class="text-4xl font-bold text-brand-dark">Hagamos que tu marca brille.</h2>
                <p class="mt-4 max-w-2xl mx-auto text-lg text-gray-600">¿Tienes un proyecto en mente o quieres una asesoría? Envíame un mensaje y empecemos a crear algo increíble juntos.</p>
                <div class="mt-8">
                     <a href="mailto:tuemail@allwilliams.com" class="bg-brand-dark text-white px-10 py-4 rounded-full text-lg font-semibold hover:bg-gray-800 transition-transform transform hover:scale-105 inline-block">
                        <i class="fas fa-envelope mr-2"></i> Envíame un correo
                    </a>
                </div>
            </div>
        </section>

    </main>

    <!-- Footer -->
    <footer class="bg-white mt-20">
        <div class="container mx-auto px-6 py-8 text-center text-gray-500">
            <p>&copy; 2025 All Williams. Todos los derechos reservados.</p>
            <div class="flex justify-center space-x-6 mt-4">
                <a href="#" class="hover:text-brand-accent"><i class="fab fa-instagram fa-lg"></i></a>
                <a href="#" class="hover:text-brand-accent"><i class="fab fa-linkedin-in fa-lg"></i></a>
            </div>
        </div>
    </footer>

    <!-- WhatsApp Button -->
    <a href="https://wa.me/TUNUMERODEWHATSAPP" target="_blank" class="fixed bottom-6 right-6 bg-green-500 text-white w-16 h-16 rounded-full flex items-center justify-center shadow-lg hover:bg-green-600 transition-transform transform hover:scale-110">
        <i class="fab fa-whatsapp fa-2x"></i>
    </a>

    <script>
        // Mobile Menu Toggle
        const mobileMenuButton = document.getElementById('mobile-menu-button');
        const mobileMenu = document.getElementById('mobile-menu');
        mobileMenuButton.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
        });

        // Fade-in sections on scroll
        const sections = document.querySelectorAll('.section-fade-in');
        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('visible');
                }
            });
        }, {
            threshold: 0.1
        });
        sections.forEach(section => {
            observer.observe(section);
        });
    </script>
</body>
</html>


<!--
**AllWilliams/Allwilliams** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
