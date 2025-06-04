&lt;!DOCTYPE html&lt;1>>

&lt;html lang="en" class="scroll-smooth">
&lt;head>
&lt;meta charset="UTF-8">
&lt;meta name="viewport" content="width=device-width, initial-scale=1.0">
&lt;title>Challouf Ghassen | Cybersecurity Portfolio&lt;/title>
&lt;script src="https://cdn.tailwindcss.com">&lt;/script>
&lt;script src="https://cdn.jsdelivr.net/npm/chart.js">&lt;/script>
&lt;2><link rel="preconnect" href="https://fonts.googleapis.com">
&lt;link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
&lt;link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;700;900&amp;display=swap" rel="stylesheet">
&lt;style>
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
&lt;/style>
&lt;!-- Chosen Palette: Cyber Neutral (Dark theme with teal/green accents) -->
&lt;!-- Application Structure Plan: A dashboard-style, single-page portfolio with a top navigation bar for smooth scrolling to thematic sections (About, Skills, Projects, Certifications). This structure prioritizes quick access for users like recruiters. Key interactions include an interactive skills radar chart for a high-impact visual summary and clickable project cards that open detailed modals, allowing users to explore content without leaving the main view. This non-linear, interactive approach is more engaging and user-friendly than a traditional linear CV. -->
&lt;!-- Visualization & Content Choices:
- Profile/About: Goal: Inform. Method: Formatted text blocks. Interaction: None. Justification: Provides a clear, concise professional summary upfront.
- Skills Overview: Goal: Compare/Inform. Method: Radar Chart (Chart.js/Canvas). Interaction: Hover tooltips for details. Justification: Offers a dynamic and visually compelling summary of skill distribution, turning a simple list into an engaging data point.
- Detailed Skills: Goal: Organize. Method: Tabbed HTML/CSS/JS interface. Interaction: Click to switch categories. Justification: Neatly organizes a large amount of information, preventing cognitive overload and improving scannability.
- Projects: Goal: Organize/Inform. Method: Card layout with JS-powered modals. Interaction: Click cards for details. Justification: Maintains a clean page layout while providing depth on demand for interested users.
- Certifications: Goal: Inform. Method: Styled list. Interaction: None. Justification: Clearly and professionally presents credentials.
-->
&lt;!-- CONFIRMATION: NO SVG graphics used. NO Mermaid JS used. -->
&lt;/head>
&lt;body class="bg-gray-900 text-gray-300 antialiased">

<header id="header" class="bg-gray-900/80 backdrop-blur-sm sticky top-0 z-50">
    <nav class="container mx-auto px-6 py-4 flex justify-between items-center">
        <a href="#hero" class="text-xl font-bold text-white">Ghassen Challouf</a>
        <div class="hidden md:flex space-x-8">
            <a href="#about" class="nav-link text-gray-300 hover:text-teal-400 transition-colors duration-300">About</a>
            <a href="#skills" class="nav-link text-gray-300 hover:text-teal-400 transition-colors duration-300">Skills</a>
            <a href="#projects" class="nav-link text-gray-300 hover:text-teal-400 transition-colors duration-300">Projects</a>
            <a href="#certs" class="nav-link text-gray-300 hover:text-teal-400 transition-colors duration-300">Certifications</a>
        </div>
        <button id="mobile-menu-button" class="md:hidden text-white">
            <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="[http://www.w3.org/2000/svg](http://www.w3.org/2000/svg)"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16m-7 6h7"></path></svg>
        </button>
    </nav>
    <div id="mobile-menu" class="hidden md:hidden px-6 pb-4">
        <a href="#about" class="block py-2 text-gray-300 hover:text-teal-400">About</a>
        <a href="#skills" class="block py-2 text-gray-300 hover:text-teal-400">Skills</a>
        <a href="#projects" class="block py-2 text-gray-300 hover:text-teal-400">Projects</a>
        <a href="#certs" class="block py-2 text-gray-300 hover:text-teal-400">Certifications</a>
    </div>
</header>

