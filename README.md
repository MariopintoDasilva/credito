<!DOCTYPE html>
<html lang="it" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Credito Personale Rapido - Da Silva Alcide Mario Pinto</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://kit.fontawesome.com/your-font-awesome-kit.js" crossorigin="anonymous"></script>
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        primary: '#5D5CDE',
                        'primary-light': '#7B7AE8',
                        'primary-dark': '#4A49C7'
                    }
                }
            }
        }
    </script>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap');
        * { font-family: 'Inter', sans-serif; }
        
        .gradient-bg {
            background: linear-gradient(135deg, #5D5CDE 0%, #7B7AE8 100%);
        }
        
        .card-hover {
            transition: all 0.3s ease;
        }
        
        .card-hover:hover {
            transform: translateY(-5px);
            box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.1), 0 10px 10px -5px rgba(0, 0, 0, 0.04);
        }
        
        .animate-float {
            animation: float 3s ease-in-out infinite;
        }
        
        @keyframes float {
            0%, 100% { transform: translateY(0px); }
            50% { transform: translateY(-20px); }
        }
        
        .modal-overlay {
            backdrop-filter: blur(10px);
        }
        
        /* Dark mode styles */
        .dark .gradient-bg {
            background: linear-gradient(135deg, #4A49C7 0%, #5D5CDE 100%);
        }
    </style>
</head>
<body class="bg-white dark:bg-gray-900 text-gray-900 dark:text-white transition-colors duration-300">

    <!-- Navigation -->
    <nav class="fixed w-full top-0 z-50 bg-white/90 dark:bg-gray-900/90 backdrop-blur-md border-b border-gray-200 dark:border-gray-700">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center h-16">
                <div class="flex items-center space-x-3">
                    <div class="w-10 h-10 bg-primary rounded-lg flex items-center justify-center">
                        <i class="fas fa-euro-sign text-white text-lg"></i>
                    </div>
                    <h1 class="text-xl font-bold text-primary">Da Silva Crediti</h1>
                </div>
                <div class="hidden md:flex space-x-8">
                    <a href="#home" class="text-gray-700 dark:text-gray-300 hover:text-primary transition-colors">Home</a>
                    <a href="#servizi" class="text-gray-700 dark:text-gray-300 hover:text-primary transition-colors">Servizi</a>
                    <a href="#calcolo" class="text-gray-700 dark:text-gray-300 hover:text-primary transition-colors">Calcolo Prestito</a>
                    <a href="#contatti" class="text-gray-700 dark:text-gray-300 hover:text-primary transition-colors">Contatti</a>
                    <button onclick="openMessageCenter()" class="bg-primary text-white px-4 py-2 rounded-lg hover:bg-primary-dark transition-colors">
                        <i class="fas fa-comments mr-2"></i>Messaggi
                    </button>
                </div>
                <button onclick="toggleMobileMenu()" class="md:hidden">
                    <i class="fas fa-bars text-2xl"></i>
                </button>
            </div>
        </div>
        
        <!-- Mobile Menu -->
        <div id="mobileMenu" class="hidden md:hidden bg-white dark:bg-gray-900 border-t border-gray-200 dark:border-gray-700">
            <div class="px-4 pt-2 pb-3 space-y-1">
                <a href="#home" class="block px-3 py-2 text-gray-700 dark:text-gray-300 hover:text-primary">Home</a>
                <a href="#servizi" class="block px-3 py-2 text-gray-700 dark:text-gray-300 hover:text-primary">Servizi</a>
                <a href="#calcolo" class="block px-3 py-2 text-gray-700 dark:text-gray-300 hover:text-primary">Calcolo Prestito</a>
                <a href="#contatti" class="block px-3 py-2 text-gray-700 dark:text-gray-300 hover:text-primary">Contatti</a>
                <button onclick="openMessageCenter()" class="block w-full text-left px-3 py-2 text-primary">
                    <i class="fas fa-comments mr-2"></i>Centro Messaggi
                </button>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section id="home" class="pt-20 pb-16 gradient-bg relative overflow-hidden">
        <div class="absolute inset-0 bg-black/10"></div>
        <div class="relative max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center text-white">
                <div class="animate-float mb-8">
                    <div class="w-24 h-24 bg-white/20 rounded-full flex items-center justify-center mx-auto mb-6">
                        <i class="fas fa-hand-holding-usd text-4xl"></i>
                    </div>
                </div>
                <h1 class="text-4xl md:text-6xl font-bold mb-6">
                    Credito Personale Rapido
                </h1>
                <h2 class="text-2xl md:text-3xl font-semibold mb-4">
                    Da Silva Alcide Mario Pinto
                </h2>
                <p class="text-xl md:text-2xl mb-8 text-white/90">
                    Prestiti personalizzati con tasso fisso del <span class="font-bold text-yellow-300">2%</span>
                </p>
                <div class="flex flex-col sm:flex-row gap-4 justify-center">
                    <button onclick="openLoanForm()" class="bg-white text-primary px-8 py-4 rounded-lg font-semibold text-lg hover:bg-gray-100 transition-colors">
                        <i class="fas fa-calculator mr-2"></i>Richiedi Prestito
                    </button>
                    <a href="https://wa.me/message/IBU2WZ7O6M72C1" target="_blank" class="bg-green-500 text-white px-8 py-4 rounded-lg font-semibold text-lg hover:bg-green-600 transition-colors">
                        <i class="fab fa-whatsapp mr-2"></i>WhatsApp
                    </a>
                </div>
            </div>
        </div>
    </section>

    <!-- Servizi Section -->
    <section id="servizi" class="py-16 bg-gray-50 dark:bg-gray-800">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-12">
                <h2 class="text-3xl md:text-4xl font-bold mb-4">I Nostri Servizi</h2>
                <p class="text-xl text-gray-600 dark:text-gray-300">Soluzioni finanziarie su misura per le tue esigenze</p>
            </div>
            
            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Prestito Personale -->
                <div class="bg-white dark:bg-gray-700 p-8 rounded-xl shadow-lg card-hover">
                    <div class="w-16 h-16 bg-primary/10 rounded-lg flex items-center justify-center mb-6">
                        <i class="fas fa-user-check text-primary text-2xl"></i>
                    </div>
                    <h3 class="text-2xl font-semibold mb-4">Prestito Personale</h3>
                    <p class="text-gray-600 dark:text-gray-300 mb-6">Prestiti fino a €50,000 con tasso fisso del 2% e approvazione rapida in 24 ore.</p>
                    <ul class="space-y-2 text-sm text-gray-600 dark:text-gray-300">
                        <li><i class="fas fa-check text-green-500 mr-2"></i>Tasso fisso 2%</li>
                        <li><i class="fas fa-check text-green-500 mr-2"></i>Durata fino a 10 anni</li>
                        <li><i class="fas fa-check text-green-500 mr-2"></i>Nessuna commissione nascosta</li>
                    </ul>
                </div>

                <!-- Prestito Casa -->
                <div class="bg-white dark:bg-gray-700 p-8 rounded-xl shadow-lg card-hover">
                    <div class="w-16 h-16 bg-primary/10 rounded-lg flex items-center justify-center mb-6">
                        <i class="fas fa-home text-primary text-2xl"></i>
                    </div>
                    <h3 class="text-2xl font-semibold mb-4">Prestito Casa</h3>
                    <p class="text-gray-600 dark:text-gray-300 mb-6">Finanziamenti per l'acquisto, ristrutturazione o surroga della tua casa.</p>
                    <ul class="space-y-2 text-sm text-gray-600 dark:text-gray-300">
                        <li><i class="fas fa-check text-green-500 mr-2"></i>Fino al 100% del valore</li>
                        <li><i class="fas fa-check text-green-500 mr-2"></i>Durata fino a 30 anni</li>
                        <li><i class="fas fa-check text-green-500 mr-2"></i>Valutazione gratuita</li>
                    </ul>
                </div>

                <!-- Prestito Aziendale -->
                <div class="bg-white dark:bg-gray-700 p-8 rounded-xl shadow-lg card-hover">
                    <div class="w-16 h-16 bg-primary/10 rounded-lg flex items-center justify-center mb-6">
                        <i class="fas fa-briefcase text-primary text-2xl"></i>
                    </div>
                    <h3 class="text-2xl font-semibold mb-4">Prestito Aziendale</h3>
                    <p class="text-gray-600 dark:text-gray-300 mb-6">Finanziamenti per imprese e liberi professionisti per crescere il tuo business.</p>
                    <ul class="space-y-2 text-sm text-gray-600 dark:text-gray-300">
                        <li><i class="fas fa-check text-green-500 mr-2"></i>Fino a €500,000</li>
                        <li><i class="fas fa-check text-green-500 mr-2"></i>Tempi di risposta rapidi</li>
                        <li><i class="fas fa-check text-green-500 mr-2"></i>Consulenza personalizzata</li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <!-- Calcolatore Prestito -->
    <section id="calcolo" class="py-16 bg-white dark:bg-gray-900">
        <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-12">
                <h2 class="text-3xl md:text-4xl font-bold mb-4">Calcola il Tuo Prestito</h2>
                <p class="text-xl text-gray-600 dark:text-gray-300">Scopri subito l'importo della tua rata mensile</p>
            </div>
            
            <div class="bg-gray-50 dark:bg-gray-800 p-8 rounded-xl shadow-lg">
                <div class="grid md:grid-cols-2 gap-8">
                    <div class="space-y-6">
                        <div>
                            <label class="block text-sm font-semibold mb-2">Importo del prestito (€)</label>
                            <input type="range" id="loanAmount" min="1000" max="50000" value="10000" 
                                   class="w-full h-2 bg-gray-200 dark:bg-gray-600 rounded-lg appearance-none cursor-pointer">
                            <div class="flex justify-between text-sm text-gray-600 dark:text-gray-400 mt-1">
                                <span>€1,000</span>
                                <span id="amountValue" class="font-semibold text-primary">€10,000</span>
                                <span>€50,000</span>
                            </div>
                        </div>
                        
                        <div>
                            <label class="block text-sm font-semibold mb-2">Durata (anni)</label>
                            <input type="range" id="loanDuration" min="1" max="10" value="5" 
                                   class="w-full h-2 bg-gray-200 dark:bg-gray-600 rounded-lg appearance-none cursor-pointer">
                            <div class="flex justify-between text-sm text-gray-600 dark:text-gray-400 mt-1">
                                <span>1 anno</span>
                                <span id="durationValue" class="font-semibold text-primary">5 anni</span>
                                <span>10 anni</span>
                            </div>
                        </div>
                        
                        <div class="bg-primary/10 p-4 rounded-lg">
                            <div class="text-sm text-gray-600 dark:text-gray-400 mb-1">Tasso di interesse</div>
                            <div class="text-2xl font-bold text-primary">2% fisso</div>
                        </div>
                    </div>
                    
                    <div class="space-y-6">
                        <div class="bg-white dark:bg-gray-700 p-6 rounded-lg shadow">
                            <h3 class="text-lg font-semibold mb-4">Riepilogo del prestito</h3>
                            <div class="space-y-3">
                                <div class="flex justify-between">
                                    <span>Importo richiesto:</span>
                                    <span class="font-semibold" id="summaryAmount">€10,000</span>
                                </div>
                                <div class="flex justify-between">
                                    <span>Durata:</span>
                                    <span class="font-semibold" id="summaryDuration">5 anni</span>
                                </div>
                                <div class="flex justify-between">
                                    <span>Tasso di interesse:</span>
                                    <span class="font-semibold text-primary">2%</span>
                                </div>
                                <hr class="dark:border-gray-600">
                                <div class="flex justify-between text-lg">
                                    <span class="font-semibold">Rata mensile:</span>
                                    <span class="font-bold text-primary text-xl" id="monthlyPayment">€175</span>
                                </div>
                                <div class="flex justify-between text-sm text-gray-600 dark:text-gray-400">
                                    <span>Importo totale:</span>
                                    <span id="totalAmount">€10,500</span>
                                </div>
                            </div>
                        </div>
                        
                        <button onclick="openLoanForm()" class="w-full bg-primary text-white py-3 rounded-lg font-semibold hover:bg-primary-dark transition-colors">
                            <i class="fas fa-paper-plane mr-2"></i>Richiedi Questo Prestito
                        </button>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contatti Section -->
    <section id="contatti" class="py-16 bg-gray-50 dark:bg-gray-800">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-12">
                <h2 class="text-3xl md:text-4xl font-bold mb-4">Contattaci</h2>
                <p class="text-xl text-gray-600 dark:text-gray-300">Siamo qui per aiutarti con le tue esigenze finanziarie</p>
            </div>
            
            <div class="grid lg:grid-cols-2 gap-12">
                <!-- Info Contatti -->
                <div class="space-y-8">
                    <div class="bg-white dark:bg-gray-700 p-6 rounded-xl shadow-lg">
                        <h3 class="text-2xl font-semibold mb-6">Da Silva Alcide Mario Pinto</h3>
                        <div class="space-y-4">
                            <div class="flex items-center space-x-3">
                                <div class="w-10 h-10 bg-green-100 dark:bg-green-900 rounded-lg flex items-center justify-center">
                                    <i class="fab fa-whatsapp text-green-600 dark:text-green-400"></i>
                                </div>
                                <div>
                                    <div class="font-semibold">WhatsApp</div>
                                    <a href="https://wa.me/message/IBU2WZ7O6M72C1" class="text-green-600 dark:text-green-400 hover:underline">
                                        Chatta con noi
                                    </a>
                                </div>
                            </div>
                            
                            <div class="flex items-center space-x-3">
                                <div class="w-10 h-10 bg-blue-100 dark:bg-blue-900 rounded-lg flex items-center justify-center">
                                    <i class="fas fa-envelope text-blue-600 dark:text-blue-400"></i>
                                </div>
                                <div>
                                    <div class="font-semibold">Email</div>
                                    <a href="mailto:josepintodasilva32@gmail.com" class="text-blue-600 dark:text-blue-400 hover:underline">
                                        josepintodasilva32@gmail.com
                                    </a>
                                </div>
                            </div>
                            
                            <div class="flex items-center space-x-3">
                                <div class="w-10 h-10 bg-purple-100 dark:bg-purple-900 rounded-lg flex items-center justify-center">
                                    <i class="fas fa-clock text-purple-600 dark:text-purple-400"></i>
                                </div>
                                <div>
                                    <div class="font-semibold">Orari di servizio</div>
                                    <div class="text-gray-600 dark:text-gray-300">Lun-Ven: 9:00-18:00</div>
                                </div>
                            </div>
                        </div>
                    </div>
                    
                    <div class="bg-primary/10 p-6 rounded-xl">
                        <h4 class="font-semibold text-primary mb-3">Perché scegliere Da Silva Crediti?</h4>
                        <ul class="space-y-2 text-sm">
                            <li><i class="fas fa-star text-yellow-500 mr-2"></i>Oltre 10 anni di esperienza nel settore</li>
                            <li><i class="fas fa-star text-yellow-500 mr-2"></i>Tasso fisso del 2% garantito</li>
                            <li><i class="fas fa-star text-yellow-500 mr-2"></i>Approvazione rapida in 24 ore</li>
                            <li><i class="fas fa-star text-yellow-500 mr-2"></i>Consulenza personalizzata gratuita</li>
                            <li><i class="fas fa-star text-yellow-500 mr-2"></i>Massima trasparenza e sicurezza</li>
                        </ul>
                    </div>
                </div>
                
                <!-- Form Contatti -->
                <div class="bg-white dark:bg-gray-700 p-8 rounded-xl shadow-lg">
                    <h3 class="text-2xl font-semibold mb-6">Invia un Messaggio</h3>
                    <form id="contactForm" class="space-y-6">
                        <div class="grid md:grid-cols-2 gap-4">
                            <div>
                                <label class="block text-sm font-semibold mb-2">Nome*</label>
                                <input type="text" id="contactName" required 
                                       class="w-full px-4 py-3 border border-gray-300 dark:border-gray-600 rounded-lg focus:ring-2 focus:ring-primary focus:border-transparent dark:bg-gray-600 dark:text-white text-base">
                            </div>
                            <div>
                                <label class="block text-sm font-semibold mb-2">Cognome*</label>
                                <input type="text" id="contactSurname" required 
                                       class="w-full px-4 py-3 border border-gray-300 dark:border-gray-600 rounded-lg focus:ring-2 focus:ring-primary focus:border-transparent dark:bg-gray-600 dark:text-white text-base">
                            </div>
                        </div>
                        
                        <div>
                            <label class="block text-sm font-semibold mb-2">Email*</label>
                            <input type="email" id="contactEmail" required 
                                   class="w-full px-4 py-3 border border-gray-300 dark:border-gray-600 rounded-lg focus:ring-2 focus:ring-primary focus:border-transparent dark:bg-gray-600 dark:text-white text-base">
                        </div>
                        
                        <div>
                            <label class="block text-sm font-semibold mb-2">Telefono</label>
                            <input type="tel" id="contactPhone" 
                                   class="w-full px-4 py-3 border border-gray-300 dark:border-gray-600 rounded-lg focus:ring-2 focus:ring-primary focus:border-transparent dark:bg-gray-600 dark:text-white text-base">
                        </div>
                        
                        <div>
                            <label class="block text-sm font-semibold mb-2">Tipo di prestito</label>
                            <select id="contactLoanType" 
                                    class="w-full px-4 py-3 border border-gray-300 dark:border-gray-600 rounded-lg focus:ring-2 focus:ring-primary focus:border-transparent dark:bg-gray-600 dark:text-white text-base">
                                <option value="">Seleziona...</option>
                                <option value="personale">Prestito Personale</option>
                                <option value="casa">Prestito Casa</option>
                                <option value="aziendale">Prestito Aziendale</option>
                                <option value="altro">Altro</option>
                            </select>
                        </div>
                        
                        <div>
                            <label class="block text-sm font-semibold mb-2">Messaggio*</label>
                            <textarea id="contactMessage" rows="4" required 
                                      class="w-full px-4 py-3 border border-gray-300 dark:border-gray-600 rounded-lg focus:ring-2 focus:ring-primary focus:border-transparent dark:bg-gray-600 dark:text-white text-base"
                                      placeholder="Descrivi le tue esigenze..."></textarea>
                        </div>
                        
                        <div class="flex flex-col sm:flex-row gap-3">
                            <button type="submit" class="flex-1 bg-primary text-white py-3 rounded-lg font-semibold hover:bg-primary-dark transition-colors">
                                <i class="fas fa-paper-plane mr-2"></i>Invia Messaggio
                            </button>
                            <a href="https://wa.me/message/IBU2WZ7O6M72C1" target="_blank" 
                               class="flex-1 bg-green-500 text-white py-3 rounded-lg font-semibold hover:bg-green-600 transition-colors text-center">
                                <i class="fab fa-whatsapp mr-2"></i>WhatsApp
                            </a>
                        </div>
                    </form>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-900 text-white py-12">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid md:grid-cols-3 gap-8">
                <div>
                    <div class="flex items-center space-x-3 mb-6">
                        <div class="w-10 h-10 bg-primary rounded-lg flex items-center justify-center">
                            <i class="fas fa-euro-sign text-white"></i>
                        </div>
                        <h3 class="text-xl font-bold">Da Silva Crediti</h3>
                    </div>
                    <p class="text-gray-400 mb-4">
                        Credito Personale Rapido di Da Silva Alcide Mario Pinto. 
                        La tua soluzione finanziaria di fiducia con tasso fisso del 2%.
                    </p>
                    <div class="flex space-x-4">
                        <a href="https://wa.me/message/IBU2WZ7O6M72C1" target="_blank" 
                           class="w-10 h-10 bg-green-500 rounded-lg flex items-center justify-center hover:bg-green-600 transition-colors">
                            <i class="fab fa-whatsapp"></i>
                        </a>
                        <a href="mailto:josepintodasilva32@gmail.com" 
                           class="w-10 h-10 bg-blue-500 rounded-lg flex items-center justify-center hover:bg-blue-600 transition-colors">
                            <i class="fas fa-envelope"></i>
                        </a>
                    </div>
                </div>
                
                <div>
                    <h4 class="text-lg font-semibold mb-4">Servizi</h4>
                    <ul class="space-y-2 text-gray-400">
                        <li><a href="#servizi" class="hover:text-white transition-colors">Prestito Personale</a></li>
                        <li><a href="#servizi" class="hover:text-white transition-colors">Prestito Casa</a></li>
                        <li><a href="#servizi" class="hover:text-white transition-colors">Prestito Aziendale</a></li>
                        <li><a href="#calcolo" class="hover:text-white transition-colors">Calcola Prestito</a></li>
                    </ul>
                </div>
                
                <div>
                    <h4 class="text-lg font-semibold mb-4">Contatti</h4>
                    <ul class="space-y-2 text-gray-400">
                        <li>
                            <i class="fab fa-whatsapp mr-2"></i>
                            <a href="https://wa.me/message/IBU2WZ7O6M72C1" class="hover:text-white transition-colors">WhatsApp</a>
                        </li>
                        <li>
                            <i class="fas fa-envelope mr-2"></i>
                            <a href="mailto:josepintodasilva32@gmail.com" class="hover:text-white transition-colors">Email</a>
                        </li>
                        <li>
                            <i class="fas fa-clock mr-2"></i>
                            Lun-Ven: 9:00-18:00
                        </li>
                    </ul>
                </div>
            </div>
            
            <div class="border-t border-gray-800 pt-8 mt-8 text-center text-gray-400">
                <p>&copy; 2025 Da Silva Alcide Mario Pinto - Credito Personale Rapido. Tutti i diritti riservati.</p>
            </div>
        </div>
    </footer>

    <!-- Modal Richiesta Prestito -->
    <div id="loanModal" class="hidden fixed inset-0 bg-black/50 modal-overlay z-50 flex items-center justify-center p-4">
        <div class="bg-white dark:bg-gray-800 rounded-xl shadow-2xl w-full max-w-2xl max-h-[90vh] overflow-y-auto">
            <div class="p-6 border-b border-gray-200 dark:border-gray-700">
                <div class="flex justify-between items-center">
                    <h3 class="text-2xl font-bold">Richiesta Prestito</h3>
                    <button onclick="closeLoanForm()" class="text-gray-500 hover:text-gray-700 dark:text-gray-400 dark:hover:text-gray-200">
                        <i class="fas fa-times text-2xl"></i>
                    </button>
                </div>
            </div>
            
            <form id="loanForm" class="p-6 space-y-6">
                <div class="grid md:grid-cols-2 gap-4">
                    <div>
                        <label class="block text-sm font-semibold mb-2">Nome*</label>
                        <input type="text" id="loanName" required 
                               class="w-full px-4 py-3 border border-gray-300 dark:border-gray-600 rounded-lg focus:ring-2 focus:ring-primary focus:border-transparent dark:bg-gray-600 dark:text-white text-base">
                    </div>
                    <div>
                        <label class="block text-sm font-semibold mb-2">Cognome*</label>
                        <input type="text" id="loanSurname" required 
                               class="w-full px-4 py-3 border border-gray-300 dark:border-gray-600 rounded-lg focus:ring-2 focus:ring-primary focus:border-transparent dark:bg-gray-600 dark:text-white text-base">
                    </div>
                </div>
                
                <div class="grid md:grid-cols-2 gap-4">
                    <div>
                        <label class="block text-sm font-semibold mb-2">Email*</label>
                        <input type="email" id="loanEmail" required 
                               class="w-full px-4 py-3 border border-gray-300 dark:border-gray-600 rounded-lg focus:ring-2 focus:ring-primary focus:border-transparent dark:bg-gray-600 dark:text-white text-base">
                    </div>
                    <div>
                        <label class="block text-sm font-semibold mb-2">Telefono*</label>
                        <input type="tel" id="loanPhone" required 
                               class="w-full px-4 py-3 border border-gray-300 dark:border-gray-600 rounded-lg focus:ring-2 focus:ring-primary focus:border-transparent dark:bg-gray-600 dark:text-white text-base">
                    </div>
                </div>
                
                <div class="grid md:grid-cols-2 gap-4">
                    <div>
                        <label class="block text-sm font-semibold mb-2">Importo richiesto (€)*</label>
                        <input type="number" id="loanRequestAmount" min="1000" max="50000" required 
                               class="w-full px-4 py-3 border border-gray-300 dark:border-gray-600 rounded-lg focus:ring-2 focus:ring-primary focus:border-transparent dark:bg-gray-600 dark:text-white text-base">
                    </div>
                    <div>
                        <label class="block text-sm font-semibold mb-2">Durata (anni)*</label>
                        <select id="loanRequestDuration" required 
                                class="w-full px-4 py-3 border border-gray-300 dark:border-gray-600 rounded-lg focus:ring-2 focus:ring-primary focus:border-transparent dark:bg-gray-600 dark:text-white text-base">
                            <option value="">Seleziona...</option>
                            <option value="1">1 anno</option>
                            <option value="2">2 anni</option>
                            <option value="3">3 anni</option>
                            <option value="4">4 anni</option>
                            <option value="5">5 anni</option>
                            <option value="6">6 anni</option>
                            <option value="7">7 anni</option>
                            <option value="8">8 anni</option>
                            <option value="9">9 anni</option>
                            <option value="10">10 anni</option>
                        </select>
                    </div>
                </div>
                
                <div>
                    <label class="block text-sm font-semibold mb-2">Tipo di prestito*</label>
                    <select id="loanType" required 
                            class="w-full px-4 py-3 border border-gray-300 dark:border-gray-600 rounded-lg focus:ring-2 focus:ring-primary focus:border-transparent dark:bg-gray-600 dark:text-white text-base">
                        <option value="">Seleziona...</option>
                        <option value="personale">Prestito Personale</option>
                        <option value="casa">Prestito Casa</option>
                        <option value="aziendale">Prestito Aziendale</option>
                    </select>
                </div>
                
                <div>
                    <label class="block text-sm font-semibold mb-2">Reddito mensile (€)*</label>
                    <input type="number" id="loanIncome" min="500" required 
                           class="w-full px-4 py-3 border border-gray-300 dark:border-gray-600 rounded-lg focus:ring-2 focus:ring-primary focus:border-transparent dark:bg-gray-600 dark:text-white text-base">
                </div>
                
                <div>
                    <label class="block text-sm font-semibold mb-2">Note aggiuntive</label>
                    <textarea id="loanNotes" rows="3" 
                              class="w-full px-4 py-3 border border-gray-300 dark:border-gray-600 rounded-lg focus:ring-2 focus:ring-primary focus:border-transparent dark:bg-gray-600 dark:text-white text-base"
                              placeholder="Qualsiasi informazione aggiuntiva..."></textarea>
                </div>
                
                <div class="flex flex-col sm:flex-row gap-3">
                    <button type="submit" class="flex-1 bg-primary text-white py-3 rounded-lg font-semibold hover:bg-primary-dark transition-colors">
                        <i class="fas fa-paper-plane mr-2"></i>Invia Richiesta
                    </button>
                    <button type="button" onclick="closeLoanForm()" class="flex-1 bg-gray-500 text-white py-3 rounded-lg font-semibold hover:bg-gray-600 transition-colors">
                        Annulla
                    </button>
                </div>
            </form>
        </div>
    </div>

    <!-- Centro Messaggi Modal -->
    <div id="messageCenterModal" class="hidden fixed inset-0 bg-black/50 modal-overlay z-50 flex items-center justify-center p-4">
        <div class="bg-white dark:bg-gray-800 rounded-xl shadow-2xl w-full max-w-4xl h-[80vh] flex flex-col">
            <div class="p-6 border-b border-gray-200 dark:border-gray-700">
                <div class="flex justify-between items-center">
                    <h3 class="text-2xl font-bold">Centro Messaggi</h3>
                    <button onclick="closeMessageCenter()" class="text-gray-500 hover:text-gray-700 dark:text-gray-400 dark:hover:text-gray-200">
                        <i class="fas fa-times text-2xl"></i>
                    </button>
                </div>
            </div>
            
            <div class="flex-1 flex">
                <!-- Lista Conversazioni -->
                <div class="w-1/3 border-r border-gray-200 dark:border-gray-700 p-4">
                    <h4 class="font-semibold mb-4">Conversazioni</h4>
                    <div id="conversationList" class="space-y-2">
                        <!-- Le conversazioni verranno aggiunte dinamicamente -->
                    </div>
                    <button onclick="startNewConversation()" class="w-full mt-4 bg-primary text-white py-2 rounded-lg hover:bg-primary-dark transition-colors">
                        <i class="fas fa-plus mr-2"></i>Nuova Chat
                    </button>
                </div>
                
                <!-- Area Chat -->
                <div class="flex-1 flex flex-col">
                    <div id="chatArea" class="flex-1 p-4 overflow-y-auto bg-gray-50 dark:bg-gray-900">
                        <div class="text-center text-gray-500 dark:text-gray-400 mt-8">
                            <i class="fas fa-comments text-4xl mb-4"></i>
                            <p>Seleziona una conversazione o inizia una nuova chat</p>
                        </div>
                    </div>
                    
                    <div id="chatInput" class="hidden p-4 border-t border-gray-200 dark:border-gray-700">
                        <div class="flex space-x-2">
                            <input type="text" id="messageInput" placeholder="Scrivi un messaggio..." 
                                   class="flex-1 px-4 py-2 border border-gray-300 dark:border-gray-600 rounded-lg focus:ring-2 focus:ring-primary focus:border-transparent dark:bg-gray-600 dark:text-white text-base">
                            <button onclick="sendMessage()" class="bg-primary text-white px-6 py-2 rounded-lg hover:bg-primary-dark transition-colors">
                                <i class="fas fa-paper-plane"></i>
                            </button>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <script>
        // Dark mode setup
        if (window.matchMedia && window.matchMedia('(prefers-color-scheme: dark)').matches) {
            document.documentElement.classList.add('dark');
        }
        window.matchMedia('(prefers-color-scheme: dark)').addEventListener('change', event => {
            if (event.matches) {
                document.documentElement.classList.add('dark');
            } else {
                document.documentElement.classList.remove('dark');
            }
        });

        // Mobile menu toggle
        function toggleMobileMenu() {
            const menu = document.getElementById('mobileMenu');
            menu.classList.toggle('hidden');
        }

        // Calcolatore prestito
        const loanAmountSlider = document.getElementById('loanAmount');
        const loanDurationSlider = document.getElementById('loanDuration');
        const amountValue = document.getElementById('amountValue');
        const durationValue = document.getElementById('durationValue');
        const summaryAmount = document.getElementById('summaryAmount');
        const summaryDuration = document.getElementById('summaryDuration');
        const monthlyPayment = document.getElementById('monthlyPayment');
        const totalAmount = document.getElementById('totalAmount');

        function calculateLoan() {
            const amount = parseInt(loanAmountSlider.value);
            const duration = parseInt(loanDurationSlider.value);
            const rate = 0.02; // 2%
            
            // Formula rata mensile: M = P * (r(1+r)^n) / ((1+r)^n - 1)
            const monthlyRate = rate / 12;
            const numPayments = duration * 12;
            const monthly = amount * (monthlyRate * Math.pow(1 + monthlyRate, numPayments)) / (Math.pow(1 + monthlyRate, numPayments) - 1);
            const total = monthly * numPayments;
            
            amountValue.textContent = `€${amount.toLocaleString()}`;
            durationValue.textContent = `${duration} anni`;
            summaryAmount.textContent = `€${amount.toLocaleString()}`;
            summaryDuration.textContent = `${duration} anni`;
            monthlyPayment.textContent = `€${Math.round(monthly)}`;
            totalAmount.textContent = `€${Math.round(total).toLocaleString()}`;
        }

        loanAmountSlider.addEventListener('input', calculateLoan);
        loanDurationSlider.addEventListener('input', calculateLoan);

        // Inizializza il calcolo
        calculateLoan();

        // Modal richiesta prestito
        function openLoanForm() {
            document.getElementById('loanModal').classList.remove('hidden');
            document.body.style.overflow = 'hidden';
            
            // Pre-compila con i valori del calcolatore
            document.getElementById('loanRequestAmount').value = loanAmountSlider.value;
            document.getElementById('loanRequestDuration').value = loanDurationSlider.value;
        }

        function closeLoanForm() {
            document.getElementById('loanModal').classList.add('hidden');
            document.body.style.overflow = 'auto';
        }

        // Gestione form richiesta prestito
        document.getElementById('loanForm').addEventListener('submit', function(e) {
            e.preventDefault();
            
            const formData = {
                nome: document.getElementById('loanName').value,
                cognome: document.getElementById('loanSurname').value,
                email: document.getElementById('loanEmail').value,
                telefono: document.getElementById('loanPhone').value,
                importo: document.getElementById('loanRequestAmount').value,
                durata: document.getElementById('loanRequestDuration').value,
                tipo: document.getElementById('loanType').value,
                reddito: document.getElementById('loanIncome').value,
                note: document.getElementById('loanNotes').value
            };
            
            // Messaggio per WhatsApp
            const whatsappMessage = `🏦 *RICHIESTA PRESTITO*

👤 *Richiedente:* ${formData.nome} ${formData.cognome}
📧 *Email:* ${formData.email}
📱 *Telefono:* ${formData.telefono}

💰 *Dettagli Prestito:*
• Importo: €${parseInt(formData.importo).toLocaleString()}
• Durata: ${formData.durata} anni
• Tipo: ${formData.tipo}
• Reddito mensile: €${parseInt(formData.reddito).toLocaleString()}

📝 *Note:* ${formData.note || 'Nessuna nota aggiuntiva'}

---
Inviato dal sito Da Silva Crediti`;

            // Messaggio per Email
            const emailSubject = `Richiesta Prestito - ${formData.nome} ${formData.cognome}`;
            const emailBody = `Gentile Da Silva,

ho ricevuto una nuova richiesta di prestito dal sito web:

DATI RICHIEDENTE:
Nome: ${formData.nome}
Cognome: ${formData.cognome}
Email: ${formData.email}
Telefono: ${formData.telefono}

DETTAGLI PRESTITO:
Importo richiesto: €${parseInt(formData.importo).toLocaleString()}
Durata: ${formData.durata} anni
Tipo di prestito: ${formData.tipo}
Reddito mensile: €${parseInt(formData.reddito).toLocaleString()}

Note aggiuntive: ${formData.note || 'Nessuna nota aggiuntiva'}

La richiesta è stata inviata tramite il modulo del sito web.

Cordiali saluti`;

            // Apri WhatsApp e Email
            const whatsappUrl = `https://wa.me/message/IBU2WZ7O6M72C1?text=${encodeURIComponent(whatsappMessage)}`;
            const emailUrl = `mailto:josepintodasilva32@gmail.com?subject=${encodeURIComponent(emailSubject)}&body=${encodeURIComponent(emailBody)}`;
            
            window.open(whatsappUrl, '_blank');
            setTimeout(() => {
                window.open(emailUrl, '_blank');
            }, 500);
            
            // Mostra messaggio di successo
            showSuccessMessage('Richiesta inviata con successo! Ti contatteremo presto.');
            closeLoanForm();
            document.getElementById('loanForm').reset();
        });

        // Gestione form contatti
        document.getElementById('contactForm').addEventListener('submit', function(e) {
            e.preventDefault();
            
            const formData = {
                nome: document.getElementById('contactName').value,
                cognome: document.getElementById('contactSurname').value,
                email: document.getElementById('contactEmail').value,
                telefono: document.getElementById('contactPhone').value,
                tipoCredito: document.getElementById('contactLoanType').value,
                messaggio: document.getElementById('contactMessage').value
            };
            
            // Messaggio per WhatsApp
            const whatsappMessage = `📨 *NUOVO MESSAGGIO*

👤 *Da:* ${formData.nome} ${formData.cognome}
📧 *Email:* ${formData.email}
📱 *Telefono:* ${formData.telefono}
🏦 *Interesse:* ${formData.tipoCredito || 'Non specificato'}

💬 *Messaggio:*
${formData.messaggio}

---
Inviato dal sito Da Silva Crediti`;

            // Messaggio per Email
            const emailSubject = `Nuovo messaggio dal sito - ${formData.nome} ${formData.cognome}`;
            const emailBody = `Gentile Da Silva,

hai ricevuto un nuovo messaggio dal sito web:

DATI MITTENTE:
Nome: ${formData.nome}
Cognome: ${formData.cognome}
Email: ${formData.email}
Telefono: ${formData.telefono}
Tipo di prestito di interesse: ${formData.tipoCredito || 'Non specificato'}

MESSAGGIO:
${formData.messaggio}

Cordiali saluti`;

            // Apri WhatsApp e Email
            const whatsappUrl = `https://wa.me/message/IBU2WZ7O6M72C1?text=${encodeURIComponent(whatsappMessage)}`;
            const emailUrl = `mailto:josepintodasilva32@gmail.com?subject=${encodeURIComponent(emailSubject)}&body=${encodeURIComponent(emailBody)}`;
            
            window.open(whatsappUrl, '_blank');
            setTimeout(() => {
                window.open(emailUrl, '_blank');
            }, 500);
            
            // Mostra messaggio di successo
            showSuccessMessage('Messaggio inviato con successo! Ti risponderemo presto.');
            document.getElementById('contactForm').reset();
        });

        // Centro Messaggi
        let conversations = [];
        let currentConversationId = null;

        function openMessageCenter() {
            document.getElementById('messageCenterModal').classList.remove('hidden');
            document.body.style.overflow = 'hidden';
            loadConversations();
        }

        function closeMessageCenter() {
            document.getElementById('messageCenterModal').classList.add('hidden');
            document.body.style.overflow = 'auto';
        }

        function loadConversations() {
            const conversationList = document.getElementById('conversationList');
            conversationList.innerHTML = '';
            
            if (conversations.length === 0) {
                conversationList.innerHTML = '<p class="text-gray-500 dark:text-gray-400 text-sm">Nessuna conversazione</p>';
                return;
            }
            
            conversations.forEach((conv, index) => {
                const div = document.createElement('div');
                div.className = `p-3 rounded-lg cursor-pointer hover:bg-gray-100 dark:hover:bg-gray-700 ${currentConversationId === index ? 'bg-primary text-white' : 'bg-gray-100 dark:bg-gray-700'}`;
                div.innerHTML = `
                    <div class="font-semibold text-sm">${conv.title}</div>
                    <div class="text-xs opacity-75">${conv.messages.length} messaggi</div>
                `;
                div.onclick = () => selectConversation(index);
                conversationList.appendChild(div);
            });
        }

        function startNewConversation() {
            const title = `Chat ${conversations.length + 1}`;
            const newConversation = {
                title: title,
                messages: []
            };
            conversations.push(newConversation);
            loadConversations();
            selectConversation(conversations.length - 1);
        }

        function selectConversation(id) {
            currentConversationId = id;
            loadConversations();
            displayChat();
            document.getElementById('chatInput').classList.remove('hidden');
        }

        function displayChat() {
            const chatArea = document.getElementById('chatArea');
            if (currentConversationId === null) return;
            
            const conversation = conversations[currentConversationId];
            chatArea.innerHTML = '';
            
            if (conversation.messages.length === 0) {
                chatArea.innerHTML = `
                    <div class="text-center text-gray-500 dark:text-gray-400 mt-8">
                        <i class="fas fa-comment text-4xl mb-4"></i>
                        <p>Inizia la conversazione scrivendo un messaggio</p>
                    </div>
                `;
                return;
            }
            
            conversation.messages.forEach(message => {
                const messageDiv = document.createElement('div');
                messageDiv.className = `mb-4 ${message.sender === 'user' ? 'text-right' : 'text-left'}`;
                messageDiv.innerHTML = `
                    <div class="inline-block max-w-xs lg:max-w-md px-4 py-2 rounded-lg ${
                        message.sender === 'user' 
                        ? 'bg-primary text-white' 
                        : 'bg-gray-200 dark:bg-gray-700 text-gray-900 dark:text-white'
                    }">
                        <p class="text-sm">${message.text}</p>
                        <p class="text-xs opacity-75 mt-1">${message.timestamp}</p>
                    </div>
                `;
                chatArea.appendChild(messageDiv);
            });
            
            chatArea.scrollTop = chatArea.scrollHeight;
        }

        function sendMessage() {
            if (currentConversationId === null) return;
            
            const input = document.getElementById('messageInput');
            const messageText = input.value.trim();
            if (!messageText) return;
            
            const message = {
                sender: 'user',
                text: messageText,
                timestamp: new Date().toLocaleTimeString('it-IT', { hour: '2-digit', minute: '2-digit' })
            };
            
            conversations[currentConversationId].messages.push(message);
            input.value = '';
            displayChat();
            
            // Invia il messaggio via WhatsApp
            const whatsappMessage = `💬 *MESSAGGIO DAL CENTRO MESSAGGI*

📝 *Messaggio:* ${messageText}

🕐 *Orario:* ${message.timestamp}

---
Inviato dal Centro Messaggi del sito Da Silva Crediti`;
            
            const whatsappUrl = `https://wa.me/message/IBU2WZ7O6M72C1?text=${encodeURIComponent(whatsappMessage)}`;
            window.open(whatsappUrl, '_blank');
            
            // Simula una risposta automatica
            setTimeout(() => {
                const autoReply = {
                    sender: 'admin',
                    text: 'Grazie per il tuo messaggio! Ti risponderemo il prima possibile.',
                    timestamp: new Date().toLocaleTimeString('it-IT', { hour: '2-digit', minute: '2-digit' })
                };
                conversations[currentConversationId].messages.push(autoReply);
                displayChat();
            }, 1000);
        }

        // Gestione invio messaggio con Enter
        document.getElementById('messageInput').addEventListener('keypress', function(e) {
            if (e.key === 'Enter') {
                sendMessage();
            }
        });

        // Funzione per mostrare messaggi di successo
        function showSuccessMessage(message) {
            const successDiv = document.createElement('div');
            successDiv.className = 'fixed top-4 right-4 bg-green-500 text-white px-6 py-3 rounded-lg shadow-lg z-50';
            successDiv.innerHTML = `
                <div class="flex items-center space-x-2">
                    <i class="fas fa-check-circle"></i>
                    <span>${message}</span>
                </div>
            `;
            document.body.appendChild(successDiv);
            
            setTimeout(() => {
                successDiv.remove();
            }, 5000);
        }

        // Smooth scrolling per i link di navigazione
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({
                        behavior: 'smooth',
                        block: 'start'
                    });
                }
                
                // Chiudi il menu mobile se aperto
                const mobileMenu = document.getElementById('mobileMenu');
                if (!mobileMenu.classList.contains('hidden')) {
                    mobileMenu.classList.add('hidden');
                }
            });
        });

        // Chiudi i modal cliccando fuori
        document.getElementById('loanModal').addEventListener('click', function(e) {
            if (e.target === this) {
                closeLoanForm();
            }
        });

        document.getElementById('messageCenterModal').addEventListener('click', function(e) {
            if (e.target === this) {
                closeMessageCenter();
            }
        });
    </script>
</body>
</html>
