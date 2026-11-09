[index.html](https://github.com/user-attachments/files/34559810/index.html)
<!DOCTYPE html>
<html lang="es" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>FH Performance | Mecánica Automotriz & Maquinaria Vial</title>
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Font Awesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <!-- Google Fonts: Montserrat & Inter -->
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,300;0,400;0,600;0,700;0,800;0,900;1,800&family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        brand: {
                            red: '#DC2626',
                            redDark: '#991B1B',
                            redLight: '#EF4444',
                            black: '#0a0a0a',
                            darkCard: '#141414',
                            darkBorder: '#262626',
                            silver: '#D1D5DB',
                            silverLight: '#F3F4F6'
                        }
                    },
                    fontFamily: {
                        sans: ['Inter', 'sans-serif'],
                        heading: ['Montserrat', 'sans-serif'],
                    }
                }
            }
        }
    </script>
    <style>
        body {
            background-color: #080808;
            color: #e5e7eb;
            font-family: 'Inter', sans-serif;
        }
        .font-heading {
            font-family: 'Montserrat', sans-serif;
        }
        /* Custom Carbon Fiber / Racing Texture Background */
        .bg-carbon {
            background-color: #0b0b0b;
            background-image: 
                radial-gradient(circle at 50% 0%, rgba(220, 38, 38, 0.15) 0%, transparent 60%),
                radial-gradient(circle at 80% 80%, rgba(220, 38, 38, 0.08) 0%, transparent 50%),
                linear-gradient(0deg, rgba(10, 10, 10, 0.95), rgba(10, 10, 10, 0.95)),
                repeating-linear-gradient(45deg, #111 0, #111 2px, #0a0a0a 0, #0a0a0a 10px);
        }
        .text-glow-red {
            text-shadow: 0 0 15px rgba(220, 38, 38, 0.6);
        }
        .card-hover {
            transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
        }
        .card-hover:hover {
            transform: translateY(-6px);
            border-color: #dc2626;
            box-shadow: 0 12px 30px -10px rgba(220, 38, 38, 0.25);
        }
        .custom-scrollbar::-webkit-scrollbar {
            width: 8px;
        }
        .custom-scrollbar::-webkit-scrollbar-track {
            background: #0d0d0d;
        }
        .custom-scrollbar::-webkit-scrollbar-thumb {
            background: #dc2626;
            border-radius: 4px;
        }
    </style>
</head>
<body class="custom-scrollbar overflow-x-hidden">

    <!-- TOP ANNOUNCEMENT BAR -->
    <div class="bg-red-700 text-white text-xs sm:text-sm py-2 px-4 text-center font-medium flex items-center justify-center gap-2 shadow-md z-50 relative">
        <span class="inline-block w-2 h-2 rounded-full bg-white animate-pulse"></span>
        <span>Atención Integral en Moreno: Autos, Camionetas, Camiones y Maquinaria Vial</span>
        <a href="#contacto" class="underline hover:text-gray-200 ml-2 font-semibold">Consulte Ahora</a>
    </div>

    <!-- MAIN STICKY NAVIGATION -->
    <header class="sticky top-0 z-40 bg-black/90 backdrop-blur-md border-b border-neutral-800">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex items-center justify-between h-20">
                <!-- LOGO SVG RECREATION -->
                <a href="#" class="flex items-center gap-3 group">
                    <div class="relative flex items-center justify-center">
                        <svg class="w-12 h-12 transition-transform duration-300 group-hover:scale-105" viewBox="0 0 200 200" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <!-- Metallic Silver FH Outer Shadow -->
                            <path d="M25 40H60V80H110V40H145V160H110V115H60V160H25V40Z" fill="url(#silverGradient)"/>
                            <!-- Gear overlay top-right -->
                            <path d="M150 30 C160 30, 175 40, 178 55 L165 60 C163 53, 155 48, 148 48 L150 30 Z" fill="#DC2626"/>
                            <path d="M165 40 L180 35 L185 48 L172 52 Z" fill="#DC2626"/>
                            <path d="M178 58 L192 60 L188 74 L175 68 Z" fill="#DC2626"/>
                            <path d="M180 78 L194 85 L185 98 L173 88 Z" fill="#DC2626"/>
                            <circle cx="150" cy="70" r="32" stroke="#DC2626" stroke-width="14" stroke-dasharray="12 6" fill="none"/>
                            <defs>
                                <linearGradient id="silverGradient" x1="0" y1="0" x2="1" y2="1">
                                    <stop offset="0%" stop-color="#FFFFFF"/>
                                    <stop offset="50%" stop-color="#9CA3AF"/>
                                    <stop offset="100%" stop-color="#4B5563"/>
                                </linearGradient>
                            </defs>
                        </svg>
                    </div>
                    <div class="flex flex-col">
                        <div class="flex items-center gap-1 leading-none">
                            <span class="font-heading font-black text-2xl tracking-tighter text-transparent bg-clip-text bg-gradient-to-r from-white via-gray-200 to-gray-400">FH</span>
                            <span class="font-heading font-extrabold text-xl tracking-wider text-red-600 ml-1">PERFORMANCE</span>
                        </div>
                        <span class="text-[10px] sm:text-[11px] font-semibold tracking-[0.2em] text-gray-400 uppercase">Mecánica Automotriz</span>
                    </div>
                </a>

                <!-- DESKTOP NAV LINKS -->
                <nav class="hidden lg:flex items-center space-x-8 text-sm font-medium">
                    <a href="#inicio" class="text-white hover:text-red-500 transition-colors">Inicio</a>
                    <a href="#nosotros" class="text-gray-300 hover:text-red-500 transition-colors">Quiénes Somos</a>
                    <a href="#servicios" class="text-gray-300 hover:text-red-500 transition-colors">Servicios</a>
                    <a href="#liviana" class="text-gray-300 hover:text-red-500 transition-colors">Línea Liviana</a>
                    <a href="#pesada" class="text-gray-300 hover:text-red-500 transition-colors">Línea Pesada</a>
                    <a href="#contacto" class="text-gray-300 hover:text-red-500 transition-colors">Contacto</a>
                </nav>

                <!-- HEADER ACTION BUTTONS -->
                <div class="hidden sm:flex items-center gap-3">
                    <a href="https://instagram.com/rivadeoperfomance" target="_blank" rel="noopener font-medium" 
                       class="flex items-center gap-2 bg-neutral-900 border border-neutral-700 hover:border-pink-600 hover:text-pink-500 text-gray-200 px-3.5 py-2 rounded-xl text-xs sm:text-sm transition-all duration-300">
                        <i class="fab fa-instagram text-lg text-pink-500"></i>
                        <span class="hidden md:inline">@rivadeoperfomance</span>
                    </a>
                    <div class="relative group">
                        <button class="bg-red-600 hover:bg-red-700 text-white font-semibold px-4 py-2 rounded-xl text-xs sm:text-sm flex items-center gap-2 shadow-lg shadow-red-600/30 transition-all duration-300">
                            <i class="fab fa-whatsapp text-lg"></i>
                            <span>WhatsApp (2 Líneas)</span>
                            <i class="fas fa-chevron-down text-xs opacity-75"></i>
                        </button>
                        <!-- Dropdown choice for 2 Numbers -->
                        <div class="absolute right-0 mt-2 w-64 bg-neutral-900 border border-neutral-800 rounded-xl shadow-2xl p-2 hidden group-hover:block transition-all z-50">
                            <a href="https://wa.me/5491144720639?text=Hola!%20Consulta%20por%20L%C3%ADnea%20Liviana%20(Celular%201)" 
                               target="_blank" class="flex items-center gap-3 p-2.5 rounded-lg hover:bg-neutral-800 text-xs text-gray-200 hover:text-white">
                                <div class="w-8 h-8 rounded-full bg-emerald-950 text-emerald-400 flex items-center justify-center font-bold shrink-0">
                                    <i class="fas fa-car"></i>
                                </div>
                                <div>
                                    <div class="font-semibold text-emerald-400">Celular 1: +54 9 11 4472-0639</div>
                                    <div class="text-[10px] text-gray-400">Línea Liviana & Turnos</div>
                                </div>
                            </a>
                            <a href="https://wa.me/5491122845098?text=Hola!%20Consulta%20por%20L%C3%ADnea%20Pesada%20(Celular%202)" 
                               target="_blank" class="flex items-center gap-3 p-2.5 rounded-lg hover:bg-neutral-800 text-xs text-gray-200 hover:text-white mt-1 border-t border-neutral-800/80 pt-2">
                                <div class="w-8 h-8 rounded-full bg-amber-950 text-amber-400 flex items-center justify-center font-bold shrink-0">
                                    <i class="fas fa-truck-monster"></i>
                                </div>
                                <div>
                                    <div class="font-semibold text-amber-400">Celular 2: +54 9 11 2284-5098</div>
                                    <div class="text-[10px] text-gray-400">Línea Pesada & Maquinaria</div>
                                </div>
                            </a>
                        </div>
                    </div>
                </div>

                <!-- MOBILE MENU BUTTON -->
                <button id="mobile-menu-btn" class="lg:hidden text-gray-300 hover:text-white focus:outline-none p-2">
                    <i class="fas fa-bars text-2xl"></i>
                </button>
            </div>
        </div>

        <!-- MOBILE MENU DROPDOWN -->
        <div id="mobile-menu" class="hidden lg:hidden bg-neutral-950 border-b border-neutral-800 px-4 pt-3 pb-6 space-y-3">
            <a href="#inicio" class="block text-gray-200 font-medium py-2 border-b border-neutral-800">Inicio</a>
            <a href="#nosotros" class="block text-gray-200 font-medium py-2 border-b border-neutral-800">Quiénes Somos</a>
            <a href="#servicios" class="block text-gray-200 font-medium py-2 border-b border-neutral-800">Servicios</a>
            <a href="#liviana" class="block text-gray-200 font-medium py-2 border-b border-neutral-800">Línea Liviana</a>
            <a href="#pesada" class="block text-gray-200 font-medium py-2 border-b border-neutral-800">Línea Pesada</a>
            <a href="#contacto" class="block text-gray-200 font-medium py-2">Contacto</a>
            <div class="pt-4 flex flex-col gap-3">
                <a href="https://wa.me/5491144720639?text=Hola!%20Consulta%20Celular%201" target="_blank"
                   class="w-full bg-emerald-600 hover:bg-emerald-700 text-white py-3 rounded-xl text-center font-semibold text-xs flex items-center justify-center gap-2">
                    <i class="fab fa-whatsapp text-lg"></i> Celular 1: +54 9 11 4472-0639
                </a>
                <a href="https://wa.me/5491122845098?text=Hola!%20Consulta%20Celular%202" target="_blank"
                   class="w-full bg-red-600 hover:bg-red-700 text-white py-3 rounded-xl text-center font-semibold text-xs flex items-center justify-center gap-2">
                    <i class="fab fa-whatsapp text-lg"></i> Celular 2: +54 9 11 2284-5098
                </a>
                <a href="https://instagram.com/rivadeoperfomance" target="_blank"
                   class="w-full bg-neutral-800 border border-neutral-700 text-pink-400 py-2.5 rounded-xl text-center font-semibold text-sm flex items-center justify-center gap-2">
                    <i class="fab fa-instagram text-lg"></i> Instagram @rivadeoperfomance
                </a>
            </div>
        </div>
    </header>

    <!-- HERO SECTION -->
<!-- ... existing code -->
                    <!-- HERO ACTION BUTTONS -->
                    <div class="pt-4 flex flex-col sm:flex-row items-center justify-center lg:justify-start gap-4">
                        <a href="https://wa.me/5491144720639?text=Hola%20FH%20Performance!%20Consulta%20a%20Celular%201" 
                           target="_blank"
                           class="w-full sm:w-auto px-6 py-4 rounded-xl bg-gradient-to-r from-emerald-600 to-emerald-500 hover:from-emerald-500 hover:to-emerald-400 text-white font-bold text-xs sm:text-sm tracking-wide shadow-xl shadow-emerald-900/40 flex items-center justify-center gap-3 transition-all duration-300 transform hover:-translate-y-0.5">
                            <i class="fab fa-whatsapp text-xl"></i>
                            <div class="text-left">
                                <div class="text-[10px] font-normal opacity-90">WHATSAPP CELULAR 1</div>
                                <div class="font-extrabold">+54 9 11 4472-0639</div>
                            </div>
                        </a>

                        <a href="https://wa.me/5491122845098?text=Hola%20FH%20Performance!%20Consulta%20a%20Celular%202" 
                           target="_blank"
                           class="w-full sm:w-auto px-6 py-4 rounded-xl bg-gradient-to-r from-red-700 to-red-600 hover:from-red-600 hover:to-red-500 text-white font-bold text-xs sm:text-sm tracking-wide shadow-xl shadow-red-900/40 flex items-center justify-center gap-3 transition-all duration-300 transform hover:-translate-y-0.5">
                            <i class="fab fa-whatsapp text-xl"></i>
                            <div class="text-left">
                                <div class="text-[10px] font-normal opacity-90">WHATSAPP CELULAR 2</div>
                                <div class="font-extrabold">+54 9 11 2284-5098</div>
                            </div>
                        </a>
                    </div>
                </div>
<!-- ... existing code -->
                    <!-- Direct Contact Badges -->
                    <div class="flex flex-wrap gap-4 pt-2">
                        <a href="https://wa.me/5491144720639" target="_blank" class="flex items-center gap-3 bg-neutral-900 hover:bg-neutral-800 border border-neutral-800 px-4 py-3 rounded-xl text-xs font-semibold text-gray-200">
                            <i class="fab fa-whatsapp text-emerald-500 text-lg"></i>
                            <span>Celular 1: +54 9 11 4472-0639</span>
                        </a>
                        <a href="https://wa.me/5491122845098" target="_blank" class="flex items-center gap-3 bg-neutral-900 hover:bg-neutral-800 border border-neutral-800 px-4 py-3 rounded-xl text-xs font-semibold text-gray-200">
                            <i class="fab fa-whatsapp text-red-500 text-lg"></i>
                            <span>Celular 2: +54 9 11 2284-5098</span>
                        </a>
                        <a href="mailto:rivadeodanielhoracio63@gmail.com" class="flex items-center gap-3 bg-neutral-900 hover:bg-neutral-800 border border-neutral-800 px-4 py-3 rounded-xl text-xs font-semibold text-gray-200">
                            <i class="fas fa-envelope text-pink-500 text-lg"></i>
                            <span>Email Oficial</span>
                        </a>
                    </div>
                </div>
<!-- ... existing code -->
    <!-- FLOATING DUAL WHATSAPP WIDGET (BOTTOM RIGHT) -->
    <div class="fixed bottom-6 right-6 z-50 flex flex-col items-end gap-3">
        <!-- Floating Expandable Options -->
        <div id="whatsapp-popup" class="hidden flex-col gap-2 bg-neutral-900 border border-neutral-800 p-3 rounded-2xl shadow-2xl mb-1 animate-fade-in w-72">
            <div class="text-xs font-bold text-white mb-1 flex items-center justify-between border-b border-neutral-800 pb-2">
                <span>Seleccionar Celular de Contacto</span>
                <button onclick="toggleWhatsAppMenu()" class="text-gray-400 hover:text-white"><i class="fas fa-times"></i></button>
            </div>
            
            <a href="https://wa.me/5491144720639?text=Hola!%20Consulta%20por%20WhatsApp%20(Celular%201)" 
               target="_blank" class="flex items-center gap-3 p-2.5 rounded-xl bg-emerald-950/80 border border-emerald-800/80 text-emerald-300 hover:bg-emerald-900 text-xs font-semibold">
                <i class="fab fa-whatsapp text-xl shrink-0"></i>
                <div>
                    <div>Celular 1: +54 9 11 4472-0639</div>
                    <div class="text-[10px] text-emerald-400 font-normal">Línea Liviana / General</div>
                </div>
            </a>

            <a href="https://wa.me/5491122845098?text=Hola!%20Consulta%20por%20WhatsApp%20(Celular%202)" 
               target="_blank" class="flex items-center gap-3 p-2.5 rounded-xl bg-red-950/80 border border-red-800/80 text-red-300 hover:bg-red-900 text-xs font-semibold">
                <i class="fab fa-whatsapp text-xl shrink-0"></i>
                <div>
                    <div>Celular 2: +54 9 11 2284-5098</div>
                    <div class="text-[10px] text-red-400 font-normal">Línea Pesada / Maquinaria</div>
                </div>
            </a>
        </div>

        <!-- MAIN FLOATING BUTTON -->
        <button onclick="toggleWhatsAppMenu()" 
                class="w-14 h-14 rounded-full bg-emerald-500 hover:bg-emerald-400 text-white shadow-2xl flex items-center justify-center text-3xl transition-transform transform hover:scale-110 active:scale-95 border-2 border-white/20">
            <i class="fab fa-whatsapp"></i>
        </button>
    </div>

    <!-- JAVASCRIPT LOGIC -->
    <script>
        // Set dynamic copyright year safely
        const yearSpan = document.getElementById('year-span');
        if (yearSpan) {
            yearSpan.textContent = new Date().getFullYear();
        }

        // Mobile menu toggle
        const mobileMenuBtn = document.getElementById('mobile-menu-btn');
        const mobileMenu = document.getElementById('mobile-menu');

        if (mobileMenuBtn && mobileMenu) {
            mobileMenuBtn.addEventListener('click', () => {
                mobileMenu.classList.toggle('hidden');
            });

            // Close mobile menu when clicking link
            document.querySelectorAll('#mobile-menu a').forEach(link => {
                link.addEventListener('click', () => {
                    mobileMenu.classList.add('hidden');
                });
            });
        }

        // Toggle Floating WhatsApp Menu
        function toggleWhatsAppMenu() {
            const popup = document.getElementById('whatsapp-popup');
            if (popup) {
                popup.classList.toggle('hidden');
                popup.classList.toggle('flex');
            }
        }

        // Switch Tips Tabs
        function switchTipTab(category) {
            // Hide all tab contents
            document.querySelectorAll('.tip-content').forEach(el => {
                el.classList.add('hidden');
            });

            // Reset all tab button styles
            document.querySelectorAll('.tip-tab-btn').forEach(btn => {
                btn.classList.remove('bg-red-600', 'text-white', 'border-red-500');
                btn.classList.add('bg-neutral-900', 'text-gray-300', 'border-neutral-800');
            });

            // Show selected content
            const activeContent = document.getElementById(`tip-tab-${category}`);
            if (activeContent) {
                activeContent.classList.remove('hidden');
            }

            // Highlight selected button
            const activeBtn = document.getElementById(`tab-btn-${category}`);
            if (activeBtn) {
                activeBtn.classList.remove('bg-neutral-900', 'text-gray-300', 'border-neutral-800');
                activeBtn.classList.add('bg-red-600', 'text-white', 'border-red-500');
            }
        }

        // Handle Interactive Calculator form submit -> redirects to pre-filled WhatsApp link
        function handleCalculatorSubmit(event) {
            event.preventDefault();
            const vehicleEl = document.getElementById('calc-vehicle');
            const serviceEl = document.getElementById('calc-service');
            const detailsEl = document.getElementById('calc-details');

            const vehicle = vehicleEl ? vehicleEl.value : '';
            const service = serviceEl ? serviceEl.value : '';
            const details = detailsEl ? detailsEl.value.trim() : '';

            let message = `Hola FH Performance! Quisiera consultar presupuesto para:\n- Vehículo: ${vehicle}\n- Servicio: ${service}`;
            if (details) {
                message += `\n- Detalle/Marca/Serie: ${details}`;
            }

            // Select target WhatsApp line based on vehicle line selected
            const phone = (vehicle && vehicle.includes('Pesada')) ? "5491122845098" : "5491144720639";
            const encodedMessage = encodeURIComponent(message);
            window.open(`https://wa.me/${phone}?text=${encodedMessage}`, '_blank');
        }
    </script>
</body>
</html>