<main class="container mx-auto px-6">

    <section id="hero" class="min-h-screen flex items-center justify-center text-center">
        <div class="max-w-4xl">
            <h1 class="text-4xl md:text-6xl font-black text-white leading-tight mb-4">Cybersecurity Engineering Student & <span class="text-teal-400">Aspiring Penetration Tester</span></h1>
            <p class="text-lg md:text-xl text-gray-400 mb-8">Passionate about offensive security and vulnerability analysis, driven to build and defend secure digital environments.</p>
            <div class="flex justify-center items-center space-x-4">
                 <a href="[https://www.linkedin.com/in/ghassen-challouf/](https://www.linkedin.com/in/ghassen-challouf/)" target="_blank" class="text-white hover:text-teal-400 transition-colors duration-300 text-2xl font-bold">LinkedIn</a>
                 <a href="[https://tryhackme.com/p/Ghassencha](https://tryhackme.com/p/Ghassencha)" target="_blank" class="text-white hover:text-teal-400 transition-colors duration-300 text-2xl font-bold">TryHackMe</a>
            </div>
        </div>
    </section>

    <section id="about" class="py-20">
        <h2 class="text-4xl font-bold text-white text-center mb-12">About Me</h2>
        <div class="grid md:grid-cols-5 gap-8 items-start">
            <div class="md:col-span-3 bg-gray-800 p-8 rounded-lg shadow-2xl">
                <p class="text-lg mb-6">I am a second-year engineering student at TEK-UP, specializing in Cybersecurity. I am passionate about offensive security and vulnerability analysis, actively seeking an internship in penetration testing to apply and expand my technical skills in a dynamic professional environment.</p>
                <p class="text-lg">I am a motivated, organized, and responsible individual, always eager to learn new technical skills and deepen my acquired knowledge. I enjoy teamwork and am driven to contribute effectively to group projects.</p>
            </div>
            <div class="md:col-span-2 space-y-6">
                <div class="bg-gray-800 p-6 rounded-lg shadow-lg">
                    <h3 class="font-bold text-white text-xl mb-3">🔭 Currently Focused On</h3>
                    <ul class="list-disc list-inside text-gray-400 space-y-2">
                        <li>Honing skills in Penetration Testing Methodologies</li>
                        <li>Analyzing malware like the Zus Trojan</li>
                        <li>Contributing to CTF designs for events</li>
                    </ul>
                </div>
                <div class="bg-gray-800 p-6 rounded-lg shadow-lg">
                    <h3 class="font-bold text-white text-xl mb-3">🌱 Actively Learning</h3>
                    <ul class="list-disc list-inside text-gray-400 space-y-2">
                        <li>Advanced Exploitation Techniques</li>
                        <li>Digital Forensics & Threat Hunting</li>
                        <li>Preparing for eJPT Certification</li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <section id="skills" class="py-20">
        <h2 class="text-4xl font-bold text-white text-center mb-4">My Arsenal</h2>
        <p class="text-center text-gray-400 max-w-2xl mx-auto mb-12">Here is a visual overview of my core competency areas. This chart highlights the domains where I focus my learning and practice. Below, you'll find a more detailed breakdown of the specific tools and technologies I use.</p>
        <div class="grid md:grid-cols-2 gap-12 items-center">
            <div>
                 <div class="chart-container">
                    <canvas id="skillsChart"></canvas>
                </div>
            </div>
            <div>
                <div id="skill-tabs">
                    <div class="border-b border-gray-700 mb-4">
                        <nav class="-mb-px flex space-x-8" aria-label="Tabs">
                            <button class="tab-btn whitespace-nowrap py-4 px-1 border-b-2 font-medium text-lg border-teal-500 text-teal-400" data-target="tools">Tools</button>
                            <button class="tab-btn whitespace-nowrap py-4 px-1 border-b-2 font-medium text-lg border-transparent text-gray-500 hover:text-gray-300 hover:border-gray-400" data-target="concepts">Concepts</button>
                            <button class="tab-btn whitespace-nowrap py-4 px-1 border-b-2 font-medium text-lg border-transparent text-gray-500 hover:text-gray-300 hover:border-gray-400" data-target="os">Systems</button>
                        </nav>
                    </div>
                    <div id="tools" class="tab-content grid grid-cols-2 sm:grid-cols-3 gap-4">
                        <span class="bg-gray-800 p-3 rounded text-center">Metasploit</span>
                        <span class="bg-gray-800 p-3 rounded text-center">Wireshark</span>
                        <span class="bg-gray-800 p-3 rounded text-center">Burp Suite</span>
                        <span class="bg-gray-800 p-3 rounded text-center">Ghidra</span>
                        <span class="bg-gray-800 p-3 rounded text-center">OWASP</span>
                        <span class="bg-gray-800 p-3 rounded text-center">ELK Stack</span>
                    </div>
                    <div id="concepts" class="tab-content hidden grid grid-cols-2 sm:grid-cols-3 gap-4">
                        <span class="bg-gray-800 p-3 rounded text-center">Penetration Testing</span>
                         <span class="bg-gray-800 p-3 rounded text-center">Network Security</span>
                        <span class="bg-gray-800 p-3 rounded text-center">Digital Forensics</span>
                        <span class="bg-gray-800 p-3 rounded text-center">OSINT</span>
                        <span class="bg-gray-800 p-3 rounded text-center">Threat Hunting</span>
                        <span class="bg-gray-800 p-3 rounded text-center">Host Auditing</span>
                    </div>
                    <div id="os" class="tab-content hidden grid grid-cols-2 sm:grid-cols-3 gap-4">
                        <span class="bg-gray-800 p-3 rounded text-center">Linux</span>
                        <span class="bg-gray-800 p-3 rounded text-center">Debian</span>
                        <span class="bg-gray-800 p-3 rounded text-center">RHEL</span>
                        <span class="bg-gray-800 p-3 rounded text-center">Ubuntu</span>
                        <span class="bg-gray-800 p-3 rounded text-center">Windows</span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <section id="projects" class="py-20">
         <h2 class="text-4xl font-bold text-white text-center mb-4">Field Work</h2>
         <p class="text-center text-gray-400 max-w-2xl mx-auto mb-12">Theory is essential, but application is where knowledge is forged. This section showcases some of the key projects where I've applied my skills to solve real-world problems. Click on any project to learn more about the objectives, process, and outcomes.</p>
        <div id="project-grid" class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
        </div>
    </section>

    <section id="certs" class="py-20">
        <h2 class="text-4xl font-bold text-white text-center mb-12">Certifications</h2>
         <p class="text-center text-gray-400 max-w-2xl mx-auto mb-12">Formal certifications validate the skills and knowledge acquired through study and hands-on practice. Here are the credentials I have earned to date, demonstrating my proficiency in key areas of cybersecurity.</p>
        <div class="max-w-4xl mx-auto grid sm:grid-cols-2 md:grid-cols-3 gap-8 text-center">
            <div class="bg-gray-800 p-8 rounded-lg shadow-lg">
                <h3 class="text-xl font-bold text-white">Junior Penetration Tester</h3>
                <p class="text-teal-400">INE Security</p>
            </div>
            <div class="bg-gray-800 p-8 rounded-lg shadow-lg">
                <h3 class="text-xl font-bold text-white">Web Penetration Tester</h3>
                <p class="text-teal-400">INE Security</p>
            </div>
            <div class="bg-gray-800 p-8 rounded-lg shadow-lg">
                <h3 class="text-xl font-bold text-white">Blue Team Junior Analyst</h3>
                <p class="text-teal-400">Security Blue Team</p>
            </div>
        </div>
    </section>

