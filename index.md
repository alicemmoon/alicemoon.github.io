<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Jane Doe - PhD Student</title>
    <!-- Tailwind CSS for styling -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Font Awesome for Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <!-- Google Fonts: Inter -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap" rel="stylesheet">
    
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        sans: ['Inter', 'sans-serif'],
                    },
                    colors: {
                        academic: {
                            50: '#f8f9fa',
                            100: '#e9ecef',
                            500: '#495057',
                            900: '#212529',
                            blue: '#0056b3'
                        }
                    }
                }
            }
        }
    </script>
    <style>
        /* Smooth scrolling for anchor links */
        html { scroll-behavior: smooth; }
        .hover-underline-animation {
            display: inline-block;
            position: relative;
        }
        .hover-underline-animation:after {
            content: '';
            position: absolute;
            width: 100%;
            transform: scaleX(0);
            height: 2px;
            bottom: 0;
            left: 0;
            background-color: #0056b3;
            transform-origin: bottom right;
            transition: transform 0.25s ease-out;
        }
        .hover-underline-animation:hover:after {
            transform: scaleX(1);
            transform-origin: bottom left;
        }
    </style>
</head>
<body class="font-sans text-academic-500 bg-white antialiased selection:bg-academic-blue selection:text-white">

    <!-- Navigation -->
    <nav class="sticky top-0 z-50 bg-white/90 backdrop-blur-sm border-b border-gray-100">
        <div class="max-w-5xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between h-16">
                <div class="flex items-center">
                    <a href="#" class="text-xl font-bold text-academic-900 tracking-tight">Jane Doe</a>
                </div>
                
                <!-- Desktop Menu -->
                <div class="hidden sm:flex items-center space-x-8">
                    <a href="#about" class="text-sm font-medium hover:text-academic-blue transition-colors">About</a>
                    <a href="#news" class="text-sm font-medium hover:text-academic-blue transition-colors">News</a>
                    <a href="#publications" class="text-sm font-medium hover:text-academic-blue transition-colors">Publications</a>
                    <a href="#teaching" class="text-sm font-medium hover:text-academic-blue transition-colors">Teaching</a>
                    <a href="#contact" class="text-sm font-medium hover:text-academic-blue transition-colors">Contact</a>
                </div>

                <!-- Mobile Menu Button -->
                <div class="flex items-center sm:hidden">
                    <button id="mobile-menu-btn" class="text-gray-500 hover:text-gray-700 focus:outline-none">
                        <i class="fas fa-bars text-xl"></i>
                    </button>
                </div>
            </div>
        </div>
        
        <!-- Mobile Menu Panel -->
        <div id="mobile-menu" class="hidden sm:hidden bg-white border-t border-gray-100">
            <div class="px-2 pt-2 pb-3 space-y-1">
                <a href="#about" class="block px-3 py-2 rounded-md text-base font-medium hover:bg-gray-50 text-gray-700">About</a>
                <a href="#news" class="block px-3 py-2 rounded-md text-base font-medium hover:bg-gray-50 text-gray-700">News</a>
                <a href="#publications" class="block px-3 py-2 rounded-md text-base font-medium hover:bg-gray-50 text-gray-700">Publications</a>
                <a href="#teaching" class="block px-3 py-2 rounded-md text-base font-medium hover:bg-gray-50 text-gray-700">Teaching</a>
                <a href="#contact" class="block px-3 py-2 rounded-md text-base font-medium hover:bg-gray-50 text-gray-700">Contact</a>
            </div>
        </div>
    </nav>

    <!-- Main Content -->
    <main class="max-w-5xl mx-auto px-4 sm:px-6 lg:px-8 py-12">
        
        <!-- About Section -->
        <section id="about" class="mb-20 pt-4">
            <div class="flex flex-col md:flex-row gap-10 items-start">
                <div class="w-full md:w-1/3 flex-shrink-0">
                    <!-- Profile Image Placeholder -->
                    <div class="aspect-square rounded-lg bg-gray-200 overflow-hidden relative shadow-sm border border-gray-100">
                        <!-- Instructions: Replace src with your photo URL. -->
                        <img src="/api/placeholder/400/400" alt="Jane Doe" class="object-cover w-full h-full" onerror="this.src='https://ui-avatars.com/api/?name=Jane+Doe&background=random&size=400'">
                    </div>
                    
                    <div class="mt-6 space-y-3">
                        <a href="mailto:janedoe@university.edu" class="flex items-center text-gray-600 hover:text-academic-blue transition-colors">
                            <i class="fas fa-envelope w-6"></i>
                            <span class="text-sm">janedoe@university.edu</span>
                        </a>
                        <a href="#" target="_blank" class="flex items-center text-gray-600 hover:text-academic-blue transition-colors">
                            <i class="fab fa-twitter w-6"></i>
                            <span class="text-sm">@janedoe_phd</span>
                        </a>
                        <a href="#" target="_blank" class="flex items-center text-gray-600 hover:text-academic-blue transition-colors">
                            <i class="fab fa-github w-6"></i>
                            <span class="text-sm">github.com/janedoe</span>
                        </a>
                        <a href="#" target="_blank" class="flex items-center text-gray-600 hover:text-academic-blue transition-colors">
                            <i class="fas fa-graduation-cap w-6"></i>
                            <span class="text-sm">Google Scholar</span>
                        </a>
                        <a href="/cv.pdf" class="inline-flex items-center justify-center w-full mt-4 px-4 py-2 bg-academic-900 text-white text-sm font-medium rounded-md hover:bg-academic-blue transition-colors shadow-sm">
                            Download CV
                        </a>
                    </div>
                </div>

                <div class="w-full md:w-2/3">
                    <h1 class="text-4xl font-bold text-academic-900 mb-2">Jane Doe</h1>
                    <h2 class="text-xl text-academic-blue mb-6 font-medium">PhD Candidate in Computer Science</h2>
                    
                    <div class="prose prose-slate max-w-none text-gray-600 leading-relaxed">
                        <p class="mb-4">
                            Hi! I am a PhD student at the <span class="font-semibold text-gray-900">University of Science</span>, advised by Prof. Alan Turing. 
                            My research interests lie at the intersection of <span class="font-semibold text-gray-900">Machine Learning</span> and <span class="font-semibold text-gray-900">Computational Biology</span>.
                        </p>
                        <p class="mb-4">
                            Currently, I am working on developing interpretable deep learning models for genomic sequence analysis. Before starting my PhD, I completed my B.S. in Mathematics.
                        </p>
                        <p>
                            When I'm not coding, I enjoy hiking, playing chess, and brewing coffee.
                        </p>
                    </div>

                    <div class="mt-8">
                        <h3 class="text-sm font-bold uppercase tracking-wider text-gray-400 mb-3">Interests</h3>
                        <div class="flex flex-wrap gap-2">
                            <span class="px-3 py-1 bg-gray-100 text-gray-700 text-sm rounded-full">Deep Learning</span>
                            <span class="px-3 py-1 bg-gray-100 text-gray-700 text-sm rounded-full">Genomics</span>
                            <span class="px-3 py-1 bg-gray-100 text-gray-700 text-sm rounded-full">Bayesian Inference</span>
                            <span class="px-3 py-1 bg-gray-100 text-gray-700 text-sm rounded-full">Open Science</span>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <hr class="border-gray-100 my-12">

        <!-- News Section -->
        <section id="news" class="mb-20 scroll-mt-24">
            <h2 class="text-2xl font-bold text-academic-900 mb-8 flex items-center">
                News
            </h2>
            <div class="space-y-6">
                <div class="flex gap-4 items-baseline">
                    <span class="text-sm font-mono text-gray-400 w-24 flex-shrink-0">Sep 2024</span>
                    <div>
                        <p class="text-gray-700">One paper accepted to <span class="font-semibold text-gray-900">NeurIPS 2024</span>! See you in Vancouver.</p>
                    </div>
                </div>
                <div class="flex gap-4 items-baseline">
                    <span class="text-sm font-mono text-gray-400 w-24 flex-shrink-0">Jun 2024</span>
                    <div>
                        <p class="text-gray-700">Started a summer internship at <span class="font-semibold text-gray-900">DeepMind</span>.</p>
                    </div>
                </div>
                <div class="flex gap-4 items-baseline">
                    <span class="text-sm font-mono text-gray-400 w-24 flex-shrink-0">Jan 2024</span>
                    <div>
                        <p class="text-gray-700">Passed my qualifying exam!</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Publications Section -->
        <section id="publications" class="mb-20 scroll-mt-24">
            <h2 class="text-2xl font-bold text-academic-900 mb-8">Selected Publications</h2>
            <div class="space-y-8">
                
                <!-- Publication 1 -->
                <div class="group relative pl-4 border-l-2 border-transparent hover:border-academic-blue transition-colors">
                    <h3 class="text-lg font-semibold text-gray-900">
                        <a href="#" class="hover-underline-animation">Understanding Neural Networks in Genomics</a>
                    </h3>
                    <div class="text-gray-600 mt-1">
                        <span class="font-semibold text-gray-900">Jane Doe</span>, John Smith, Alan Turing
                    </div>
                    <div class="text-sm text-gray-500 italic mt-1">
                        Neural Information Processing Systems (NeurIPS), 2024
                    </div>
                    <div class="mt-3 flex gap-3">
                        <a href="#" class="text-xs font-medium px-2 py-1 border border-gray-300 rounded hover:bg-gray-50 text-gray-600 transition-colors"><i class="far fa-file-pdf mr-1"></i> PDF</a>
                        <a href="#" class="text-xs font-medium px-2 py-1 border border-gray-300 rounded hover:bg-gray-50 text-gray-600 transition-colors"><i class="fab fa-github mr-1"></i> Code</a>
                        <a href="#" class="text-xs font-medium px-2 py-1 border border-gray-300 rounded hover:bg-gray-50 text-gray-600 transition-colors">Slides</a>
                    </div>
                </div>

                <!-- Publication 2 -->
                <div class="group relative pl-4 border-l-2 border-transparent hover:border-academic-blue transition-colors">
                    <h3 class="text-lg font-semibold text-gray-900">
                        <a href="#" class="hover-underline-animation">Bayesian Inference for Large Scale Data</a>
                    </h3>
                    <div class="text-gray-600 mt-1">
                        Robert Brown, <span class="font-semibold text-gray-900">Jane Doe</span>
                    </div>
                    <div class="text-sm text-gray-500 italic mt-1">
                        International Conference on Machine Learning (ICML), 2023
                    </div>
                    <div class="mt-3 flex gap-3">
                        <a href="#" class="text-xs font-medium px-2 py-1 border border-gray-300 rounded hover:bg-gray-50 text-gray-600 transition-colors"><i class="far fa-file-pdf mr-1"></i> PDF</a>
                        <a href="#" class="text-xs font-medium px-2 py-1 border border-gray-300 rounded hover:bg-gray-50 text-gray-600 transition-colors"><i class="fab fa-github mr-1"></i> Code</a>
                    </div>
                </div>

            </div>
        </section>

        <!-- Teaching Section -->
        <section id="teaching" class="mb-20 scroll-mt-24">
            <h2 class="text-2xl font-bold text-academic-900 mb-8">Teaching</h2>
            <div class="grid gap-6 md:grid-cols-2">
                <div class="p-6 bg-gray-50 rounded-lg border border-gray-100">
                    <div class="text-sm text-gray-400 font-mono mb-2">Fall 2023</div>
                    <h3 class="font-semibold text-gray-900 mb-1">CS101: Intro to Computer Science</h3>
                    <p class="text-gray-600 text-sm">Graduate Teaching Assistant</p>
                </div>
                <div class="p-6 bg-gray-50 rounded-lg border border-gray-100">
                    <div class="text-sm text-gray-400 font-mono mb-2">Spring 2023</div>
                    <h3 class="font-semibold text-gray-900 mb-1">CS224: Deep Learning</h3>
                    <p class="text-gray-600 text-sm">Guest Lecturer on Transformers</p>
                </div>
            </div>
        </section>

        <!-- Contact Section -->
        <section id="contact" class="scroll-mt-24 mb-12">
            <div class="bg-academic-900 text-gray-300 rounded-2xl p-8 md:p-12 text-center">
                <h2 class="text-2xl font-bold text-white mb-4">Get In Touch</h2>
                <p class="mb-8 max-w-xl mx-auto">
                    I am always open to discussing new research collaborations or opportunities. The best way to reach me is via email.
                </p>
                <a href="mailto:janedoe@university.edu" class="inline-block px-8 py-3 bg-white text-academic-900 font-bold rounded-lg hover:bg-gray-100 transition-colors">
                    Send Email
                </a>
            </div>
        </section>

    </main>

    <footer class="border-t border-gray-100 py-8 mt-12">
        <div class="max-w-5xl mx-auto px-4 sm:px-6 lg:px-8 flex flex-col md:flex-row justify-between items-center">
            <p class="text-sm text-gray-500">© 2024 Jane Doe. All rights reserved.</p>
            <p class="text-sm text-gray-400 mt-2 md:mt-0">Built with HTML & Tailwind CSS</p>
        </div>
    </footer>

    <script>
        // Mobile Menu Toggle
        const btn = document.getElementById('mobile-menu-btn');
        const menu = document.getElementById('mobile-menu');

        btn.addEventListener('click', () => {
            menu.classList.toggle('hidden');
        });

        // Close mobile menu when clicking a link
        document.querySelectorAll('#mobile-menu a').forEach(link => {
            link.addEventListener('click', () => {
                menu.classList.add('hidden');
            });
        });
    </script>
</body>
</html>
