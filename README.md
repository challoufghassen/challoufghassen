<!DOCTYPE html>
<html lang="en" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Challouf Ghassen | Cybersecurity Portfolio</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;700;900&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Inter', sans-serif;
        }
        .chart-container {
            position: relative;
            width: 100%;
            max-width: 500px;
            margin-left: auto;
            margin-right: auto;
            height: 300px;
            max-height: 40vh;
        }
        @media (min-width: 768px) {
            .chart-container {
                height: 400px;
            }
        }
        .modal-backdrop {
            transition: opacity 0.3s ease-in-out;
        }
        .modal-content {
            transition: transform 0.3s ease-in-out;
        }
        .nav-link::after {
            content: '';
            display: block;
            width: 0;
            height: 2px;
            background: #4fd1c5;
            transition: width .3s;
        }
        .nav-link:hover::after {
            width: 100%;
        }
        .active-link::after {
            width: 100%;
        }
        .gradient-text {
            background: linear-gradient(135deg, #4fd1c5, #38b2ac);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }
        .card-hover {
            transition: all 0.3s ease;
        }
        .card-hover:hover {
            transform: translateY(-8px);
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.3);
        }
    </style>
</head>
<body class="bg-gray-900 text-gray-300 antialiased">

<header id="header" class="bg-gray-900/95 backdrop-blur-sm sticky top-0 z-50 border-b border-gray-800">
    <nav class="container mx-auto px-6 py-4 flex justify-between items-center">
        <a href="#hero" class="text-xl font-bold text-white hover:text-teal-400 transition-colors">Ghassen Challouf</a>
        <div class="hidden md:flex space-x-8">
            <a href="#about" class="nav-link text-gray-300 hover:text-teal-400 transition-colors duration-300">About</a>
            <a href="#skills" class="nav-link text-gray-300 hover:text-teal-400 transition-colors duration-300">Skills</a>
            <a href="#projects" class="nav-link text-gray-300 hover:text-teal-400 transition-colors duration-300">Projects</a>
            <a href="#certs" class="nav-link text-gray-300 hover:text-teal-400 transition-colors duration-300">Certifications</a>
        </div>
        <button id="mobile-menu-button" class="md:hidden text-white hover:text-teal-400 transition-colors">
            <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16m-7 6h7"></path>
            </svg>
        </button>
    </nav>
    <div id="mobile-menu" class="hidden md:hidden px-6 pb-4 border-t border-gray-800">
        <a href="#about" class="block py-3 text-gray-300 hover:text-teal-400 transition-colors">About</a>
        <a href="#skills" class="block py-3 text-gray-300 hover:text-teal-400 transition-colors">Skills</a>
        <a href="#projects" class="block py-3 text-gray-300 hover:text-teal-400 transition-colors">Projects</a>
        <a href="#certs" class="block py-3 text-gray-300 hover:text-teal-400 transition-colors">Certifications</a>
    </div>
</header>

<main class="container mx-auto px-6">

    <section id="hero" class="min-h-screen flex items-center justify-center text-center">
        <div class="max-w-5xl">
            <h1 class="text-4xl md:text-6xl lg:text-7xl font-black text-white leading-tight mb-6">
                Cybersecurity Engineering Student & 
                <span class="gradient-text">Aspiring Penetration Tester</span>
            </h1>
            <p class="text-lg md:text-xl lg:text-2xl text-gray-400 mb-10 max-w-3xl mx-auto">
                Passionate about offensive security and vulnerability analysis, driven to build and defend secure digital environments.
            </p>
            <div class="flex justify-center items-center space-x-6">
                <a href="https://www.linkedin.com/in/ghassen-challouf/" target="_blank" 
                   class="bg-teal-600 hover:bg-teal-700 text-white px-8 py-3 rounded-lg font-semibold transition-all duration-300 transform hover:scale-105">
                    LinkedIn Profile
                </a>
                <a href="https://tryhackme.com/p/Ghassencha" target="_blank" 
                   class="border-2 border-teal-400 text-teal-400 hover:bg-teal-400 hover:text-gray-900 px-8 py-3 rounded-lg font-semibold transition-all duration-300 transform hover:scale-105">
                    TryHackMe
                </a>
            </div>
        </div>
    </section>

    <section id="about" class="py-20">
        <h2 class="text-4xl md:text-5xl font-bold text-white text-center mb-16">About Me</h2>
        <div class="grid md:grid-cols-5 gap-8 items-start">
            <div class="md:col-span-3 bg-gray-800/50 backdrop-blur-sm p-8 rounded-xl shadow-2xl border border-gray-700">
                <p class="text-lg mb-6 leading-relaxed">
                    I am a second-year engineering student at TEK-UP, specializing in Cybersecurity. I am passionate about offensive security and vulnerability analysis, actively seeking an internship in penetration testing to apply and expand my technical skills in a dynamic professional environment.
                </p>
                <p class="text-lg leading-relaxed">
                    I am a motivated, organized, and responsible individual, always eager to learn new technical skills and deepen my acquired knowledge. I enjoy teamwork and am driven to contribute effectively to group projects.
                </p>
            </div>
            <div class="md:col-span-2 space-y-6">
                <div class="bg-gray-800/50 backdrop-blur-sm p-6 rounded-xl shadow-lg border border-gray-700">
                    <h3 class="font-bold text-white text-xl mb-4 flex items-center">
                        <span class="text-2xl mr-3">🔭</span>
                        Currently Focused On
                    </h3>
                    <ul class="space-y-3 text-gray-300">
                        <li class="flex items-start">
                            <span class="text-teal-400 mr-2">•</span>
                            Honing skills in Penetration Testing Methodologies
                        </li>
                        <li class="flex items-start">
                            <span class="text-teal-400 mr-2">•</span>
                            Analyzing malware like the Zus Trojan
                        </li>
                        <li class="flex items-start">
                            <span class="text-teal-400 mr-2">•</span>
                            Contributing to CTF designs for events
                        </li>
                    </ul>
                </div>
                <div class="bg-gray-800/50 backdrop-blur-sm p-6 rounded-xl shadow-lg border border-gray-700">
                    <h3 class="font-bold text-white text-xl mb-4 flex items-center">
                        <span class="text-2xl mr-3">🌱</span>
                        Actively Learning
                    </h3>
                    <ul class="space-y-3 text-gray-300">
                        <li class="flex items-start">
                            <span class="text-teal-400 mr-2">•</span>
                            Advanced Exploitation Techniques
                        </li>
                        <li class="flex items-start">
                            <span class="text-teal-400 mr-2">•</span>
                            Digital Forensics & Threat Hunting
                        </li>
                        <li class="flex items-start">
                            <span class="text-teal-400 mr-2">•</span>
                            Preparing for eJPT Certification
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <section id="skills" class="py-20">
        <h2 class="text-4xl md:text-5xl font-bold text-white text-center mb-6">My Arsenal</h2>
        <p class="text-center text-gray-400 max-w-3xl mx-auto mb-16 text-lg">
            Here is a visual overview of my core competency areas. This chart highlights the domains where I focus my learning and practice. Below, you'll find a more detailed breakdown of the specific tools and technologies I use.
        </p>
        <div class="grid lg:grid-cols-2 gap-16 items-center">
            <div class="bg-gray-800/30 p-8 rounded-xl border border-gray-700">
                <div class="chart-container">
                    <canvas id="skillsChart"></canvas>
                </div>
            </div>
            <div>
                <div id="skill-tabs">
                    <div class="border-b border-gray-700 mb-6">
                        <nav class="-mb-px flex space-x-8" aria-label="Tabs">
                            <button class="tab-btn whitespace-nowrap py-4 px-1 border-b-2 font-medium text-lg border-teal-500 text-teal-400" data-target="tools">Tools</button>
                            <button class="tab-btn whitespace-nowrap py-4 px-1 border-b-2 font-medium text-lg border-transparent text-gray-500 hover:text-gray-300 hover:border-gray-400 transition-all" data-target="concepts">Concepts</button>
                            <button class="tab-btn whitespace-nowrap py-4 px-1 border-b-2 font-medium text-lg border-transparent text-gray-500 hover:text-gray-300 hover:border-gray-400 transition-all" data-target="os">Systems</button>
                        </nav>
                    </div>
                    <div id="tools" class="tab-content grid grid-cols-2 sm:grid-cols-3 gap-4">
                        <span class="bg-gray-800 hover:bg-gray-700 p-4 rounded-lg text-center transition-colors cursor-default">Metasploit</span>
                        <span class="bg-gray-800 hover:bg-gray-700 p-4 rounded-lg text-center transition-colors cursor-default">Wireshark</span>
                        <span class="bg-gray-800 hover:bg-gray-700 p-4 rounded-lg text-center transition-colors cursor-default">Burp Suite</span>
                        <span class="bg-gray-800 hover:bg-gray-700 p-4 rounded-lg text-center transition-colors cursor-default">Ghidra</span>
                        <span class="bg-gray-800 hover:bg-gray-700 p-4 rounded-lg text-center transition-colors cursor-default">OWASP</span>
                        <span class="bg-gray-800 hover:bg-gray-700 p-4 rounded-lg text-center transition-colors cursor-default">ELK Stack</span>
                    </div>
                    <div id="concepts" class="tab-content hidden grid grid-cols-2 sm:grid-cols-3 gap-4">
                        <span class="bg-gray-800 hover:bg-gray-700 p-4 rounded-lg text-center transition-colors cursor-default">Penetration Testing</span>
                        <span class="bg-gray-800 hover:bg-gray-700 p-4 rounded-lg text-center transition-colors cursor-default">Network Security</span>
                        <span class="bg-gray-800 hover:bg-gray-700 p-4 rounded-lg text-center transition-colors cursor-default">Digital Forensics</span>
                        <span class="bg-gray-800 hover:bg-gray-700 p-4 rounded-lg text-center transition-colors cursor-default">OSINT</span>
                        <span class="bg-gray-800 hover:bg-gray-700 p-4 rounded-lg text-center transition-colors cursor-default">Threat Hunting</span>
                        <span class="bg-gray-800 hover:bg-gray-700 p-4 rounded-lg text-center transition-colors cursor-default">Host Auditing</span>
                    </div>
                    <div id="os" class="tab-content hidden grid grid-cols-2 sm:grid-cols-3 gap-4">
                        <span class="bg-gray-800 hover:bg-gray-700 p-4 rounded-lg text-center transition-colors cursor-default">Linux</span>
                        <span class="bg-gray-800 hover:bg-gray-700 p-4 rounded-lg text-center transition-colors cursor-default">Debian</span>
                        <span class="bg-gray-800 hover:bg-gray-700 p-4 rounded-lg text-center transition-colors cursor-default">RHEL</span>
                        <span class="bg-gray-800 hover:bg-gray-700 p-4 rounded-lg text-center transition-colors cursor-default">Ubuntu</span>
                        <span class="bg-gray-800 hover:bg-gray-700 p-4 rounded-lg text-center transition-colors cursor-default">Windows</span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <section id="projects" class="py-20">
        <h2 class="text-4xl md:text-5xl font-bold text-white text-center mb-6">Field Work</h2>
        <p class="text-center text-gray-400 max-w-3xl mx-auto mb-16 text-lg">
            Theory is essential, but application is where knowledge is forged. This section showcases some of the key projects where I've applied my skills to solve real-world problems. Click on any project to learn more about the objectives, process, and outcomes.
        </p>
        <div id="project-grid" class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
        </div>
    </section>

    <section id="certs" class="py-20">
        <h2 class="text-4xl md:text-5xl font-bold text-white text-center mb-6">Certifications</h2>
        <p class="text-center text-gray-400 max-w-3xl mx-auto mb-16 text-lg">
            Formal certifications validate the skills and knowledge acquired through study and hands-on practice. Here are the credentials I have earned to date, demonstrating my proficiency in key areas of cybersecurity.
        </p>
        <div class="max-w-5xl mx-auto grid sm:grid-cols-2 lg:grid-cols-3 gap-8">
            <div class="bg-gray-800/50 backdrop-blur-sm p-8 rounded-xl shadow-lg border border-gray-700 text-center card-hover">
                <div class="w-16 h-16 bg-teal-600 rounded-full flex items-center justify-center mx-auto mb-4">
                    <svg class="w-8 h-8 text-white" fill="currentColor" viewBox="0 0 20 20">
                        <path d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z"/>
                    </svg>
                </div>
                <h3 class="text-xl font-bold text-white mb-2">Junior Penetration Tester</h3>
                <p class="text-teal-400 font-medium">INE Security</p>
            </div>
            <div class="bg-gray-800/50 backdrop-blur-sm p-8 rounded-xl shadow-lg border border-gray-700 text-center card-hover">
                <div class="w-16 h-16 bg-teal-600 rounded-full flex items-center justify-center mx-auto mb-4">
                    <svg class="w-8 h-8 text-white" fill="currentColor" viewBox="0 0 20 20">
                        <path d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z"/>
                    </svg>
                </div>
                <h3 class="text-xl font-bold text-white mb-2">Web Penetration Tester</h3>
                <p class="text-teal-400 font-medium">INE Security</p>
            </div>
            <div class="bg-gray-800/50 backdrop-blur-sm p-8 rounded-xl shadow-lg border border-gray-700 text-center card-hover">
                <div class="w-16 h-16 bg-teal-600 rounded-full flex items-center justify-center mx-auto mb-4">
                    <svg class="w-8 h-8 text-white" fill="currentColor" viewBox="0 0 20 20">
                        <path d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z"/>
                    </svg>
                </div>
                <h3 class="text-xl font-bold text-white mb-2">Blue Team Junior Analyst</h3>
                <p class="text-teal-400 font-medium">Security Blue Team</p>
            </div>
        </div>
    </section>

</main>

<footer class="bg-gray-800/50 backdrop-blur-sm border-t border-gray-700 py-12">
    <div class="container mx-auto px-6 text-center">
        <div class="mb-6">
            <h3 class="text-2xl font-bold text-white mb-2">Let's Connect</h3>
            <p class="text-gray-400">Ready to discuss cybersecurity opportunities</p>
        </div>
        <div class="flex justify-center space-x-6 mb-8">
            <a href="https://www.linkedin.com/in/ghassen-challouf/" target="_blank" 
               class="text-gray-400 hover:text-teal-400 transition-colors">
                <span class="sr-only">LinkedIn</span>
                <svg class="w-6 h-6" fill="currentColor" viewBox="0 0 24 24">
                    <path d="M20.447 20.452h-3.554v-5.569c0-1.328-.027-3.037-1.852-3.037-1.853 0-2.136 1.445-2.136 2.939v5.667H9.351V9h3.414v1.561h.046c.477-.9 1.637-1.85 3.37-1.85 3.601 0 4.267 2.37 4.267 5.455v6.286zM5.337 7.433c-1.144 0-2.063-.926-2.063-2.065 0-1.138.92-2.063 2.063-2.063 1.14 0 2.064.925 2.064 2.063 0 1.139-.925 2.065-2.064 2.065zm1.782 13.019H3.555V9h3.564v11.452zM22.225 0H1.771C.792 0 0 .774 0 1.729v20.542C0 23.227.792 24 1.771 24h20.451C23.2 24 24 23.227 24 22.271V1.729C24 .774 23.2 0 22.222 0h.003z"/>
                </svg>
            </a>
            <a href="https://tryhackme.com/p/Ghassencha" target="_blank" 
               class="text-gray-400 hover:text-teal-400 transition-colors">
                <span class="sr-only">TryHackMe</span>
                <svg class="w-6 h-6" fill="currentColor" viewBox="0 0 24 24">
                    <path d="M12 0C5.373 0 0 5.373 0 12s5.373 12 12 12 12-5.373 12-12S18.627 0 12 0zm0 2c5.523 0 10 4.477 10 10s-4.477 10-10 10S2 17.523 2 12 6.477 2 12 2z"/>
                </svg>
            </a>
        </div>
        <div class="border-t border-gray-700 pt-8">
            <p class="text-gray-400 mb-2">&copy; 2024 Challouf Ghassen. All rights reserved.</p>
            <p class="text-gray-500 text-sm">Built with determination and a little bit of caffeine ☕</p>
        </div>
    </div>
</footer>

<!-- Modal -->
<div id="project-modal" class="modal-backdrop fixed inset-0 bg-black/80 backdrop-blur-sm flex items-center justify-center p-4 opacity-0 pointer-events-none z-50">
    <div class="modal-content bg-gray-800 rounded-xl shadow-2xl w-full max-w-3xl max-h-[90vh] overflow-y-auto transform scale-95 border border-gray-700">
        <div class="sticky top-0 bg-gray-800 p-6 border-b border-gray-700 flex justify-between items-center rounded-t-xl">
            <h3 id="modal-title" class="text-2xl font-bold text-white"></h3>
            <button id="modal-close" class="text-gray-400 hover:text-white text-3xl leading-none">&times;</button>
        </div>
        <div class="p-8">
            <p id="modal-description" class="text-gray-300 mb-8 text-lg leading-relaxed"></p>
            <h4 class="font-bold text-white mb-4 text-lg">Tools & Technologies Used:</h4>
            <div id="modal-tools" class="flex flex-wrap gap-3"></div>
        </div>
    </div>
</div>

<script>
    document.addEventListener('DOMContentLoaded', () => {
        // Mobile menu functionality
        const mobileMenuButton = document.getElementById('mobile-menu-button');
        const mobileMenu = document.getElementById('mobile-menu');
        
        mobileMenuButton.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
        });

        // Close mobile menu when clicking nav links
        const navLinks = document.querySelectorAll('#header a');
        navLinks.forEach(link => {
            link.addEventListener('click', () => {
                if (!mobileMenu.classList.contains('hidden')) {
                    mobileMenu.classList.add('hidden');
                }
            });
        });

        // Active navigation highlighting
        const sections = document.querySelectorAll('section');
        const headerNavLinks = document.querySelectorAll('#header .hidden a');
        
        window.addEventListener('scroll', () => {
            let current = '';
            sections.forEach(section => {
                const sectionTop = section.offsetTop;
                if (pageYOffset >= sectionTop - 100) {
                    current = section.getAttribute('id');
                }
            });
            
            headerNavLinks.forEach(link => {
                link.classList.remove('active-link', 'text-teal-400');
                if (link.href.includes(current)) {
                    link.classList.add('active-link', 'text-teal-400');
                }
            });
        });

        // Skills radar chart
        const ctx = document.getElementById('skillsChart').getContext('2d');
        const skillsChart = new Chart(ctx, {
            type: 'radar',
            data: {
                labels: ['Offensive Security', 'Defensive Security', 'Network Analysis', 'Malware Analysis', 'Forensics', 'Vulnerability Assessment'],
                datasets: [{
                    label: 'Skill Level',
                    data: [9, 6, 7, 8, 7, 9],
                    backgroundColor: 'rgba(79, 209, 197, 0.15)',
                    borderColor: 'rgba(79, 209, 197, 1)',
                    borderWidth: 3,
                    pointBackgroundColor: 'rgba(79, 209, 197, 1)',
                    pointBorderColor: '#fff',
                    pointBorderWidth: 2,
                    pointRadius: 6,
                    pointHoverBackgroundColor: '#fff',
                    pointHoverBorderColor: 'rgba(79, 209, 197, 1)',
                    pointHoverRadius: 8
                }]
            },
            options: {
                maintainAspectRatio: false,
                responsive: true,
                scales: {
                    r: {
                        beginAtZero: true,
                        max: 10,
                        angleLines: { 
                            color: 'rgba(255, 255, 255, 0.1)',
                            lineWidth: 1
                        },
                        grid: { 
                            color: 'rgba(255, 255, 255, 0.1)',
                            lineWidth: 1
                        },
                        pointLabels: { 
                            color: '#a0aec0', 
                            font: { 
                                size: 14,
                                weight: '500'
                            }
                        },
                        ticks: {
                            color: 'rgba(160, 174, 192, 0.8)',
                            backdropColor: 'rgba(31, 41, 55, 0.8)',
                            stepSize: 2,
                            font: {
                                size: 12
                            }
                        }
                    }
                },
                plugins: {
                    legend: {
                        display: false
                    },
                    tooltip: {
                        backgroundColor: 'rgba(31, 41, 55, 0.9)',
                        titleColor: '#fff',
                        bodyColor: '#a0aec0',
                        borderColor: 'rgba(79, 209, 197, 1)',
                        borderWidth: 1
                    }
                }
            }
        });

        // Skills tabs functionality
        const tabs = document.querySelectorAll('.tab-btn');
        const tabContents = document.querySelectorAll('.tab-content');
        
        tabs.forEach(tab => {
            tab.addEventListener('click', () => {
                const target = document.getElementById(tab.dataset.target);
                
                // Hide all tab contents
                tabContents.forEach(tc => tc.classList.add('hidden'));
                target.classList.remove('hidden');

                // Update tab styles
                tabs.forEach(t => {
                    t.classList.remove('border-teal-500', 'text-teal-400');
                    t.classList.add('border-transparent', 'text-gray-500');
                });
                tab.classList.remove('border-transparent', 'text-gray-500');
                tab.classList.add('border-teal-500', 'text-teal-400');
            });
        });

        // Projects data and modal functionality
        const projectsData = [
            {
                title: "Zus Trojan Malware Analysis",
                description: "Conducted an in-depth analysis of the Zus Trojan, a complex banking malware. The primary goal was to understand its propagation methods, evasion techniques, and data exfiltration capabilities. This comprehensive analysis involved reverse engineering the malware binary, examining its network communications, and identifying its command and control infrastructure. Based on the findings, I developed custom detection rules for SIEM systems and outlined effective defense strategies to mitigate the risk of financial fraud. The project also included creating indicators of compromise (IOCs) and developing incident response procedures for organizations potentially affected by this threat.",
                tools: ["Ghidra", "Wireshark", "Docker", "IDA Pro", "Volatility", "YARA"]
            },
            {
                title: "Secure Facial Recognition System",
                description: "Designed and deployed a secure facial recognition surveillance system with a strong focus on privacy and security. This project involved implementing end-to-end encryption for biometric data, secure storage mechanisms, and access control systems. The system was built with strict compliance to GDPR and other data protection standards throughout its architecture and operational lifecycle. Key features included real-time face detection and recognition, encrypted database storage, audit logging, and user consent management. The project also incorporated privacy-by-design principles, ensuring that personal data processing was minimized and transparent to users.",
                tools: ["Python", "OpenCV", "TensorFlow", "Linux", "PostgreSQL", "Docker"]
            },
            {
                title: "eJPT Certification Training Program",
                description: "Organized and led a comprehensive hands-on cybersecurity training program to support fellow students in preparing for and achieving the eJPT (eLearnSecurity Junior Penetration Tester) certification. The curriculum covered foundational penetration testing methodologies, network reconnaissance and scanning with Nmap, vulnerability assessment techniques, and various exploitation methods using Metasploit. The program included practical lab exercises, simulated penetration testing scenarios, and mock examinations. Over 20 students participated in the program, with an 85% certification pass rate. The training materials and lab environments I developed are now used as part of the university's cybersecurity curriculum.",
                tools: ["Metasploit", "Nmap", "Burp Suite", "Kali Linux", "VirtualBox", "CTF Design"]
            },
            {
                title: "Securinets CTF Challenge Development",
                description: "As a core technical team member for Securinets at TEK-UP, I was responsible for creating, testing, and deploying Capture The Flag (CTF) challenges for various cybersecurity events and competitions. This involved developing vulnerable web applications with realistic security flaws, designing network-based challenges that simulate real-world attack scenarios, and creating cryptographic puzzles that test participants' analytical skills. Each challenge was thoroughly tested and documented with detailed write-ups and solution guides. The challenges I developed were used in regional CTF competitions, attracting over 200 participants from universities across Tunisia and neighboring countries.",
                tools: ["Web Security", "PHP", "JavaScript", "Docker", "Linux", "Cryptography"]
            }
        ];

        // Generate project cards
        const projectGrid = document.getElementById('project-grid');
        const modal = document.getElementById('project-modal');
        const modalTitle = document.getElementById('modal-title');
        const modalDescription = document.getElementById('modal-description');
        const modalTools = document.getElementById('modal-tools');
        const modalClose = document.getElementById('modal-close');

        projectsData.forEach((project, index) => {
            const card = document.createElement('div');
            card.className = 'bg-gray-800/50 backdrop-blur-sm rounded-xl overflow-hidden shadow-lg cursor-pointer card-hover border border-gray-700';
            card.innerHTML = `
                <div class="p-8">
                    <div class="w-12 h-12 bg-teal-600 rounded-lg flex items-center justify-center mb-4">
                        <span class="text-white font-bold text-xl">${index + 1}</span>
                    </div>
                    <h3 class="text-xl font-bold text-white mb-4">${project.title}</h3>
                    <p class="text-gray-400 mb-4 line-clamp-3">${project.description.substring(0, 150)}...</p>
                    <div class="flex flex-wrap gap-2 mb-4">
                        ${project.tools.slice(0, 3).map(tool => 
                            `<span class="bg-gray-700 text-teal-300 text-xs font-medium px-2 py-1 rounded">${tool}</span>`
                        ).join('')}
                        ${project.tools.length > 3 ? `<span class="text-gray-500 text-xs">+${project.tools.length - 3} more</span>` : ''}
                    </div>
                    <div class="text-teal-400 font-medium text-sm">Click to learn more →</div>
                </div>
            `;
            card.addEventListener('click', () => openModal(project));
            projectGrid.appendChild(card);
        });

        // Modal functions
        function openModal(project) {
            modalTitle.textContent = project.title;
            modalDescription.textContent = project.description;
            modalTools.innerHTML = project.tools.map(tool => 
                `<span class="bg-gray-700 text-teal-300 text-sm font-medium px-3 py-2 rounded-lg">${tool}</span>`
            ).join('');
            
            modal.classList.remove('opacity-0', 'pointer-events-none');
            modal.querySelector('.modal-content').classList.remove('scale-95');
            document.body.style.overflow = 'hidden';
        }
        
        function closeModal() {
            modal.classList.add('opacity-0', 'pointer-events-none');
            modal.querySelector('.modal-content').classList.add('scale-95');
            document.body.style.overflow = 'auto';
        }

        // Modal event listeners
        modalClose.addEventListener('click', closeModal);
        modal.addEventListener('click', (e) => {
            if (e.target === modal) {
                closeModal();
            }
        });
        document.addEventListener('keydown', (e) => {
            if (e.key === 'Escape') {
                closeModal();
            }
        });

        // Smooth scrolling for anchor links
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
    });
</script>

</body>
</html>