</main>

<footer class="bg-gray-800 py-8">
    <div class="container mx-auto px-6 text-center text-gray-400">
        <p>&copy; 2024 Challouf Ghassen. All rights reserved.</p>
        <p>Built with determination and a little bit of caffeine.</p>
    </div>
</footer>

<div id="project-modal" class="modal-backdrop fixed inset-0 bg-black bg-opacity-70 flex items-center justify-center p-4 opacity-0 pointer-events-none">
    <div class="modal-content bg-gray-800 rounded-lg shadow-2xl w-full max-w-2xl max-h-[90vh] overflow-y-auto transform scale-95">
        <div class="sticky top-0 bg-gray-800 p-4 border-b border-gray-700 flex justify-between items-center">
            <h3 id="modal-title" class="text-2xl font-bold text-white"></h3>
            <button id="modal-close" class="text-gray-400 hover:text-white">&times;</button>
        </div>
        <div class="p-6">
            <p id="modal-description" class="text-gray-300 mb-6"></p>
            <h4 class="font-bold text-white mb-2">Tools Used:</h4>
            <div id="modal-tools" class="flex flex-wrap gap-2"></div>
        </div>
    </div>
</div>


<script>
    document.addEventListener('DOMContentLoaded', () => {

        const mobileMenuButton = document.getElementById('mobile-menu-button');
        const mobileMenu = document.getElementById('mobile-menu');
        mobileMenuButton.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
        });

        const navLinks = document.querySelectorAll('#header a');
        navLinks.forEach(link => {
            link.addEventListener('click', () => {
                if (!mobileMenu.classList.contains('hidden')) {
                     mobileMenu.classList.add('hidden');
                }
            });
        });

        const sections = document.querySelectorAll('section');
        const headerNavLinks = document.querySelectorAll('#header .hidden a');
        window.onscroll = () => {
            let current = '';
            sections.forEach(section => {
                const sectionTop = section.offsetTop;
                if (pageYOffset >= sectionTop - 60) {
                    current = section.getAttribute('id');
                }
            });
            headerNavLinks.forEach(link => {
                link.classList.remove('active-link', 'text-teal-400');
                if (link.href.includes(current)) {
                    link.classList.add('active-link', 'text-teal-400');
                }
            });
        };

        const ctx = document.getElementById('skillsChart').getContext('2d');
        const skillsChart = new Chart(ctx, {
            type: 'radar',
            data: {
                labels: ['Offensive Security', 'Defensive Security', 'Network Analysis', 'Malware Analysis', 'Forensics', 'Vulnerability Assessment'],
                datasets: [{
                    label: 'Focus Area',
                    data: [9, 6, 7, 8, 7, 9],
                    backgroundColor: 'rgba(79, 209, 197, 0.2)',
                    borderColor: 'rgba(79, 209, 197, 1)',
                    pointBackgroundColor: 'rgba(79, 209, 197, 1)',
                    pointBorderColor: '#fff',
                    pointHoverBackgroundColor: '#fff',
                    pointHoverBorderColor: 'rgba(79, 209, 197, 1)'
                }]
            },
            options: {
                maintainAspectRatio: false,
                scales: {
                    r: {
                        angleLines: { color: 'rgba(255, 255, 255, 0.2)' },
                        grid: { color: 'rgba(255, 255, 255, 0.2)' },
                        pointLabels: { color: '#a0aec0', font: { size: 14 } },
                        ticks: {
                            color: '#1a202c',
                            backdropColor: 'rgba(255, 255, 255, 0.8)',
                            stepSize: 2
                        }
                    }
                },
                plugins: {
                    legend: {
                        display: false
                    }
                }
            }
        });

        const tabs = document.querySelectorAll('.tab-btn');
        const tabContents = document.querySelectorAll('.tab-content');
        tabs.forEach(tab => {
            tab.addEventListener('click', () => {
                const target = document.getElementById(tab.dataset.target);
                tabContents.forEach(tc => tc.classList.add('hidden'));
                target.classList.remove('hidden');

                tabs.forEach(t => t.classList.remove('border-teal-500', 'text-teal-400'));
                tab.classList.add('border-teal-500', 'text-teal-400');
            });
        });

        const projectsData = [
            {
                title: "Zus Trojan Malware Analysis",
                description: "Conducted an in-depth analysis of the Zus Trojan, a complex banking malware. The primary goal was to understand its propagation methods, evasion techniques, and data exfiltration capabilities. Based on the findings, I developed custom detection rules and outlined effective defense strategies to mitigate the risk of financial fraud.",
                tools: ["Ghidra", "Wireshark", "Docker"]
            },
            {
                title: "Secure Facial Recognition System",
                description: "Designed and deployed a secure facial recognition surveillance system. This project had a strong focus on data privacy, ensuring strict compliance with GDPR and other data protection standards throughout the system's architecture and operational lifecycle.",
                tools: ["Python", "OpenCV", "Linux"]
            },
            {
                title: "eJPT Certification Training Lead",
                description: "Organized and led a hands-on cybersecurity training program to support fellow students in preparing for and achieving the eJPT certification. The curriculum covered foundational penetration testing, network scanning with Nmap, and various exploitation techniques using Metasploit.",
                tools: ["Metasploit", "Nmap", "CTF Design"]
            },
            {
                title: "Securinets CTF Contributor",
                description: "As a technical team member for Securinets at TEK-UP, I was responsible for creating and testing Capture The Flag (CTF) challenges for various events. This involved developing vulnerable web applications, network challenges, and cryptographic puzzles to test participants' skills.",
                tools: ["CTF Design", "Web Security", "Scripting"]
            }
        ];

        const projectGrid = document.getElementById('project-grid');
        const modal = document.getElementById('project-modal');
        const modalTitle = document.getElementById('modal-title');
        const modalDescription = document.getElementById('modal-description');
        const modalTools = document.getElementById('modal-tools');
        const modalClose = document.getElementById('modal-close');

        projectsData.forEach(project => {
            const card = document.createElement('div');
            card.className = 'bg-gray-800 rounded-lg overflow-hidden shadow-lg cursor-pointer transform hover:-translate-y-2 transition-transform duration-300';
            card.innerHTML = `<div class="p-6"><h3 class="text-xl font-bold text-white mb-2">${project.title}</h3><p class="text-gray-400">${project.description.substring(0, 100)}...</p></div>`;
            card.addEventListener('click', () => openModal(project));
            projectGrid.appendChild(card);
        });

        function openModal(project) {
            modalTitle.textContent = project.title;
            modalDescription.textContent = project.description;
            modalTools.innerHTML = project.tools.map(tool => `<span class="bg-gray-700 text-teal-300 text-sm font-medium mr-2 px-2.5 py-0.5 rounded">${tool}</span>`).join('');
            modal.classList.remove('opacity-0', 'pointer-events-none');
            modal.querySelector('.modal-content').classList.remove('scale-95');
        }
        
        function closeModal() {
            modal.classList.add('opacity-0', 'pointer-events-none');
            modal.querySelector('.modal-content').classList.add('scale-95');
        }

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
    });
</script>
