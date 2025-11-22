
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Alice Moon | PhD Candidate</title>
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Font Awesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Lato:wght@300;400;700&family=Merriweather:wght@700&display=swap" rel="stylesheet">
    
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        sans: ['Lato', 'sans-serif'],
                        serif: ['Merriweather', 'serif'],
                    },
                    colors: {
                        slate: {
                            850: '#1e293b', // Custom dark sidebar color
                        }
                    }
                }
            }
        }
    </script>
    <style>
        html { scroll-behavior: smooth; }
        /* Mobile menu transition */
        .mobile-menu {
            transition: transform 0.3s ease-in-out;
        }
    </style>
</head>
<body class="bg-white text-gray-700 antialiased">

    <!-- Mobile Header (Visible only on small screens) -->
    <div class="md:hidden flex items-center justify-between p-4 bg-slate-850 text-white fixed w-full z-50 top-0">
        <span class="font-serif font-bold text-lg">Jane Doe</span>
        <button id="mobile-btn" class="text-white hover:text-gray-300">
            <i class="fas fa-bars text-xl"></i>
        </button>
    </div>

    <div class="flex flex-col md:flex-row min-h-screen pt-16 md:pt-0">
        
        <!-- Sidebar (Left side - Fixed on Desktop) -->
        <aside class="w-full md:w-72 bg-slate-850 text-gray-100 flex-shrink-0 md:fixed md:h-screen md:overflow-y-auto z-40 hidden md:block" id="sidebar">
            <div class="p-8 flex flex-col items-center text-center h-full">
                
                <!-- Instructions: Replace src with your photo URL -->
                <div class="w-40 h-40 rounded-full border-4 border-gray-700 overflow-hidden mb-6 shadow-xl relative">
                    <img src="/api/placeholder/400/400" alt="Alice Moon" class="w-full h-full object-cover" onerror="this.src='https://ui-avatars.com/api/?name=Alice+Moon&background=random&size=400'">
                </div>

                <h1 class="text-2xl font-serif font-bold tracking-wide mb-1 text-white">Alice Moon</h1>
                <p class="text-sky-400 text-sm font-medium tracking-wider mb-6">PHD CANDIDATE</p>

                <!-- Navigation -->
                <nav class="w-full space-y-1 mb-8 text-left">
                    <a href="#about" class="block py-2.5 px-4 rounded transition duration-200 hover:bg-gray-700 hover:text-white flex items-center">
                        <i class="fas fa-user w-6 text-center mr-2 text-sm text-gray-400"></i> About
                    </a>
                    <a href="#publications" class="block py-2.5 px-4 rounded transition duration-200 hover:bg-gray-700 hover:text-white flex items-center">
                        <i class="fas fa-book w-6 text-center mr-2 text-sm text-gray-400"></i> Publications
                    </a>
                    <a href="#news" class="block py-2.5 px-4 rounded transition duration-200 hover:bg-gray-700 hover:text-white flex items-center">
                        <i class="fas fa-newspaper w-6 text-center mr-2 text-sm text-gray-400"></i> News
                    </a>
                    <a href="#cv" class="block py-2.5 px-4 rounded transition duration-200 hover:bg-gray-700 hover:text-white flex items-center">
                        <i class="fas fa-file-alt w-6 text-center mr-2 text-sm text-gray-400"></i> CV
                    </a>
                </nav>

                <!-- Footer Socials -->
                <div class="mt-auto w-full pt-6 border-t border-gray-700 flex justify-center space-x-5">
                    <a href="mailto:moon.519@osu.edu" class="text-gray-400 hover:text-white transition"><i class="fas fa-envelope text-lg"></i></a>
                    <a href="#" class="text-gray-400 hover:text-white transition"><i class="fab fa-github text-lg"></i></a>
                    <a href="#" class="text-gray-400 hover:text-white transition"><i class="fab fa-twitter text-lg"></i></a>
                    <a href="#" class="text-gray-400 hover:text-white transition"><i class="fas fa-graduation-cap text-lg"></i></a>
                </div>
            </div>
        </aside>

        <!-- Main Content (Right side) -->
        <main class="flex-1 md:ml-72 p-8 md:p-16 lg:p-24 bg-white">
            
            <!-- About Section -->
            <section id="about" class="max-w-3xl mb-24 scroll-mt-24">
                <h2 class="text-4xl font-serif font-bold text-gray-900 mb-6 border-b-4 border-sky-500 inline-block pb-2">About Me</h2>
                <div class="prose prose-lg text-gray-600 leading-relaxed">
                    <p class="mb-6">
                        Hello! I am a PhD candidate in the Department of Computer Science at the <span class="font-semibold text-gray-900">University of Science</span>. I am fortunate to be advised by <a href="#" class="text-sky-600 hover:underline decoration-2 underline-offset-2">Prof. Alan Turing</a>.
                    </p>
                    <p class="mb-6">
                        My research interests encompass <strong>Machine Learning</strong> and <strong>Genomics</strong>. Specifically, I am interested in building interpretable deep learning models that can uncover new biological insights from large-scale sequencing data.
                    </p>
                    <p>
                        Previously, I obtained my Bachelor's degree in Mathematics. When not doing research, I enjoy long-distance running and photography.
                    </p>
                </div>
                <div class="mt-8">
                    <button class="bg-sky-600 hover:bg-sky-700 text-white font-bold py-2 px-6 rounded shadow transition duration-200">
                        <i class="fas fa-download mr-2"></i> Download Full CV
                    </button>
                </div>
            </section>

            <!-- Publications Section -->
            <section id="publications" class="max-w-4xl mb-24 scroll-mt-24">
                <h2 class="text-3xl font-serif font-bold text-gray-900 mb-8">Selected Publications</h2>
                
                <div class="space-y-12">
                    
                    <!-- Paper 1 -->
                    <div class="flex flex-col sm:flex-row gap-6">
                        <!-- Abstract Thumbnail -->
                        <div class="hidden sm:block w-32 h-24 bg-gray-100 rounded-lg flex-shrink-0 border border-gray-200 flex items-center justify-center text-gray-300">
                           <i class="fas fa-image text-2xl"></i>
                        </div>
                        <div>
                            <h3 class="text-xl font-bold text-gray-800 leading-snug">
                                <a href="#" class="hover:text-sky-600 transition">Deep Learning for Genomic Sequence Analysis</a>
                            </h3>
                            <div class="text-gray-600 mt-2">
                                <span class="font-bold text-gray-900 border-b border-gray-300">Jane Doe</span>, John Smith, Alice Johnson
                            </div>
                            <div class="text-sm text-gray-500 italic mt-1 font-serif">
                                Neural Information Processing Systems (NeurIPS), 2024
                            </div>
                            <div class="flex gap-3 mt-3">
                                <a href="#" class="text-xs font-bold uppercase tracking-wide text-sky-600 hover:bg-sky-50 px-2 py-1 rounded border border-sky-200 transition">PDF</a>
                                <a href="#" class="text-xs font-bold uppercase tracking-wide text-gray-600 hover:bg-gray-100 px-2 py-1 rounded border border-gray-200 transition">Code</a>
                            </div>
                        </div>
                    </div>

                    <!-- Paper 2 -->
                    <div class="flex flex-col sm:flex-row gap-6">
                         <div class="hidden sm:block w-32 h-24 bg-gray-100 rounded-lg flex-shrink-0 border border-gray-200 flex items-center justify-center text-gray-300">
                           <i class="fas fa-chart-line text-2xl"></i>
                        </div>
                        <div>
                            <h3 class="text-xl font-bold text-gray-800 leading-snug">
                                <a href="#" class="hover:text-sky-600 transition">Bayesian Methods for Noisy Data</a>
                            </h3>
                            <div class="text-gray-600 mt-2">
                                Robert Brown, <span class="font-bold text-gray-900 border-b border-gray-300">Jane Doe</span>
                            </div>
                            <div class="text-sm text-gray-500 italic mt-1 font-serif">
                                International Conference on Machine Learning (ICML), 2023
                            </div>
                            <div class="flex gap-3 mt-3">
                                <a href="#" class="text-xs font-bold uppercase tracking-wide text-sky-600 hover:bg-sky-50 px-2 py-1 rounded border border-sky-200 transition">PDF</a>
                                <a href="#" class="text-xs font-bold uppercase tracking-wide text-gray-600 hover:bg-gray-100 px-2 py-1 rounded border border-gray-200 transition">Code</a>
                            </div>
                        </div>
                    </div>

                </div>
            </section>

            <!-- News Section -->
            <section id="news" class="max-w-3xl mb-12 scroll-mt-24">
                <h2 class="text-3xl font-serif font-bold text-gray-900 mb-8">Recent News</h2>
                <div class="border-l-2 border-sky-200 pl-6 space-y-8">
                    
                    <div class="relative">
                        <div class="absolute -left-[31px] top-1 h-4 w-4 rounded-full bg-sky-500 border-2 border-white"></div>
                        <div class="text-sm font-bold text-sky-600 mb-1">September 2024</div>
                        <p class="text-gray-700">One paper accepted to <span class="font-bold">NeurIPS 2024</span>! I will be presenting in Vancouver this winter.</p>
                    </div>

                    <div class="relative">
                        <div class="absolute -left-[31px] top-1 h-4 w-4 rounded-full bg-gray-300 border-2 border-white"></div>
                        <div class="text-sm font-bold text-gray-500 mb-1">June 2024</div>
                        <p class="text-gray-700">Started my summer internship at <span class="font-bold">Google Research</span> working on large language models.</p>
                    </div>

                    <div class="relative">
                        <div class="absolute -left-[31px] top-1 h-4 w-4 rounded-full bg-gray-300 border-2 border-white"></div>
                        <div class="text-sm font-bold text-gray-500 mb-1">January 2024</div>
                        <p class="text-gray-700">Passed my PhD qualifying exam.</p>
                    </div>

                </div>
            </section>

            <footer class="pt-12 mt-12 border-t border-gray-100 text-sm text-gray-400">
                &copy; 2024 Jane Doe. Powered by GitHub Pages.
            </footer>
        </main>
    </div>

    <!-- Mobile Menu Javascript -->
    <script>
        const mobileBtn = document.getElementById('mobile-btn');
        const sidebar = document.getElementById('sidebar');
        
        mobileBtn.addEventListener('click', () => {
            sidebar.classList.toggle('hidden');
            sidebar.classList.toggle('fixed');
            sidebar.classList.toggle('inset-0');
            sidebar.classList.toggle('z-40');
            sidebar.classList.toggle('w-full');
            // Basic toggle for demonstration; in production you'd want a more robust drawer
        });
    </script>
</body>
</html>
