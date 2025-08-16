
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>muhammad naufal ardhi zaidan - Portfolio</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        'sans': ['Inter', 'system-ui', 'sans-serif'],
                        'display': ['Playfair Display', 'serif']
                    },
                    colors: {
                        'luxury-gold': '#D4AF37',
                        'luxury-dark': '#1a1a1a',
                        'luxury-gray': '#2a2a2a'
                    }
                }
            }
        }
    </script>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&family=Playfair+Display:wght@400;500;600;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            scroll-behavior: smooth;
        }
        
        .gradient-text {
            background: linear-gradient(135deg, #D4AF37, #FFE55C);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }
        
        .luxury-shadow {
            box-shadow: 0 25px 50px -12px rgba(0, 0, 0, 0.25), 0 0 0 1px rgba(212, 175, 55, 0.1);
        }
        
        .glass-effect {
            background: rgba(42, 42, 42, 0.8);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(212, 175, 55, 0.2);
        }
        
        .hover-lift {
            transition: all 0.3s ease;
        }
        
        .hover-lift:hover {
            transform: translateY(-10px);
            box-shadow: 0 30px 60px -12px rgba(0, 0, 0, 0.3);
        }
        
        .animate-fadeInUp {
            animation: fadeInUp 0.8s ease-out forwards;
        }
        
        .animate-fadeInLeft {
            animation: fadeInLeft 0.8s ease-out forwards;
        }
        
        .animate-fadeInRight {
            animation: fadeInRight 0.8s ease-out forwards;
        }
        
        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(50px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        
        @keyframes fadeInLeft {
            from {
                opacity: 0;
                transform: translateX(-50px);
            }
            to {
                opacity: 1;
                transform: translateX(0);
            }
        }
        
        @keyframes fadeInRight {
            from {
                opacity: 0;
                transform: translateX(50px);
            }
            to {
                opacity: 1;
                transform: translateX(0);
            }
        }
        
        .typing-animation {
            border-right: 2px solid #D4AF37;
            animation: blink 1s infinite;
        }
        
        @keyframes blink {
            0%, 50% { border-color: #D4AF37; }
            51%, 100% { border-color: transparent; }
        }
        
        .progress-bar {
            transition: width 2s ease-in-out;
        }
        
        .project-card {
            position: relative;
            overflow: hidden;
        }
        
        .project-overlay {
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: linear-gradient(135deg, rgba(212, 175, 55, 0.9), rgba(26, 26, 26, 0.9));
            opacity: 0;
            transition: all 0.3s ease;
            display: flex;
            align-items: center;
            justify-content: center;
            flex-direction: column;
        }
        
        .project-card:hover .project-overlay {
            opacity: 1;
        }
        
        .floating {
            animation: floating 3s ease-in-out infinite;
        }
        
        @keyframes floating {
            0%, 100% { transform: translateY(0px); }
            50% { transform: translateY(-10px); }
        }
        
        .parallax-bg {
            background-attachment: fixed;
            background-position: center;
            background-repeat: no-repeat;
            background-size: cover;
        }
        
        .custom-scrollbar::-webkit-scrollbar {
            width: 8px;
        }
        
        .custom-scrollbar::-webkit-scrollbar-track {
            background: #1a1a1a;
        }
        
        .custom-scrollbar::-webkit-scrollbar-thumb {
            background: #D4AF37;
            border-radius: 4px;
        }
        
        body {
            overflow-x: hidden;
        }
        
        .navbar-blur {
            backdrop-filter: blur(20px);
            background: rgba(26, 26, 26, 0.9);
        }
    </style>
</head>
<body class="bg-luxury-dark text-white font-sans custom-scrollbar">
    <!-- Navigation -->
    <nav class="fixed top-0 w-full z-50 transition-all duration-300" id="navbar">
        <div class="container mx-auto px-6 py-4">
            <div class="flex justify-between items-center">
                <div class="text-2xl font-display font-bold gradient-text">
                    muhammad naufal ardhi zaidan
                </div>
                <div class="hidden md:flex space-x-8">
                    <a href="#home" class="hover:text-luxury-gold transition-colors">Home</a>
                    <a href="#about" class="hover:text-luxury-gold transition-colors">About</a>
                    <a href="#skills" class="hover:text-luxury-gold transition-colors">Skills</a>
                    <a href="#portfolio" class="hover:text-luxury-gold transition-colors">Portfolio</a>
                    <a href="#experience" class="hover:text-luxury-gold transition-colors">Experience</a>
                    <a href="#contact" class="hover:text-luxury-gold transition-colors">Contact</a>
                </div>
                <div class="md:hidden">
                    <button id="mobile-menu-btn" class="text-luxury-gold">
                        <i class="fas fa-bars text-xl"></i>
                    </button>
                </div>
            </div>
        </div>
        <!-- Mobile Menu -->
        <div id="mobile-menu" class="hidden md:hidden glass-effect">
            <div class="px-6 py-4 space-y-4">
                <a href="#home" class="block hover:text-luxury-gold transition-colors">Home</a>
                <a href="#about" class="block hover:text-luxury-gold transition-colors">About</a>
                <a href="#skills" class="block hover:text-luxury-gold transition-colors">Skills</a>
                <a href="#portfolio" class="block hover:text-luxury-gold transition-colors">Portfolio</a>
                <a href="#experience" class="block hover:text-luxury-gold transition-colors">Experience</a>
                <a href="#contact" class="block hover:text-luxury-gold transition-colors">Contact</a>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section id="home" class="min-h-screen flex items-center justify-center relative overflow-hidden">
        <div class="absolute inset-0 z-0">
            <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/16929681-944e-4479-91d6-3632456ebf16.png" alt="Elegant dark workspace with modern laptop, ambient lighting, and minimalist design elements creating a sophisticated professional atmosphere" class="w-full h-full object-cover opacity-20" />
        </div>
        <div class="container mx-auto px-6 text-center relative z-10">
            <div class="animate-fadeInUp">
                <h1 class="text-5xl md:text-7xl font-display font-bold mb-6">
                    <span class="gradient-text"muhammad naufal ardhi zaidan</span>
                </h1>
                <div class="text-xl md:text-2xl mb-8 text-gray-300">
                    <span id="typing-text" class="typing-animation"></span>
                </div>
                <p class="text-lg md:text-xl mb-12 max-w-3xl mx-auto text-gray-400 leading-relaxed">
                    Crafting digital experiences with passion and precision. Specializing in full-stack development, 
                    UI/UX design, and innovative web solutions that bring ideas to life.
                </p>
                <div class="flex flex-col sm:flex-row gap-4 justify-center">
                    <a href="#portfolio" class="bg-luxury-gold text-luxury-dark px-8 py-4 rounded-lg font-semibold hover:bg-yellow-400 transition-all hover-lift">
                        View My Work
                    </a>
                    <a href="#contact" class="border border-luxury-gold text-luxury-gold px-8 py-4 rounded-lg font-semibold hover:bg-luxury-gold hover:text-luxury-dark transition-all">
                        Get In Touch
                    </a>
                </div>
            </div>
        </div>
        <div class="absolute bottom-8 left-1/2 transform -translate-x-1/2 floating">
            <i class="fas fa-chevron-down text-luxury-gold text-2xl"></i>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="py-20 bg-luxury-gray">
        <div class="container mx-auto px-6">
            <div class="grid md:grid-cols-2 gap-12 items-center">
                <div class="animate-fadeInLeft">
                    <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/10c8c5e4-7021-4510-80de-dc376b8db7e6.png" alt="Professional headshot of Alexander Chen in business attire with confident smile against modern office background" class="rounded-2xl luxury-shadow w-full" />
                </div>
                <div class="animate-fadeInRight">
                    <h2 class="text-4xl md:text-5xl font-display font-bold mb-6 gradient-text">About Me</h2>
                    <p class="text-lg text-gray-300 mb-6 leading-relaxed">
                        I'm a passionate full-stack developer with over 8 years of experience creating 
                        digital solutions that matter. My journey began with a curiosity about how 
                        technology can solve real-world problems, and it has evolved into a career 
                        dedicated to crafting exceptional user experiences.
                    </p>
                    <p class="text-lg text-gray-300 mb-8 leading-relaxed">
                        When I'm not coding, you'll find me exploring new technologies, contributing to 
                        open-source projects, or mentoring aspiring developers. I believe in the power 
                        of clean code, thoughtful design, and continuous learning.
                    </p>
                    <div class="grid grid-cols-2 gap-6">
                        <div class="text-center">
                            <div class="text-3xl font-bold gradient-text">150+</div>
                            <div class="text-gray-400">Projects Completed</div>
                        </div>
                        <div class="text-center">
                            <div class="text-3xl font-bold gradient-text">8+</div>
                            <div class="text-gray-400">Years Experience</div>
                        </div>
                        <div class="text-center">
                            <div class="text-3xl font-bold gradient-text">50+</div>
                            <div class="text-gray-400">Happy Clients</div>
                        </div>
                        <div class="text-center">
                            <div class="text-3xl font-bold gradient-text">15+</div>
                            <div class="text-gray-400">Awards Won</div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Skills Section -->
    <section id="skills" class="py-20">
        <div class="container mx-auto px-6">
            <div class="text-center mb-16">
                <h2 class="text-4xl md:text-5xl font-display font-bold mb-6 gradient-text">Skills & Expertise</h2>
                <p class="text-xl text-gray-400 max-w-3xl mx-auto">
                    A comprehensive toolkit built through years of experience and continuous learning
                </p>
            </div>
            
            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Frontend Skills -->
                <div class="glass-effect p-8 rounded-2xl hover-lift">
                    <div class="text-center mb-6">
                        <i class="fas fa-code text-4xl text-luxury-gold mb-4"></i>
                        <h3 class="text-2xl font-bold mb-4">Frontend Development</h3>
                    </div>
                    <div class="space-y-4">
                        <div>
                            <div class="flex justify-between mb-2">
                                <span>React.js</span>
                                <span>95%</span>
                            </div>
                            <div class="bg-gray-700 rounded-full h-2">
                                <div class="bg-luxury-gold h-2 rounded-full progress-bar" style="width: 0%" data-width="95%"></div>
                            </div>
                        </div>
                        <div>
                            <div class="flex justify-between mb-2">
                                <span>Vue.js</span>
                                <span>90%</span>
                            </div>
                            <div class="bg-gray-700 rounded-full h-2">
                                <div class="bg-luxury-gold h-2 rounded-full progress-bar" style="width: 0%" data-width="90%"></div>
                            </div>
                        </div>
                        <div>
                            <div class="flex justify-between mb-2">
                                <span>TypeScript</span>
                                <span>88%</span>
                            </div>
                            <div class="bg-gray-700 rounded-full h-2">
                                <div class="bg-luxury-gold h-2 rounded-full progress-bar" style="width: 0%" data-width="88%"></div>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- Backend Skills -->
                <div class="glass-effect p-8 rounded-2xl hover-lift">
                    <div class="text-center mb-6">
                        <i class="fas fa-server text-4xl text-luxury-gold mb-4"></i>
                        <h3 class="text-2xl font-bold mb-4">Backend Development</h3>
                    </div>
                    <div class="space-y-4">
                        <div>
                            <div class="flex justify-between mb-2">
                                <span>Node.js</span>
                                <span>92%</span>
                            </div>
                            <div class="bg-gray-700 rounded-full h-2">
                                <div class="bg-luxury-gold h-2 rounded-full progress-bar" style="width: 0%" data-width="92%"></div>
                            </div>
                        </div>
                        <div>
                            <div class="flex justify-between mb-2">
                                <span>Python</span>
                                <span>85%</span>
                            </div>
                            <div class="bg-gray-700 rounded-full h-2">
                                <div class="bg-luxury-gold h-2 rounded-full progress-bar" style="width: 0%" data-width="85%"></div>
                            </div>
                        </div>
                        <div>
                            <div class="flex justify-between mb-2">
                                <span>PostgreSQL</span>
                                <span>90%</span>
                            </div>
                            <div class="bg-gray-700 rounded-full h-2">
                                <div class="bg-luxury-gold h-2 rounded-full progress-bar" style="width: 0%" data-width="90%"></div>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- Design Skills -->
                <div class="glass-effect p-8 rounded-2xl hover-lift">
                    <div class="text-center mb-6">
                        <i class="fas fa-paint-brush text-4xl text-luxury-gold mb-4"></i>
                        <h3 class="text-2xl font-bold mb-4">Design & Tools</h3>
                    </div>
                    <div class="space-y-4">
                        <div>
                            <div class="flex justify-between mb-2">
                                <span>UI/UX Design</span>
                                <span>88%</span>
                            </div>
                            <div class="bg-gray-700 rounded-full h-2">
                                <div class="bg-luxury-gold h-2 rounded-full progress-bar" style="width: 0%" data-width="88%"></div>
                            </div>
                        </div>
                        <div>
                            <div class="flex justify-between mb-2">
                                <span>Figma</span>
                                <span>85%</span>
                            </div>
                            <div class="bg-gray-700 rounded-full h-2">
                                <div class="bg-luxury-gold h-2 rounded-full progress-bar" style="width: 0%" data-width="85%"></div>
                            </div>
                        </div>
                        <div>
                            <div class="flex justify-between mb-2">
                                <span>Adobe Creative</span>
                                <span>80%</span>
                            </div>
                            <div class="bg-gray-700 rounded-full h-2">
                                <div class="bg-luxury-gold h-2 rounded-full progress-bar" style="width: 0%" data-width="80%"></div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Portfolio Section -->
    <section id="portfolio" class="py-20 bg-luxury-gray">
        <div class="container mx-auto px-6">
            <div class="text-center mb-16">
                <h2 class="text-4xl md:text-5xl font-display font-bold mb-6 gradient-text">Featured Projects</h2>
                <p class="text-xl text-gray-400 max-w-3xl mx-auto">
                    A selection of my most impactful work, showcasing innovation and technical excellence
                </p>
            </div>

            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Project 1 -->
                <div class="project-card bg-luxury-dark rounded-2xl overflow-hidden luxury-shadow hover-lift">
                    <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/93e3b4cb-d307-47a9-b8a0-7787b1894237.png" alt="Modern e-commerce website interface with clean design, product showcases, and intuitive navigation demonstrating responsive web development" class="w-full h-48 object-cover" />
                    <div class="project-overlay">
                        <h3 class="text-2xl font-bold mb-4">E-Commerce Platform</h3>
                        <p class="text-center mb-6 px-4">Full-stack e-commerce solution with React, Node.js, and Stripe integration</p>
                        <div class="flex space-x-4">
                            <a href="#" class="bg-luxury-gold text-luxury-dark px-4 py-2 rounded-lg font-semibold">View Demo</a>
                            <a href="#" class="border border-white text-white px-4 py-2 rounded-lg font-semibold">View Code</a>
                        </div>
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-bold mb-3">E-Commerce Platform</h3>
                        <p class="text-gray-400 mb-4">A comprehensive online shopping platform with advanced features and seamless user experience.</p>
                        <div class="flex flex-wrap gap-2">
                            <span class="bg-luxury-gold text-luxury-dark px-3 py-1 rounded-full text-sm">React</span>
                            <span class="bg-luxury-gold text-luxury-dark px-3 py-1 rounded-full text-sm">Node.js</span>
                            <span class="bg-luxury-gold text-luxury-dark px-3 py-1 rounded-full text-sm">MongoDB</span>
                        </div>
                    </div>
                </div>

                <!-- Project 2 -->
                <div class="project-card bg-luxury-dark rounded-2xl overflow-hidden luxury-shadow hover-lift">
                    <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/99590f71-3016-466b-91e7-cd1d9c863abb.png" alt="Sophisticated dashboard analytics interface with charts, graphs, and data visualizations for business intelligence and reporting" class="w-full h-48 object-cover" />
                    <div class="project-overlay">
                        <h3 class="text-2xl font-bold mb-4">Analytics Dashboard</h3>
                        <p class="text-center mb-6 px-4">Real-time analytics platform with interactive charts and data visualization</p>
                        <div class="flex space-x-4">
                            <a href="#" class="bg-luxury-gold text-luxury-dark px-4 py-2 rounded-lg font-semibold">View Demo</a>
                            <a href="#" class="border border-white text-white px-4 py-2 rounded-lg font-semibold">View Code</a>
                        </div>
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-bold mb-3">Analytics Dashboard</h3>
                        <p class="text-gray-400 mb-4">Advanced data visualization tool for business intelligence and real-time monitoring.</p>
                        <div class="flex flex-wrap gap-2">
                            <span class="bg-luxury-gold text-luxury-dark px-3 py-1 rounded-full text-sm">Vue.js</span>
                            <span class="bg-luxury-gold text-luxury-dark px-3 py-1 rounded-full text-sm">D3.js</span>
                            <span class="bg-luxury-gold text-luxury-dark px-3 py-1 rounded-full text-sm">Python</span>
                        </div>
                    </div>
                </div>

                <!-- Project 3 -->
                <div class="project-card bg-luxury-dark rounded-2xl overflow-hidden luxury-shadow hover-lift">
                    <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/6da6aef0-2f87-4988-9a54-037cbd5ddc8e.png" alt="Mobile app mockup showing sleek social media interface with modern design, user profiles, and interactive features on smartphone screens" class="w-full h-48 object-cover" />
                    <div class="project-overlay">
                        <h3 class="text-2xl font-bold mb-4">Social Media App</h3>
                        <p class="text-center mb-6 px-4">Mobile-first social platform with real-time messaging and media sharing</p>
                        <div class="flex space-x-4">
                            <a href="#" class="bg-luxury-gold text-luxury-dark px-4 py-2 rounded-lg font-semibold">View Demo</a>
                            <a href="#" class="border border-white text-white px-4 py-2 rounded-lg font-semibold">View Code</a>
                        </div>
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-bold mb-3">Social Media App</h3>
                        <p class="text-gray-400 mb-4">Feature-rich social platform with real-time communication and content sharing capabilities.</p>
                        <div class="flex flex-wrap gap-2">
                            <span class="bg-luxury-gold text-luxury-dark px-3 py-1 rounded-full text-sm">React Native</span>
                            <span class="bg-luxury-gold text-luxury-dark px-3 py-1 rounded-full text-sm">Firebase</span>
                            <span class="bg-luxury-gold text-luxury-dark px-3 py-1 rounded-full text-sm">Socket.io</span>
                        </div>
                    </div>
                </div>

                <!-- Project 4 -->
                <div class="project-card bg-luxury-dark rounded-2xl overflow-hidden luxury-shadow hover-lift">
                    <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/132d3e1b-7b2f-40b0-8fb9-3a6e446db9d5.png" alt="AI-powered web application interface showing machine learning algorithms, data processing flows, and intelligent automation features" class="w-full h-48 object-cover" />
                    <div class="project-overlay">
                        <h3 class="text-2xl font-bold mb-4">AI Web Platform</h3>
                        <p class="text-center mb-6 px-4">Machine learning powered web application with intelligent automation</p>
                        <div class="flex space-x-4">
                            <a href="#" class="bg-luxury-gold text-luxury-dark px-4 py-2 rounded-lg font-semibold">View Demo</a>
                            <a href="#" class="border border-white text-white px-4 py-2 rounded-lg font-semibold">View Code</a>
                        </div>
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-bold mb-3">AI Web Platform</h3>
                        <p class="text-gray-400 mb-4">Cutting-edge AI integration for intelligent data processing and automation workflows.</p>
                        <div class="flex flex-wrap gap-2">
                            <span class="bg-luxury-gold text-luxury-dark px-3 py-1 rounded-full text-sm">TensorFlow</span>
                            <span class="bg-luxury-gold text-luxury-dark px-3 py-1 rounded-full text-sm">FastAPI</span>
                            <span class="bg-luxury-gold text-luxury-dark px-3 py-1 rounded-full text-sm">AWS</span>
                        </div>
                    </div>
                </div>

                <!-- Project 5 -->
                <div class="project-card bg-luxury-dark rounded-2xl overflow-hidden luxury-shadow hover-lift">
                    <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/afb6ae71-23d9-4da1-a871-d8e44bfa9889.png" alt="Cryptocurrency trading platform interface with real-time price charts, trading tools, and market analysis features in a professional dark theme" class="w-full h-48 object-cover" />
                    <div class="project-overlay">
                        <h3 class="text-2xl font-bold mb-4">Crypto Trading Platform</h3>
                        <p class="text-center mb-6 px-4">Real-time cryptocurrency trading platform with advanced charting tools</p>
                        <div class="flex space-x-4">
                            <a href="#" class="bg-luxury-gold text-luxury-dark px-4 py-2 rounded-lg font-semibold">View Demo</a>
                            <a href="#" class="border border-white text-white px-4 py-2 rounded-lg font-semibold">View Code</a>
                        </div>
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-bold mb-3">Crypto Trading Platform</h3>
                        <p class="text-gray-400 mb-4">Professional trading interface with real-time data and advanced technical analysis tools.</p>
                        <div class="flex flex-wrap gap-2">
                            <span class="bg-luxury-gold text-luxury-dark px-3 py-1 rounded-full text-sm">Angular</span>
                            <span class="bg-luxury-gold text-luxury-dark px-3 py-1 rounded-full text-sm">WebSocket</span>
                            <span class="bg-luxury-gold text-luxury-dark px-3 py-1 rounded-full text-sm">Redis</span>
                        </div>
                    </div>
                </div>

                <!-- Project 6 -->
                <div class="project-card bg-luxury-dark rounded-2xl overflow-hidden luxury-shadow hover-lift">
                    <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/9d10d55e-02dc-43a6-9796-b91b9e0d25c2.png" alt="Healthcare management system interface showing patient records, appointment scheduling, and medical data visualization in a clean professional layout" class="w-full h-48 object-cover" />
                    <div class="project-overlay">
                        <h3 class="text-2xl font-bold mb-4">Healthcare System</h3>
                        <p class="text-center mb-6 px-4">Comprehensive healthcare management system with patient portal and analytics</p>
                        <div class="flex space-x-4">
                            <a href="#" class="bg-luxury-gold text-luxury-dark px-4 py-2 rounded-lg font-semibold">View Demo</a>
                            <a href="#" class="border border-white text-white px-4 py-2 rounded-lg font-semibold">View Code</a>
                        </div>
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-bold mb-3">Healthcare System</h3>
                        <p class="text-gray-400 mb-4">Secure healthcare management platform with patient records and appointment scheduling.</p>
                        <div class="flex flex-wrap gap-2">
                            <span class="bg-luxury-gold text-luxury-dark px-3 py-1 rounded-full text-sm">Next.js</span>
                            <span class="bg-luxury-gold text-luxury-dark px-3 py-1 rounded-full text-sm">PostgreSQL</span>
                            <span class="bg-luxury-gold text-luxury-dark px-3 py-1 rounded-full text-sm">Docker</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Experience Section -->
    <section id="experience" class="py-20">
        <div class="container mx-auto px-6">
            <div class="text-center mb-16">
                <h2 class="text-4xl md:text-5xl font-display font-bold mb-6 gradient-text">Professional Journey</h2>
                <p class="text-xl text-gray-400 max-w-3xl mx-auto">
                    A timeline of growth, innovation, and impactful contributions across diverse projects
                </p>
            </div>

            <div class="max-w-4xl mx-auto">
                <!-- Timeline -->
                <div class="relative">
                    <div class="absolute left-1/2 transform -translate-x-1/2 w-1 bg-luxury-gold h-full"></div>
                    
                    <!-- Experience Item 1 -->
                    <div class="mb-12 flex justify-between items-center w-full">
                        <div class="order-1 w-5/12 px-6 py-8 bg-luxury-gray rounded-2xl luxury-shadow hover-lift">
                            <h3 class="text-xl font-bold text-luxury-gold mb-2">Senior Full Stack Developer</h3>
                            <h4 class="text-lg font-semibold mb-2">TechCorp Solutions</h4>
                            <p class="text-sm text-gray-400 mb-4">2021 - Present</p>
                            <p class="text-gray-300">Leading development of enterprise web applications and mentoring junior developers. Implemented microservices architecture resulting in 40% performance improvement.</p>
                        </div>
                        <div class="z-20 flex items-center order-1 bg-luxury-gold shadow-xl w-12 h-12 rounded-full">
                            <h1 class="mx-auto font-semibold text-lg text-luxury-dark">1</h1>
                        </div>
                        <div class="order-1 w-5/12"></div>
                    </div>

                    <!-- Experience Item 2 -->
                    <div class="mb-12 flex justify-between flex-row-reverse items-center w-full">
                        <div class="order-1 w-5/12 px-6 py-8 bg-luxury-gray rounded-2xl luxury-shadow hover-lift">
                            <h3 class="text-xl font-bold text-luxury-gold mb-2">Frontend Developer</h3>
                            <h4 class="text-lg font-semibold mb-2">Digital Innovations Inc.</h4>
                            <p class="text-sm text-gray-400 mb-4">2019 - 2021</p>
                            <p class="text-gray-300">Developed responsive web applications using React and Vue.js. Collaborated with design teams to create pixel-perfect user interfaces and improve user experience metrics by 35%.</p>
                        </div>
                        <div class="z-20 flex items-center order-1 bg-luxury-gold shadow-xl w-12 h-12 rounded-full">
                            <h1 class="mx-auto font-semibold text-lg text-luxury-dark">2</h1>
                        </div>
                        <div class="order-1 w-5/12"></div>
                    </div>

                    <!-- Experience Item 3 -->
                    <div class="mb-12 flex justify-between items-center w-full">
                        <div class="order-1 w-5/12 px-6 py-8 bg-luxury-gray rounded-2xl luxury-shadow hover-lift">
                            <h3 class="text-xl font-bold text-luxury-gold mb-2">Web Developer</h3>
                            <h4 class="text-lg font-semibold mb-2">StartupLab</h4>
                            <p class="text-sm text-gray-400 mb-4">2017 - 2019</p>
                            <p class="text-gray-300">Built and maintained multiple client websites and web applications. Gained experience in full-stack development and agile methodologies while working in a fast-paced startup environment.</p>
                        </div>
                        <div class="z-20 flex items-center order-1 bg-luxury-gold shadow-xl w-12 h-12 rounded-full">
                            <h1 class="mx-auto font-semibold text-lg text-luxury-dark">3</h1>
                        </div>
                        <div class="order-1 w-5/12"></div>
                    </div>

                    <!-- Experience Item 4 -->
                    <div class="mb-12 flex justify-between flex-row-reverse items-center w-full">
                        <div class="order-1 w-5/12 px-6 py-8 bg-luxury-gray rounded-2xl luxury-shadow hover-lift">
                            <h3 class="text-xl font-bold text-luxury-gold mb-2">Junior Developer</h3>
                            <h4 class="text-lg font-semibold mb-2">WebSolutions Co.</h4>
                            <p class="text-sm text-gray-400 mb-4">2016 - 2017</p>
                            <p class="text-gray-300">Started my professional journey learning modern web technologies and best practices. Contributed to various client projects and developed strong foundation in HTML, CSS, JavaScript, and PHP.</p>
                        </div>
                        <div class="z-20 flex items-center order-1 bg-luxury-gold shadow-xl w-12 h-12 rounded-full">
                            <h1 class="mx-auto font-semibold text-lg text-luxury-dark">4</h1>
                        </div>
                        <div class="order-1 w-5/12"></div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-20 bg-luxury-gray">
        <div class="container mx-auto px-6">
            <div class="text-center mb-16">
                <h2 class="text-4xl md:text-5xl font-display font-bold mb-6 gradient-text">Let's Work Together</h2>
                <p class="text-xl text-gray-400 max-w-3xl mx-auto">
                    Ready to bring your ideas to life? Let's discuss your next project and create something extraordinary.
                </p>
            </div>

            <div class="grid md:grid-cols-2 gap-12 max-w-6xl mx-auto">
                <div class="space-y-8">
                    <div class="flex items-center space-x-4">
                        <div class="bg-luxury-gold p-4 rounded-full">
                            <i class="fas fa-envelope text-luxury-dark text-xl"></i>
                        </div>
                        <div>
                            <h3 class="text-xl font-bold mb-1">Email</h3>
                            <p class="text-gray-400">alexander.chen@email.com</p>
                        </div>
                    </div>
                    <div class="flex items-center space-x-4">
                        <div class="bg-luxury-gold p-4 rounded-full">
                            <i class="fas fa-phone text-luxury-dark text-xl"></i>
                        </div>
                        <div>
                            <h3 class="text-xl font-bold mb-1">Phone</h3>
                            <p class="text-gray-400">+1 (555) 123-4567</p>
                        </div>
                    </div>
                    <div class="flex items-center space-x-4">
                        <div class="bg-luxury-gold p-4 rounded-full">
                            <i class="fas fa-map-marker-alt text-luxury-dark text-xl"></i>
                        </div>
                        <div>
                            <h3 class="text-xl font-bold mb-1">Location</h3>
                            <p class="text-gray-400">San Francisco, CA</p>
                        </div>
                    </div>
                    <div class="pt-8">
                        <h3 class="text-xl font-bold mb-4">Follow Me</h3>
                        <div class="flex space-x-4">
                            <a href="#" class="bg-luxury-dark p-3 rounded-full hover:bg-luxury-gold hover:text-luxury-dark transition-all">
                                <i class="fab fa-linkedin text-xl"></i>
                            </a>
                            <a href="#" class="bg-luxury-dark p-3 rounded-full hover:bg-luxury-gold hover:text-luxury-dark transition-all">
                                <i class="fab fa-github text-xl"></i>
                            </a>
                            <a href="#" class="bg-luxury-dark p-3 rounded-full hover:bg-luxury-gold hover:text-luxury-dark transition-all">
                                <i class="fab fa-twitter text-xl"></i>
                            </a>
                            <a href="#" class="bg-luxury-dark p-3 rounded-full hover:bg-luxury-gold hover:text-luxury-dark transition-all">
                                <i class="fab fa-dribbble text-xl"></i>
                            </a>
                        </div>
                    </div>
                </div>

                <div class="glass-effect p-8 rounded-2xl">
                    <form class="space-y-6">
                        <div class="grid md:grid-cols-2 gap-6">
                            <div>
                                <label class="block text-sm font-medium mb-2">First Name</label>
                                <input type="text" class="w-full bg-luxury-dark border border-gray-600 rounded-lg px-4 py-3 focus:border-luxury-gold focus:outline-none transition-colors" placeholder="John">
                            </div>
                            <div>
                                <label class="block text-sm font-medium mb-2">Last Name</label>
                                <input type="text" class="w-full bg-luxury-dark border border-gray-600 rounded-lg px-4 py-3 focus:border-luxury-gold focus:outline-none transition-colors" placeholder="Doe">
                            </div>
                        </div>
                        <div>
                            <label class="block text-sm font-medium mb-2">Email</label>
                            <input type="email" class="w-full bg-luxury-dark border border-gray-600 rounded-lg px-4 py-3 focus:border-luxury-gold focus:outline-none transition-colors" placeholder="john@example.com">
                        </div>
                        <div>
                            <label class="block text-sm font-medium mb-2">Subject</label>
                            <input type="text" class="w-full bg-luxury-dark border border-gray-600 rounded-lg px-4 py-3 focus:border-luxury-gold focus:outline-none transition-colors" placeholder="Project Inquiry">
                        </div>
                        <div>
                            <label class="block text-sm font-medium mb-2">Message</label>
                            <textarea rows="5" class="w-full bg-luxury-dark border border-gray-600 rounded-lg px-4 py-3 focus:border-luxury-gold focus:outline-none transition-colors resize-none" placeholder="Tell me about your project..."></textarea>
                        </div>
                        <button type="submit" class="w-full bg-luxury-gold text-luxury-dark py-3 rounded-lg font-semibold hover:bg-yellow-400 transition-all hover-lift">
                            Send Message
                        </button>
                    </form>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="py-8 bg-luxury-dark border-t border-gray-800">
        <div class="container mx-auto px-6 text-center">
            <p class="text-gray-400">
                © 2025 MUHAMMAD NMAUFAL. All rights reserved. Crafted with passion and precision.
            </p>
        </div>
    </footer>

    <script>
        // Typing animation
        const typingText = document.getElementById('typing-text');
        const phrases = [
            'Full Stack Developer',
            'UI/UX Designer',
            'Problem Solver',
            'Tech Enthusiast'
        ];
        let currentPhrase = 0;
        let currentChar = 0;
        let isDeleting = false;

        function typeText() {
            const current = phrases[currentPhrase];
            
            if (!isDeleting) {
                typingText.textContent = current.substring(0, currentChar + 1);
                currentChar++;
                
                if (currentChar === current.length) {
                    isDeleting = true;
                    setTimeout(typeText, 2000);
                    return;
                }
            } else {
                typingText.textContent = current.substring(0, currentChar - 1);
                currentChar--;
                
                if (currentChar === 0) {
                    isDeleting = false;
                    currentPhrase = (currentPhrase + 1) % phrases.length;
                }
            }
            
            setTimeout(typeText, isDeleting ? 50 : 100);
        }

        // Start typing animation
        typeText();

        // Navbar scroll effect
        const navbar = document.getElementById('navbar');
        window.addEventListener('scroll', () => {
            if (window.scrollY > 100) {
                navbar.classList.add('navbar-blur');
            } else {
                navbar.classList.remove('navbar-blur');
            }
        });

        // Mobile menu toggle
        const mobileMenuBtn = document.getElementById('mobile-menu-btn');
        const mobileMenu = document.getElementById('mobile-menu');
        
        mobileMenuBtn.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
        });

        // Close mobile menu when clicking on links
        const mobileLinks = mobileMenu.querySelectorAll('a');
        mobileLinks.forEach(link => {
            link.addEventListener('click', () => {
                mobileMenu.classList.add('hidden');
            });
        });

        // Progress bars animation
        function animateProgressBars() {
            const progressBars = document.querySelectorAll('.progress-bar');
            progressBars.forEach(bar => {
                const width = bar.getAttribute('data-width');
                bar.style.width = width;
            });
        }

        // Intersection Observer for animations
        const observerOptions = {
            threshold: 0.1,
            rootMargin: '0px 0px -50px 0px'
        };

        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    // Add animation classes
                    if (entry.target.classList.contains('animate-fadeInUp')) {
                        entry.target.style.opacity = '1';
                        entry.target.style.transform = 'translateY(0)';
                    }
                    if (entry.target.classList.contains('animate-fadeInLeft')) {
                        entry.target.style.opacity = '1';
                        entry.target.style.transform = 'translateX(0)';
                    }
                    if (entry.target.classList.contains('animate-fadeInRight')) {
                        entry.target.style.opacity = '1';
                        entry.target.style.transform = 'translateX(0)';
                    }
                    
                    // Animate progress bars when skills section is visible
                    if (entry.target.id === 'skills') {
                        setTimeout(animateProgressBars, 500);
                    }
                }
            });
        }, observerOptions);

        // Observe animated elements
        document.querySelectorAll('.animate-fadeInUp, .animate-fadeInLeft, .animate-fadeInRight').forEach(el => {
            el.style.opacity = '0';
            if (el.classList.contains('animate-fadeInUp')) {
                el.style.transform = 'translateY(50px)';
            }
            if (el.classList.contains('animate-fadeInLeft')) {
                el.style.transform = 'translateX(-50px)';
            }
            if (el.classList.contains('animate-fadeInRight')) {
                el.style.transform = 'translateX(50px)';
            }
            observer.observe(el);
        });

        // Observe skills section for progress bar animation
        const skillsSection = document.getElementById('skills');
        if (skillsSection) {
            observer.observe(skillsSection);
        }

        // Smooth scroll for navigation links
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
            });
        });

        // Form submission
        document.querySelector('form').addEventListener('submit', function(e) {
            e.preventDefault();
            
            // Simple form validation and submission logic
            const formData = new FormData(this);
            
            // Show success message (you would integrate with your backend here)
            alert('Thank you for your message! I will get back to you soon.');
            
            // Reset form
            this.reset();
        });

        // Add loading animation to buttons
        document.querySelectorAll('button, .bg-luxury-gold').forEach(button => {
            button.addEventListener('click', function() {
                const originalText = this.textContent;
                this.style.opacity = '0.8';
                this.style.transform = 'scale(0.98)';
                
                setTimeout(() => {
                    this.style.opacity = '1';
                    this.style.transform = 'scale(1)';
                }, 150);
            });
        });

        // Parallax effect for hero section
        window.addEventListener('scroll', () => {
            const scrolled = window.pageYOffset;
            const parallax = document.querySelector('#home img');
            if (parallax) {
                const speed = scrolled * 0.5;
                parallax.style.transform = `translateY(${speed}px)`;
            }
        });

        // Add cursor trail effect
        let mouseX = 0;
        let mouseY = 0;
        let trail = [];

        document.addEventListener('mousemove', (e) => {
            mouseX = e.clientX;
            mouseY = e.clientY;
        });

        // Counter animation for stats
        function animateCounters() {
            const counters = document.querySelectorAll('.text-3xl.font-bold.gradient-text');
            counters.forEach(counter => {
                const target = parseInt(counter.textContent.replace('+', ''));
                let current = 0;
                const increment = target / 100;
                const timer = setInterval(() => {
                    current += increment;
                    if (current >= target) {
                        counter.textContent = target + '+';
                        clearInterval(timer);
                    } else {
                        counter.textContent = Math.floor(current) + '+';
                    }
                }, 20);
            });
        }

        // Animate counters when about section is visible
        const aboutSection = document.getElementById('about');
        if (aboutSection) {
            const aboutObserver = new IntersectionObserver((entries) => {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        animateCounters();
                        aboutObserver.unobserve(entry.target);
                    }
                });
            }, { threshold: 0.5 });
            
            aboutObserver.observe(aboutSection);
        }
    </script>
</body>
</html>


