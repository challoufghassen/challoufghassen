<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ghassen Challouf | Cybersecurity Engineer</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Fira+Code:wght@400;500;700&family=Inter:wght@400;500;700;900&display=swap');
        
        body {
            font-family: 'Inter', sans-serif;
            background-color: #0a0a0a;
            color: #e5e7eb;
        }
        
        .code-font {
            font-family: 'Fira Code', monospace;
        }
        
        .gradient-text {
            background: linear-gradient(90deg, #4fd1c5, #38b2ac, #319795);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
        }
        
        .skill-badge {
            transition: all 0.3s ease;
        }
        
        .skill-badge:hover {
            transform: translateY(-2px);
            box-shadow: 0 4px 6px rgba(79, 209, 197, 0.3);
        }
        
        .project-card {
            transition: all 0.3s ease;
            border-left: 3px solid transparent;
        }
        
        .project-card:hover {
            transform: translateY(-5px);
            border-left: 3px solid #4fd1c5;
            box-shadow: 0 10px 15px rgba(0, 0, 0, 0.2);
        }
        
        .nav-link {
            position: relative;
        }
        
        .nav-link::after {
            content: '';
            position: absolute;
            bottom: -2px;
            left: 0;
            width: 0;
            height: 2px;
            background: #4fd1c5;
            transition: width 0.3s ease;
        }
        
        .nav-link:hover::after {
            width: 100%;
        }
        
        .active-nav::after {
            width: 100%;
        }
    </style>
</head>
<body class="bg-gray-900">
    <!-- Header/Navigation -->
    <header class="sticky top-0 z-50 bg-gray-900/90 backdrop-blur-sm border-b border-gray-800">
        <div class="container mx-auto px-6 py-4">
            <div class="flex justify-between items-center">
                <a href="#" class="text-2xl font-bold text-white">
                    <span class="gradient-text">GhassenC</span>
                </a>
                
                <nav class="hidden md:flex space-x-8">
                    <a href="#about" class="nav-link text-gray-300 hover:text-teal-400">About</a>
                    <a href="#skills" class="nav-link text-gray-300 hover:text-teal-400">Skills</a>
                    <a href="#projects" class="nav-link text-gray-300 hover:text-teal-400">Projects</a>
                    <a href="#experience" class="nav-link text-gray-300 hover:text-teal-400">Experience</a>
                    <a href="#contact" class="nav-link text-gray-300 hover:text-teal-400">Contact</a>
                </nav>
                
                <button id="mobile-menu-button" class="md:hidden text-gray-300 focus:outline-none">
                    <i class="fas fa-bars text-xl"></i>
                </button>
            </div>
            
            <!-- Mobile Menu -->
            <div id="mobile-menu" class="hidden md:hidden mt-4 space-y-2 pb-2">
                <a href="#about" class="block py-2 text-gray-300 hover:text-teal-400">About</a>
                <a href="#skills" class="block py-2 text-gray-300 hover:text-teal-400">Skills</a>
                <a href="#projects" class="block py-2 text-gray-300 hover:text-teal-400">Projects</a>
                <a href="#experience" class="block py-2 text-gray-300 hover:text-teal-400">Experience</a>
                <a href="#contact" class="block py-2 text-gray-300 hover:text-teal-400">Contact</a>
            </div>
        </div>
    </header>

    <!-- Hero Section -->
    <section id="hero" class="min-h-screen flex items-center justify-center py-20">
        <div class="container mx-auto px-6 text-center">
            <div class="max-w-3xl mx-auto">
                <h1 class="text-4xl md:text-6xl font-bold text-white mb-6">
                    <span class="gradient-text">Cybersecurity Engineer</span> &<br>
                    Penetration Tester
                </h1>
                
                <p class="text-xl text-gray-400 mb-8">
                    I identify vulnerabilities, secure systems, and help organizations defend against cyber threats.
                </p>
                
                <div class="flex justify-center space-x-4">
                    <a href="https://www.linkedin.com/in/ghassen-challouf/" target="_blank" class="bg-teal-600 hover:bg-teal-700 text-white px-6 py-3 rounded-lg font-medium transition-colors">
                        Connect on LinkedIn
                    </a>
                    <a href="#projects" class="border border-teal-400 text-teal-400 hover:bg-teal-400 hover:text-gray-900 px-6 py-3 rounded-lg font-medium transition-colors">
                        View My Work
                    </a>
                </div>
                
                <div class="mt-12 flex justify-center space-x-6">
                    <a href="https://tryhackme.com/p/Ghassencha" target="_blank" class="text-gray-400 hover:text-teal-400 text-xl">
                        <i class="fas fa-shield-alt"></i>
                    </a>
                    <a href="https://github.com/ghassencha" target="_blank" class="text-gray-400 hover:text-teal-400 text-xl">
                        <i class="fab fa-github"></i>
                    </a>
                    <a href="#" class="text-gray-400 hover:text-teal-400 text-xl">
                        <i class="fas fa-file-pdf"></i>
                    </a>
                </div>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="py-20 bg-gray-800/50">
        <div class="container mx-auto px-6">
            <div class="flex flex-col md:flex-row items-center">
                <div class="md:w-1/3 mb-10 md:mb-0 flex justify-center">
                    <div class="relative">
                        <div class="w-64 h-64 rounded-full overflow-hidden border-4 border-teal-400 shadow-lg">
                            <img src="https://via.placeholder.com/256" alt="Ghassen Challouf" class="w-full h-full object-cover">
                        </div>
                        <div class="absolute -bottom-3 -right-3 bg-gray-900 px-4 py-2 rounded-full border border-teal-400 shadow-lg">
                            <span class="text-teal-400 font-bold">Security Engineer</span>
                        </div>
                    </div>
                </div>
                
                <div class="md:w-2/3 md:pl-12">
                    <h2 class="text-3xl font-bold text-white mb-6">
                        <span class="border-b-2 border-teal-400 pb-2">About Me</span>
                    </h2>
                    
                    <p class="text-gray-400 mb-6 text-lg">
                        I'm a second-year Cybersecurity Engineering student at TEK-UP with a passion for offensive security and vulnerability research. My journey in cybersecurity began with a curiosity about how systems can be compromised and how to defend them.
                    </p>
                    
                    <p class="text-gray-400 mb-8 text-lg">
                        Currently focused on preparing for the eJPT certification while contributing to security research projects. I enjoy participating in CTF competitions and analyzing real-world malware samples to understand attacker techniques.
                    </p>
                    
                    <div class="grid grid-cols-1 sm:grid-cols-2 gap-4">
                        <div class="bg-gray-900 p-4 rounded-lg border-l-4 border-teal-400">
                            <h3 class="font-bold text-white mb-2"><i class="fas fa-bullseye text-teal-400 mr-2"></i> Focus Areas</h3>
                            <ul class="text-gray-400">
                                <li class="mb-1">• Penetration Testing</li>
                                <li class="mb-1">• Malware Analysis</li>
                                <li>• Vulnerability Research</li>
                            </ul>
                        </div>
                        
                        <div class="bg-gray-900 p-4 rounded-lg border-l-4 border-teal-400">
                            <h3 class="font-bold text-white mb-2"><i class="fas fa-graduation-cap text-teal-400 mr-2"></i> Education</h3>
                            <p class="text-gray-400 mb-1">Cybersecurity Engineering</p>
                            <p class="text-teal-400 text-sm">TEK-UP University</p>
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
                <h2 class="text-3xl font-bold text-white mb-4">
                    <span class="border-b-2 border-teal-400 pb-2">Technical Skills</span>
                </h2>
                <p class="text-gray-400 max-w-2xl mx-auto">
                    My skill set spans across offensive and defensive security domains, with hands-on experience in various tools and technologies.
                </p>
            </div>
            
            <div class="grid md:grid-cols-2 gap-12 items-center mb-16">
                <div>
                    <canvas id="skillsChart" height="400"></canvas>
                </div>
                
                <div>
                    <h3 class="text-xl font-bold text-white mb-6">Core Competencies</h3>
                    
                    <div class="grid grid-cols-2 gap-4">
                        <div class="bg-gray-800 p-4 rounded-lg">
                            <div class="text-teal-400 mb-2">
                                <i class="fas fa-shield-alt text-2xl"></i>
                            </div>
                            <h4 class="font-bold text-white mb-2">Offensive Security</h4>
                            <p class="text-gray-400 text-sm">
                                Penetration testing, vulnerability assessment, and exploitation techniques.
                            </p>
                        </div>
                        
                        <div class="bg-gray-800 p-4 rounded-lg">
                            <div class="text-teal-400 mb-2">
                                <i class="fas fa-search text-2xl"></i>
                            </div>
                            <h4 class="font-bold text-white mb-2">Malware Analysis</h4>
                            <p class="text-gray-400 text-sm">
                                Static and dynamic analysis of malicious software samples.
                            </p>
                        </div>
                        
                        <div class="bg-gray-800 p-4 rounded-lg">
                            <div class="text-teal-400 mb-2">
                                <i class="fas fa-network-wired text-2xl"></i>
                            </div>
                            <h4 class="font-bold text-white mb-2">Network Security</h4>
                            <p class="text-gray-400 text-sm">
                                Traffic analysis, intrusion detection, and secure architecture design.
                            </p>
                        </div>
                        
                        <div class="bg-gray-800 p-4 rounded-lg">
                            <div class="text-teal-400 mb-2">
                                <i class="fas fa-laptop-code text-2xl"></i>
                            </div>
                            <h4 class="font-bold text-white mb-2">Secure Coding</h4>
                            <p class="text-gray-400 text-sm">
                                Developing applications with security best practices in mind.
                            </p>
                        </div>
                    </div>
                </div>
            </div>
            
            <div>
                <h3 class="text-xl font-bold text-white mb-6">Tools & Technologies</h3>
                
                <div class="flex flex-wrap gap-3">
                    <span class="skill-badge bg-gray-800 text-teal-400 px-4 py-2 rounded-full">Metasploit</span>
                    <span class="skill-badge bg-gray-800 text-teal-400 px-4 py-2 rounded-full">Burp Suite</span>
                    <span class="skill-badge bg-gray-800 text-teal-400 px-4 py-2 rounded-full">Wireshark</span>
                    <span class="skill-badge bg-gray-800 text-teal-400 px-4 py-2 rounded-full">Ghidra</span>
                    <span class="skill-badge bg-gray-800 text-teal-400 px-4 py-2 rounded-full">Nmap</span>
                    <span class="skill-badge bg-gray-800 text-teal-400 px-4 py-2 rounded-full">Python</span>
                    <span class="skill-badge bg-gray-800 text-teal-400 px-4 py-2 rounded-full">Kali Linux</span>
                    <span class="skill-badge bg-gray-800 text-teal-400 px-4 py-2 rounded-full">Docker</span>
                    <span class="skill-badge bg-gray-800 text-teal-400 px-4 py-2 rounded-full">OWASP ZAP</span>
                    <span class="skill-badge bg-gray-800 text-teal-400 px-4 py-2 rounded-full">ELK Stack</span>
                    <span class="skill-badge bg-gray-800 text-teal-400 px-4 py-2 rounded-full">Git</span>
                    <span class="skill-badge bg-gray-800 text-teal-400 px-4 py-2 rounded-full">Bash</span>
                </div>
            </div>
        </div>
    </section>

    <!-- Projects Section -->
    <section id="projects" class="py-20 bg-gray-800/50">
        <div class="container mx-auto px-6">
            <div class="text-center mb-16">
                <h2 class="text-3xl font-bold text-white mb-4">
                    <span class="border-b-2 border-teal-400 pb-2">Featured Projects</span>
                </h2>
                <p class="text-gray-400 max-w-2xl mx-auto">
                    Hands-on security projects demonstrating my technical skills and problem-solving approach.
                </p>
            </div>
            
            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Project 1 -->
                <div class="project-card bg-gray-900 rounded-lg overflow-hidden shadow-lg">
                    <div class="p-6">
                        <div class="flex items-center mb-4">
                            <div class="bg-teal-400/10 p-3 rounded-full mr-4">
                                <i class="fas fa-bug text-teal-400"></i>
                            </div>
                            <h3 class="text-xl font-bold text-white">Zus Trojan Analysis</h3>
                        </div>
                        <p class="text-gray-400 mb-4">
                            In-depth analysis of banking malware including behavior, evasion techniques, and detection rules.
                        </p>
                        <div class="flex flex-wrap gap-2 mb-4">
                            <span class="bg-gray-800 text-teal-400 text-xs px-3 py-1 rounded-full">Ghidra</span>
                            <span class="bg-gray-800 text-teal-400 text-xs px-3 py-1 rounded-full">Wireshark</span>
                            <span class="bg-gray-800 text-teal-400 text-xs px-3 py-1 rounded-full">YARA</span>
                        </div>
                        <a href="#" class="text-teal-400 hover:text-teal-300 font-medium inline-flex items-center">
                            Read Case Study <i class="fas fa-arrow-right ml-2"></i>
                        </a>
                    </div>
                </div>
                
                <!-- Project 2 -->
                <div class="project-card bg-gray-900 rounded-lg overflow-hidden shadow-lg">
                    <div class="p-6">
                        <div class="flex items-center mb-4">
                            <div class="bg-teal-400/10 p-3 rounded-full mr-4">
                                <i class="fas fa-lock text-teal-400"></i>
                            </div>
                            <h3 class="text-xl font-bold text-white">Secure Facial Recognition</h3>
                        </div>
                        <p class="text-gray-400 mb-4">
                            Privacy-focused facial recognition system with GDPR compliance and secure data handling.
                        </p>
                        <div class="flex flex-wrap gap-2 mb-4">
                            <span class="bg-gray-800 text-teal-400 text-xs px-3 py-1 rounded-full">Python</span>
                            <span class="bg-gray-800 text-teal-400 text-xs px-3 py-1 rounded-full">OpenCV</span>
                            <span class="bg-gray-800 text-teal-400 text-xs px-3 py-1 rounded-full">Docker</span>
                        </div>
                        <a href="#" class="text-teal-400 hover:text-teal-300 font-medium inline-flex items-center">
                            View Details <i class="fas fa-arrow-right ml-2"></i>
                        </a>
                    </div>
                </div>
                
                <!-- Project 3 -->
                <div class="project-card bg-gray-900 rounded-lg overflow-hidden shadow-lg">
                    <div class="p-6">
                        <div class="flex items-center mb-4">
                            <div class="bg-teal-400/10 p-3 rounded-full mr-4">
                                <i class="fas fa-user-graduate text-teal-400"></i>
                            </div>
                            <h3 class="text-xl font-bold text-white">eJPT Training Program</h3>
                        </div>
                        <p class="text-gray-400 mb-4">
                            Developed and led a training curriculum to prepare students for eJPT certification.
                        </p>
                        <div class="flex flex-wrap gap-2 mb-4">
                            <span class="bg-gray-800 text-teal-400 text-xs px-3 py-1 rounded-full">Metasploit</span>
                            <span class="bg-gray-800 text-teal-400 text-xs px-3 py-1 rounded-full">Nmap</span>
                            <span class="bg-gray-800 text-teal-400 text-xs px-3 py-1 rounded-full">CTF</span>
                        </div>
                        <a href="#" class="text-teal-400 hover:text-teal-300 font-medium inline-flex items-center">
                            See Curriculum <i class="fas fa-arrow-right ml-2"></i>
                        </a>
                    </div>
                </div>
            </div>
            
            <div class="text-center mt-12">
                <a href="https://github.com/ghassencha" target="_blank" class="inline-flex items-center px-6 py-3 border border-teal-400 text-teal-400 rounded-lg hover:bg-teal-400 hover:text-gray-900 transition-colors">
                    <i class="fab fa-github mr-2"></i> View All Projects on GitHub
                </a>
            </div>
        </div>
    </section>

    <!-- Certifications Section -->
    <section id="experience" class="py-20">
        <div class="container mx-auto px-6">
            <div class="text-center mb-16">
                <h2 class="text-3xl font-bold text-white mb-4">
                    <span class="border-b-2 border-teal-400 pb-2">Certifications & Experience</span>
                </h2>
                <p class="text-gray-400 max-w-2xl mx-auto">
                    My professional credentials and hands-on security experience.
                </p>
            </div>
            
            <div class="max-w-4xl mx-auto">
                <!-- Certifications -->
                <div class="mb-12">
                    <h3 class="text-xl font-bold text-white mb-6 flex items-center">
                        <i class="fas fa-certificate text-teal-400 mr-3"></i> Certifications
                    </h3>
                    
                    <div class="space-y-6">
                        <div class="bg-gray-900 p-6 rounded-lg border-l-4 border-teal-400">
                            <div class="flex flex-col sm:flex-row sm:items-center sm:justify-between">
                                <h4 class="text-lg font-bold text-white">eJPT (Junior Penetration Tester)</h4>
                                <span class="text-teal-400 text-sm mt-1 sm:mt-0">INE Security | 2023</span>
                            </div>
                            <p class="text-gray-400 mt-2">
                                Certified in foundational penetration testing skills including network scanning, vulnerability assessment, and exploitation.
                            </p>
                        </div>
                        
                        <div class="bg-gray-900 p-6 rounded-lg border-l-4 border-teal-400">
                            <div class="flex flex-col sm:flex-row sm:items-center sm:justify-between">
                                <h4 class="text-lg font-bold text-white">Blue Team Junior Analyst</h4>
                                <span class="text-teal-400 text-sm mt-1 sm:mt-0">Security Blue Team | 2023</span>
                            </div>
                            <p class="text-gray-400 mt-2">
                                Certified in basic digital forensics, SIEM monitoring, and incident response techniques.
                            </p>
                        </div>
                    </div>
                </div>
                
                <!-- Experience -->
                <div>
                    <h3 class="text-xl font-bold text-white mb-6 flex items-center">
                        <i class="fas fa-briefcase text-teal-400 mr-3"></i> Experience
                    </h3>
                    
                    <div class="space-y-6">
                        <div class="bg-gray-900 p-6 rounded-lg border-l-4 border-teal-400">
                            <div class="flex flex-col sm:flex-row sm:items-center sm:justify-between">
                                <h4 class="text-lg font-bold text-white">Securinets TEK-UP</h4>
                                <span class="text-teal-400 text-sm mt-1 sm:mt-0">CTF Challenge Developer | 2023-Present</span>
                            </div>
                            <p class="text-gray-400 mt-2">
                                Designed and tested Capture The Flag challenges for cybersecurity events, focusing on web security and network exploitation scenarios.
                            </p>
                        </div>
                        
                        <div class="bg-gray-900 p-6 rounded-lg border-l-4 border-teal-400">
                            <div class="flex flex-col sm:flex-row sm:items-center sm:justify-between">
                                <h4 class="text-lg font-bold text-white">eJPT Training Lead</h4>
                                <span class="text-teal-400 text-sm mt-1 sm:mt-0">TEK-UP University | 2023</span>
                            </div>
                            <p class="text-gray-400 mt-2">
                                Organized and led training sessions to prepare students for the eJPT certification, covering penetration testing fundamentals and tools.
                            </p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-20 bg-gray-800/50">
        <div class="container mx-auto px-6">
            <div class="max-w-2xl mx-auto text-center">
                <h2 class="text-3xl font-bold text-white mb-4">
                    <span class="border-b-2 border-teal-400 pb-2">Get In Touch</span>
                </h2>
                <p class="text-gray-400 mb-8">
                    Interested in discussing security research, collaboration opportunities, or potential internships? Feel free to reach out.
                </p>
                
                <div class="flex justify-center space-x-6 mb-8">
                    <a href="https://www.linkedin.com/in/ghassen-challouf/" target="_blank" class="text-gray-400 hover:text-teal-400 text-2xl">
                        <i class="fab fa-linkedin"></i>
                    </a>
                    <a href="https://github.com/ghassencha" target="_blank" class="text-gray-400 hover:text-teal-400 text-2xl">
                        <i class="fab fa-github"></i>
                    </a>
                    <a href="mailto:your.email@example.com" class="text-gray-400 hover:text-teal-400 text-2xl">
                        <i class="fas fa-envelope"></i>
                    </a>
                </div>
                
                <a href="#" class="inline-block bg-teal-600 hover:bg-teal-700 text-white px-8 py-3 rounded-lg font-medium transition-colors">
                    <i class="fas fa-file-download mr-2"></i> Download Resume
                </a>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-900 py-8 border-t border-gray-800">
        <div class="container mx-auto px-6 text-center">
            <p class="text-gray-400">
                &copy; 2024 Ghassen Challouf. All rights reserved.
            </p>
            <p class="text-gray-500 text-sm mt-2">
                Built with <i class="fas fa-heart text-red-400"></i> and <i class="fas fa-coffee text-amber-500"></i>
            </p>
        </div>
    </footer>

    <script>
        document.addEventListener('DOMContentLoaded', function() {
            // Mobile menu toggle
            const mobileMenuButton = document.getElementById('mobile-menu-button');
            const mobileMenu = document.getElementById('mobile-menu');
            
            mobileMenuButton.addEventListener('click', function() {
                mobileMenu.classList.toggle('hidden');
            });
            
            // Close mobile menu when clicking on a link
            const mobileLinks = document.querySelectorAll('#mobile-menu a');
            mobileLinks.forEach(link => {
                link.addEventListener('click', function() {
                    mobileMenu.classList.add('hidden');
                });
            });
            
            // Active navigation highlighting
            const sections = document.querySelectorAll('section');
            const navLinks = document.querySelectorAll('header nav a');
            
            window.addEventListener('scroll', function() {
                let current = '';
                
                sections.forEach(section => {
                    const sectionTop = section.offsetTop;
                    const sectionHeight = section.clientHeight;
                    
                    if (pageYOffset >= sectionTop - 100) {
                        current = section.getAttribute('id');
                    }
                });
                
                navLinks.forEach(link => {
                    link.classList.remove('active-nav', 'text-teal-400');
                    if (link.getAttribute('href').includes(current)) {
                        link.classList.add('active-nav', 'text-teal-400');
                    }
                });
            });
            
            // Skills Radar Chart
            const ctx = document.getElementById('skillsChart').getContext('2d');
            const skillsChart = new Chart(ctx, {
                type: 'radar',
                data: {
                    labels: [
                        'Penetration Testing',
                        'Malware Analysis',
                        'Network Security',
                        'Vulnerability Research',
                        'Digital Forensics',
                        'Secure Coding'
                    ],
                    datasets: [{
                        label: 'Skill Level',
                        data: [85, 75, 80, 85, 70, 65],
                        backgroundColor: 'rgba(79, 209, 197, 0.2)',
                        borderColor: 'rgba(79, 209, 197, 1)',
                        pointBackgroundColor: 'rgba(79, 209, 197, 1)',
                        pointBorderColor: '#fff',
                        pointHoverBackgroundColor: '#fff',
                        pointHoverBorderColor: 'rgba(79, 209, 197, 1)',
                        borderWidth: 2
                    }]
                },
                options: {
                    scales: {
                        r: {
                            angleLines: {
                                color: 'rgba(255, 255, 255, 0.1)'
                            },
                            grid: {
                                color: 'rgba(255, 255, 255, 0.1)'
                            },
                            pointLabels: {
                                color: '#e5e7eb',
                                font: {
                                    size: 12
                                }
                            },
                            ticks: {
                                backdropColor: 'rgba(0, 0, 0, 0)',
                                color: 'rgba(255, 255, 255, 0.5)',
                                stepSize: 20,
                                showLabelBackdrop: false
                            },
                            suggestedMin: 0,
                            suggestedMax: 100
                        }
                    },
                    plugins: {
                        legend: {
                            display: false
                        },
                        tooltip: {
                            callbacks: {
                                label: function(context) {
                                    return context.dataset.label + ': ' + context.raw + '%';
                                }
                            }
                        }
                    },
                    elements: {
                        line: {
                            tension: 0.1
                        }
                    }
                }
            });
            
            // Smooth scrolling for anchor links
            document.querySelectorAll('a[href^="#"]').forEach(anchor => {
                anchor.addEventListener('click', function(e) {
                    e.preventDefault();
                    
                    const targetId = this.getAttribute('href');
                    if (targetId === '#') return;
                    
                    const targetElement = document.querySelector(targetId);
                    if (targetElement) {
                        window.scrollTo({
                            top: targetElement.offsetTop - 80,
                            behavior: 'smooth'
                        });
                    }
                });
            });
        });
    </script>
</body>
</html>
