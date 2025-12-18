<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Need It Take It - Premium AI Tools Library</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        primary: '#0f172a',
                        secondary: '#1e293b',
                        accent: '#8b5cf6',
                        neon: '#00ff9d',
                        gradientStart: '#7e22ce',
                        gradientEnd: '#3b82f6'
                    }
                }
            }
        }
    </script>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&display=swap');
        
        body {
            font-family: 'Inter', sans-serif;
            background: linear-gradient(135deg, #0f172a 0%, #1e293b 100%);
            color: #e2e8f0;
            min-height: 100vh;
            position: relative;
            overflow-x: hidden;
        }
        
        body::after {
            content: "TakeThis";
            position: fixed;
            bottom: 20px;
            right: 20px;
            font-size: 1.2rem;
            opacity: 0.15;
            color: #8b5cf6;
            font-weight: 900;
            z-index: 0;
            pointer-events: none;
        }
        
        .watermark {
            position: fixed;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            display: flex;
            align-items: center;
            justify-content: center;
            pointer-events: none;
            font-size: 20rem;
            font-weight: bold;
            opacity: 0.02;
            z-index: -1;
            transform: rotate(-45deg);
            color: #00ff9d;
            font-family: monospace;
        }
        
        .card-hover {
            transition: all 0.3s ease;
            border: 1px solid rgba(139, 92, 246, 0.2);
        }
        
        .card-hover:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(139, 92, 246, 0.3);
            border-color: rgba(139, 92, 246, 0.4);
        }
        
        .glow {
            box-shadow: 0 0 15px rgba(139, 92, 246, 0.5);
        }
        
        .gradient-bg {
            background: linear-gradient(90deg, #7e22ce 0%, #3b82f6 100%);
        }
        
        .typewriter {
            overflow: hidden;
            border-right: 0.15em solid #8b5cf6;
            white-space: nowrap;
            animation: typing 3.5s steps(40, end), blink-caret 0.75s step-end infinite;
        }
        
        @keyframes typing {
            from { width: 0 }
            to { width: 100% }
        }
        
        @keyframes blink-caret {
            from, to { border-color: transparent }
            50% { border-color: #8b5cf6 }
        }
        
        .pagination-btn {
            transition: all 0.3s ease;
        }
        
        .pagination-btn:hover {
            background: linear-gradient(90deg, #7e22ce 0%, #3b82f6 100%);
            transform: scale(1.05);
        }
        
        .tool-card {
            transition: all 0.3s ease;
            background: rgba(30, 41, 59, 0.7);
            backdrop-filter: blur(10px);
        }
        
        .tool-card:hover {
            background: rgba(55, 65, 81, 0.8);
        }
        
        .category-btn {
            transition: all 0.3s ease;
            border: 2px solid transparent;
        }
        
        .category-btn:hover {
            border-color: #8b5cf6;
            transform: translateY(-3px);
        }
        
        .category-btn.active {
            background: linear-gradient(90deg, #7e22ce 0%, #3b82f6 100%);
        }
        
        .search-input:focus {
            box-shadow: 0 0 0 3px rgba(139, 92, 246, 0.5);
        }
        
        .back-to-top {
            position: fixed;
            bottom: 20px;
            right: 20px;
            opacity: 0;
            transition: all 0.3s ease;
            z-index: 100;
        }
        
        .back-to-top.show {
            opacity: 1;
        }
    </style>
</head>
<body class="min-h-screen">
    <div class="watermark">TakeThis</div>
    
    <!-- Navigation -->
    <nav class="bg-primary border-b border-secondary py-4 sticky top-0 z-50">
        <div class="container mx-auto px-4 flex justify-between items-center">
            <div class="flex items-center">
                <div class="w-10 h-10 rounded-full gradient-bg flex items-center justify-center mr-3 glow">
                    <i class="fas fa-brain text-white"></i>
                </div>
                <h1 class="text-2xl font-bold bg-clip-text text-transparent gradient-bg">
                    Need It <span class="text-neon">Take It</span>
                </h1>
            </div>
            
            <div class="hidden md:flex space-x-6">
                <a href="#featured" class="hover:text-accent transition">Featured</a>
                <a href="#categories" class="hover:text-accent transition">Categories</a>
                <a href="#search" class="hover:text-accent transition">Search</a>
                <a href="#about" class="hover:text-accent transition">About</a>
            </div>
            
            <button class="md:hidden text-xl">
                <i class="fas fa-bars"></i>
            </button>
        </div>
    </nav>
    
    <!-- Hero Section -->
    <section class="py-20 px-4">
        <div class="container mx-auto text-center max-w-4xl">
            <h1 class="text-4xl md:text-6xl font-bold mb-6">
                <span class="block mb-2">Discover Powerful AI Tools</span>
                <span class="typewriter inline-block bg-clip-text text-transparent gradient-bg">That Feel Illegal To Use</span>
            </h1>
            <p class="text-xl text-gray-300 mb-10 max-w-2xl mx-auto">
                Access over 900+ premium AI tools, apps, and resources - completely free. We've curated the most powerful AI resources on the internet that deliver premium results without the price tag.
            </p>
            
            <div class="flex flex-col sm:flex-row justify-center gap-4">
                <a href="#categories" class="px-8 py-3 rounded-full gradient-bg text-white font-bold hover:opacity-90 transition">
                    Explore Tools <i class="ml-2 fas fa-arrow-right"></i>
                </a>
                <a href="#featured" class="px-8 py-3 rounded-full bg-secondary text-white font-bold border border-accent hover:bg-accent/10 transition">
                    View Featured
                </a>
            </div>
        </div>
    </section>
    
    <!-- Stats Section -->
    <section class="py-12 bg-gradient-to-r from-primary to-secondary border-y border-secondary">
        <div class="container mx-auto px-4">
            <div class="grid grid-cols-2 md:grid-cols-4 gap-6">
                <div class="text-center p-6 bg-secondary/50 rounded-xl card-hover">
                    <div class="text-4xl font-bold text-accent mb-2">900+</div>
                    <div class="text-gray-300">AI Tools</div>
                </div>
                <div class="text-center p-6 bg-secondary/50 rounded-xl card-hover">
                    <div class="text-4xl font-bold text-neon mb-2">30+</div>
                    <div class="text-gray-300">Categories</div>
                </div>
                <div class="text-center p-6 bg-secondary/50 rounded-xl card-hover">
                    <div class="text-4xl font-bold text-purple-400 mb-2">24/7</div>
                    <div class="text-gray-300">Updated</div>
                </div>
                <div class="text-center p-6 bg-secondary/50 rounded-xl card-hover">
                    <div class="text-4xl font-bold text-blue-400 mb-2">100%</div>
                    <div class="text-gray-300">Free Access</div>
                </div>
            </div>
        </div>
    </section>
    
    <!-- Featured Tools -->
    <section id="featured" class="py-20 px-4">
        <div class="container mx-auto max-w-6xl">
            <div class="text-center mb-16">
                <h2 class="text-3xl md:text-4xl font-bold mb-4">
                    <span class="gradient-text bg-clip-text text-transparent gradient-bg">Featured AI Tools</span>
                </h2>
                <p class="text-gray-400 max-w-2xl mx-auto">
                    Our top picks of AI tools that deliver premium results completely free
                </p>
            </div>
            
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Tool Cards -->
                <div class="tool-card rounded-xl p-6 card-hover">
                    <div class="flex items-center mb-4">
                        <div class="w-12 h-12 rounded-lg bg-purple-900/30 flex items-center justify-center">
                            <i class="fab fa-google text-purple-400 text-xl"></i>
                        </div>
                        <h3 class="text-xl font-bold ml-4">MagicBriefs</h3>
                    </div>
                    <p class="text-gray-400 mb-6">AI-powered content analysis and summarization tool that works with any document.</p>
                    <a href="https://example.com/magicbriefs" target="_blank" class="text-accent font-semibold hover:underline flex items-center">
                        Visit Website <i class="ml-2 fas fa-external-link-alt text-sm"></i>
                    </a>
                </div>
                
                <div class="tool-card rounded-xl p-6 card-hover">
                    <div class="flex items-center mb-4">
                        <div class="w-12 h-12 rounded-lg bg-blue-900/30 flex items-center justify-center">
                            <i class="fas fa-paint-brush text-blue-400 text-xl"></i>
                        </div>
                        <h3 class="text-xl font-bold ml-4">ArtisanAI</h3>
                    </div>
                    <p class="text-gray-400 mb-6">Generate stunning digital art with advanced AI models completely free.</p>
                    <a href="https://example.com/artisanai" target="_blank" class="text-accent font-semibold hover:underline flex items-center">
                        Visit Website <i class="ml-2 fas fa-external-link-alt text-sm"></i>
                    </a>
                </div>
                
                <div class="tool-card rounded-xl p-6 card-hover">
                    <div class="flex items-center mb-4">
                        <div class="w-12 h-12 rounded-lg bg-green-900/30 flex items-center justify-center">
                            <i class="fas fa-code text-green-400 text-xl"></i>
                        </div>
                        <h3 class="text-xl font-bold ml-4">CodeCraft AI</h3>
                    </div>
                    <p class="text-gray-400 mb-6">Advanced AI assistant for developers that writes and optimizes code.</p>
                    <a href="https://example.com/codecraft" target="_blank" class="text-accent font-semibold hover:underline flex items-center">
                        Visit Website <i class="ml-2 fas fa-external-link-alt text-sm"></i>
                    </a>
                </div>
            </div>
        </div>
    </section>
    
    <!-- Categories -->
    <section id="categories" class="py-20 bg-secondary px-4">
        <div class="container mx-auto max-w-6xl">
            <div class="text-center mb-16">
                <h2 class="text-3xl md:text-4xl font-bold mb-4">
                    <span class="gradient-text bg-clip-text text-transparent gradient-bg">AI Tool Categories</span>
                </h2>
                <p class="text-gray-400 max-w-2xl mx-auto">
                    Explore over 900+ AI tools organized into specialized categories
                </p>
            </div>
            
            <div class="grid grid-cols-2 sm:grid-cols-3 md:grid-cols-4 lg:grid-cols-6 gap-4 mb-12">
                <button class="category-btn bg-primary py-3 px-4 rounded-lg font-medium text-center">
                    Writing
                </button>
                <button class="category-btn bg-primary py-3 px-4 rounded-lg font-medium text-center">
                    Image
                </button>
                <button class="category-btn bg-primary py-3 px-4 rounded-lg font-medium text-center active">
                    Video
                </button>
                <button class="category-btn bg-primary py-3 px-4 rounded-lg font-medium text-center">
                    Audio
                </button>
                <button class="category-btn bg-primary py-3 px-4 rounded-lg font-medium text-center">
                    Code
                </button>
                <button class="category-btn bg-primary py-3 px-4 rounded-lg font-medium text-center">
                    Design
                </button>
                <button class="category-btn bg-primary py-3 px-4 rounded-lg font-medium text-center">
                    Marketing
                </button>
                <button class="category-btn bg-primary py-3 px-4 rounded-lg font-medium text-center">
                    Productivity
                </button>
                <button class="category-btn bg-primary py-3 px-4 rounded-lg font-medium text-center">
                    Research
                </button>
                <button class="category-btn bg-primary py-3 px-4 rounded-lg font-medium text-center">
                    Education
                </button>
                <button class="category-btn bg-primary py-3 px-4 rounded-lg font-medium text-center">
                    Finance
                </button>
                <button class="category-btn bg-primary py-3 px-4 rounded-lg font-medium text-center">
                    Healthcare
                </button>
            </div>
            
            <!-- Search Section -->
            <div id="search" class="mb-16">
                <div class="max-w-2xl mx-auto">
                    <div class="relative">
                        <input 
                            type="text" 
                            class="w-full py-4 px-6 rounded-full bg-primary border border-accent/30 focus:border-accent/50 text-white search-input" 
                            placeholder="Search through 900+ AI tools..."
                        >
                        <button class="absolute right-3 top-1/2 transform -translate-y-1/2 gradient-bg rounded-full w-10 h-10 flex items-center justify-center">
                            <i class="fas fa-search text-white"></i>
                        </button>
                    </div>
                </div>
            </div>
            
            <!-- Tools Grid -->
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Tool cards repeated dynamically -->
                <div class="tool-card rounded-xl p-6 card-hover">
                    <div class="flex items-center mb-4">
                        <div class="w-12 h-12 rounded-lg bg-purple-900/30 flex items-center justify-center">
                            <i class="fas fa-video text-purple-400 text-xl"></i>
                        </div>
                        <h3 class="text-xl font-bold ml-4">VideoMagic AI</h3>
                    </div>
                    <p class="text-gray-400 mb-6">Professional video editing with AI-powered effects and automation.</p>
                    <a href="https://example.com/videomagic" target="_blank" class="text-accent font-semibold hover:underline flex items-center">
                        Visit Website <i class="ml-2 fas fa-external-link-alt text-sm"></i>
                    </a>
                </div>
                
                <div class="tool-card rounded-xl p-6 card-hover">
                    <div class="flex items-center mb-4">
                        <div class="w-12 h-12 rounded-lg bg-blue-900/30 flex items-center justify-center">
                            <i class="fas fa-headphones text-blue-400 text-xl"></i>
                        </div>
                        <h3 class="text-xl font-bold ml-4">AudioForge Pro</h3>
                    </div>
                    <p class="text-gray-400 mb-6">AI-powered audio enhancement and noise removal studio.</p>
                    <a href="https://example.com/audioforge" target="_blank" class="text-accent font-semibold hover:underline flex items-center">
                        Visit Website <i class="ml-2 fas fa-external-link-alt text-sm"></i>
                    </a>
                </div>
                
                <div class="tool-card rounded-xl p-6 card-hover">
                    <div class="flex items-center mb-4">
                        <div class="w-12 h-12 rounded-lg bg-green-900/30 flex items-center justify-center">
                            <i class="fas fa-rocket text-green-400 text-xl"></i>
                        </div>
                        <h3 class="text-xl font-bold ml-4">GrowthAI Suite</h3>
                    </div>
                    <p class="text-gray-400 mb-6">Complete marketing automation with predictive analytics.</p>
                    <a href="https://example.com/growthai" target="_blank" class="text-accent font-semibold hover:underline flex items-center">
                        Visit Website <i class="ml-2 fas fa-external-link-alt text-sm"></i>
                    </a>
                </div>
            </div>
            
            <!-- Pagination -->
            <div class="mt-16 flex justify-center">
                <div class="flex space-x-2">
                    <button class="pagination-btn w-10 h-10 rounded-full bg-primary flex items-center justify-center font-bold">
                        1
                    </button>
                    <button class="pagination-btn w-10 h-10 rounded-full bg-secondary flex items-center justify-center">
                        2
                    </button>
                    <button class="pagination-btn w-10 h-10 rounded-full bg-secondary flex items-center justify-center">
                        3
                    </button>
                    <button class="pagination-btn w-10 h-10 rounded-full bg-secondary flex items-center justify-center">
                        <i class="fas fa-ellipsis-h"></i>
                    </button>
                    <button class="pagination-btn w-10 h-10 rounded-full bg-secondary flex items-center justify-center">
                        30
                    </button>
                </div>
            </div>
        </div>
    </section>
    
    <!-- About Section -->
    <section id="about" class="py-20 px-4">
        <div class="container mx-auto max-w-4xl">
            <div class="text-center mb-16">
                <h2 class="text-3xl md:text-4xl font-bold mb-4">
                    <span class="gradient-text bg-clip-text text-transparent gradient-bg">About This Project</span>
                </h2>
                <p class="text-gray-400 max-w-2xl mx-auto">
                    Why we created this resource for the AI community
                </p>
            </div>
            
            <div class="bg-secondary/50 rounded-2xl p-8 md:p-12">
                <div class="grid grid-cols-1 md:grid-cols-2 gap-8 items-center">
                    <div>
                        <h3 class="text-2xl font-bold mb-4">Our Mission</h3>
                        <p class="text-gray-300 mb-6">
                            At Need It Take It, we believe powerful AI tools should be accessible to everyone. We've spent countless hours discovering and testing AI resources that deliver premium results without the premium price tag.

