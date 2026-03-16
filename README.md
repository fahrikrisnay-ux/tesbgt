<!DOCTYPE html>
<html lang="en">
<head>
    <base target="_self">
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>TESSSS AJAA</title>
    <meta name="description" content="Nufarm Indonesia provides innovative crop protection solutions, seeds, and agricultural technologies to help farmers increase productivity and sustainability.">
    <meta name="keywords" content="agriculture, crop protection, seeds, farming, Indonesia, pesticides, herbicides, fungicides">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css">
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        'nufarm-green': '#2e7d32',
                        'nufarm-dark-green': '#1b5e20',
                        'nufarm-light-green': '#4caf50',
                        'nufarm-yellow': '#ffc107',
                        'nufarm-orange': '#ff9800',
                        'nufarm-blue': '#2196f3'
                    },
                    fontFamily: {
                        'sans': ['Segoe UI', 'Roboto', 'Arial', 'sans-serif'],
                        'heading': ['Montserrat', 'Segoe UI', 'sans-serif']
                    }
                }
            }
        }
    </script>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;500;600;700&display=swap" rel="stylesheet">
    <style>
        .hero-gradient {
            background: linear-gradient(135deg, rgba(46, 125, 50, 0.9) 0%, rgba(27, 94, 32, 0.9) 100%);
        }
        .card-hover {
            transition: all 0.3s ease;
        }
        .card-hover:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.1);
        }
        .nav-link {
            position: relative;
        }
        .nav-link::after {
            content: '';
            position: absolute;
            width: 0;
            height: 2px;
            bottom: -5px;
            left: 0;
            background-color: #ffc107;
            transition: width 0.3s ease;
        }
        .nav-link:hover::after {
            width: 100%;
        }
    </style>
</head>
<body class="font-sans text-gray-800 bg-gray-50">
    <!-- Header & Navigation -->
    <header class="sticky top-0 z-50 bg-white shadow-md">
        <div class="container mx-auto px-4">
            <div class="flex items-center justify-between py-4">
                <!-- Logo -->
                <div class="flex items-center">
                    <div id="logo-container" class="flex items-center space-x-2">
                        <img src="https://picsum.photos/40?random=100" alt="Nufarm Logo" class="h-10 w-auto">
                        <span class="text-2xl font-bold text-nufarm-green font-heading">Nufarm</span>
                        <span class="text-sm text-gray-600">Indonesia</span>
                    </div>
                </div>

                <!-- Desktop Navigation -->
                <nav class="hidden lg:block">
                    <ul id="main-nav" class="flex space-x-8"></ul>
                </nav>

                <!-- Language & Search -->
                <div class="flex items-center space-x-4">
                    <div class="hidden md:block">
                        <select id="language-select" class="border border-gray-300 rounded px-3 py-1 text-sm focus:outline-none focus:ring-2 focus:ring-nufarm-green">
                            <option value="id">ID</option>
                            <option value="en">EN</option>
                        </select>
                    </div>
                    <button id="search-toggle" class="text-gray-600 hover:text-nufarm-green">
                        <i class="fas fa-search"></i>
                    </button>
                    <button id="mobile-menu-toggle" class="lg:hidden text-gray-600 hover:text-nufarm-green">
                        <i class="fas fa-bars text-xl"></i>
                    </button>
                </div>
            </div>

            <!-- Search Bar -->
            <div id="search-bar" class="hidden py-4 border-t">
                <div class="relative">
                    <input type="text" placeholder="Search products, solutions, or resources..." 
                           class="w-full px-4 py-3 pl-12 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-nufarm-green">
                    <i class="fas fa-search absolute left-4 top-1/2 transform -translate-y-1/2 text-gray-400"></i>
                </div>
            </div>
        </div>

        <!-- Mobile Navigation -->
        <div id="mobile-nav" class="hidden lg:hidden bg-white border-t">
            <ul id="mobile-nav-list" class="py-4"></ul>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="relative bg-gray-900 text-white">
        <img src="https://picsum.photos/1920/600?random=1" alt="Agricultural field with crops" 
             class="w-full h-64 md:h-96 object-cover opacity-70">
        <div class="absolute inset-0 hero-gradient flex items-center">
            <div class="container mx-auto px-4">
                <div class="max-w-2xl">
                    <h1 class="text-3xl md:text-5xl font-bold mb-4 font-heading">Growing Together with Indonesian Agriculture</h1>
                    <p class="text-lg md:text-xl mb-8 opacity-90">Innovative crop protection solutions for sustainable farming and increased productivity.</p>
                    <div class="flex flex-wrap gap-4">
                        <button id="explore-products" class="bg-nufarm-yellow text-nufarm-dark-green font-semibold px-6 py-3 rounded-lg hover:bg-yellow-500 transition">
                            Explore Our Products
                        </button>
                        <button id="contact-sales" class="bg-transparent border-2 border-white text-white font-semibold px-6 py-3 rounded-lg hover:bg-white hover:text-nufarm-dark-green transition">
                            Contact Sales
                        </button>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Main Content -->
    <main>
        <!-- Products Section -->
        <section class="py-16 bg-white">
            <div class="container mx-auto px-4">
                <div class="text-center mb-12">
                    <h2 class="text-3xl md:text-4xl font-bold text-nufarm-dark-green mb-4 font-heading">Our Product Categories</h2>
                    <p class="text-gray-600 max-w-2xl mx-auto">Comprehensive range of agricultural solutions for every stage of crop development</p>
                </div>
                <div id="product-categories" class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6"></div>
            </div>
        </section>

        <!-- Solutions Section -->
        <section class="py-16 bg-gray-50">
            <div class="container mx-auto px-4">
                <div class="text-center mb-12">
                    <h2 class="text-3xl md:text-4xl font-bold text-nufarm-dark-green mb-4 font-heading">Agricultural Solutions</h2>
                    <p class="text-gray-600 max-w-2xl mx-auto">Tailored solutions for different crops and farming challenges</p>
                </div>
                <div id="solutions-grid" class="grid grid-cols-1 lg:grid-cols-3 gap-8"></div>
            </div>
        </section>

        <!-- Featured Products -->
        <section class="py-16 bg-white">
            <div class="container mx-auto px-4">
                <div class="flex justify-between items-center mb-12">
                    <div>
                        <h2 class="text-3xl md:text-4xl font-bold text-nufarm-dark-green mb-2 font-heading">Featured Products</h2>
                        <p class="text-gray-600">Latest innovations in crop protection</p>
                    </div>
                    <button id="view-all-products" class="text-nufarm-green font-semibold hover:text-nufarm-dark-green flex items-center">
                        View All Products <i class="fas fa-arrow-right ml-2"></i>
                    </button>
                </div>
                <div id="featured-products" class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6"></div>
            </div>
        </section>

        <!-- News & Updates -->
        <section class="py-16 bg-gray-50">
            <div class="container mx-auto px-4">
                <div class="text-center mb-12">
                    <h2 class="text-3xl md:text-4xl font-bold text-nufarm-dark-green mb-4 font-heading">Latest News & Updates</h2>
                    <p class="text-gray-600 max-w-2xl mx-auto">Stay informed about agricultural innovations, events, and industry insights</p>
                </div>
                <div id="news-grid" class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8"></div>
            </div>
        </section>

        <!-- Contact CTA -->
        <section class="py-16 bg-nufarm-green text-white">
            <div class="container mx-auto px-4">
                <div class="max-w-3xl mx-auto text-center">
                    <h2 class="text-3xl md:text-4xl font-bold mb-6 font-heading">Need Agricultural Solutions?</h2>
                    <p class="text-xl mb-8 opacity-90">Our team of experts is ready to help you find the right products for your farming needs.</p>
                    <div class="flex flex-col sm:flex-row gap-4 justify-center">
                        <button id="contact-expert" class="bg-white text-nufarm-dark-green font-semibold px-8 py-4 rounded-lg hover:bg-gray-100 transition text-lg">
                            <i class="fas fa-user-tie mr-2"></i> Contact Our Expert
                        </button>
                        <button id="download-catalog" class="bg-transparent border-2 border-white text-white font-semibold px-8 py-4 rounded-lg hover:bg-white hover:text-nufarm-dark-green transition text-lg">
                            <i class="fas fa-download mr-2"></i> Download Product Catalog
                        </button>
                    </div>
                </div>
            </div>
        </section>
    </main>

    <!-- Footer -->
    <footer class="bg-gray-900 text-white">
        <div class="container mx-auto px-4 py-12">
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-8">
                <!-- Company Info -->
                <div>
                    <div class="flex items-center space-x-2 mb-6">
                        <img src="https://picsum.photos/40?random=101" alt="Nufarm Logo" class="h-10 w-auto">
                        <span class="text-2xl font-bold font-heading">Nufarm</span>
                    </div>
                    <p class="text-gray-400 mb-6">Providing innovative agricultural solutions to farmers across Indonesia since 1995.</p>
                    <div id="social-links" class="flex space-x-4"></div>
                </div>

                <!-- Quick Links -->
                <div>
                    <h3 class="text-lg font-bold mb-6 font-heading">Quick Links</h3>
                    <ul id="quick-links" class="space-y-3"></ul>
                </div>

                <!-- Products -->
                <div>
                    <h3 class="text-lg font-bold mb-6 font-heading">Products</h3>
                    <ul id="product-links" class="space-y-3"></ul>
                </div>

                <!-- Contact Info -->
                <div>
                    <h3 class="text-lg font-bold mb-6 font-heading">Contact Us</h3>
                    <ul id="contact-info" class="space-y-4"></ul>
                </div>
            </div>

            <!-- Copyright -->
            <div class="border-t border-gray-800 mt-12 pt-8 text-center text-gray-400">
                <p>&copy; 2024 Nufarm Indonesia. All rights reserved.</p>
                <div id="footer-bottom-links" class="flex justify-center space-x-6 mt-4"></div>
            </div>
        </div>
    </footer>

    <!-- JavaScript -->
    <script>
        // ========== DATA LAYER ==========
        const navigationData = [
            { "label": "Home", "href": "#home", "icon": "fas fa-home" },
            { "label": "Products", "href": "#products", "icon": "fas fa-seedling" },
            { "label": "Solutions", "href": "#solutions", "icon": "fas fa-tractor" },
            { "label": "Resources", "href": "#resources", "icon": "fas fa-book" },
            { "label": "About Us", "href": "#about", "icon": "fas fa-info-circle" },
            { "label": "Contact", "href": "#contact", "icon": "fas fa-envelope" }
        ];

        const productCategories = [
            { 
                "title": "Herbicides", 
                "description": "Effective weed control solutions", 
                "icon": "fas fa-leaf",
                "color": "bg-green-100 text-green-800",
                "image": "https://picsum.photos/400/300?random=2"
            },
            { 
                "title": "Fungicides", 
                "description": "Protect crops from fungal diseases", 
                "icon": "fas fa-biohazard",
                "color": "bg-blue-100 text-blue-800",
                "image": "https://picsum.photos/400/300?random=3"
            },
            { 
                "title": "Insecticides", 
                "description": "Combat pest infestations", 
                "icon": "fas fa-bug",
                "color": "bg-red-100 text-red-800",
                "image": "https://picsum.photos/400/300?random=4"
            },
            { 
                "title": "Seeds", 
                "description": "High-quality hybrid seeds", 
                "icon": "fas fa-seedling",
                "color": "bg-yellow-100 text-yellow-800",
                "image": "https://picsum.photos/400/300?random=5"
            }
        ];

        const solutionsData = [
            {
                "title": "Rice Farming Solutions",
                "description": "Complete protection package for rice cultivation from seedling to harvest.",
                "image": "https://picsum.photos/600/400?random=6",
                "crops": ["Rice", "Paddy"]
            },
            {
                "title": "Palm Oil Plantation",
                "description": "Specialized solutions for palm oil disease and pest management.",
                "image": "https://picsum.photos/600/400?random=7",
                "crops": ["Palm Oil", "Oil Palm"]
            },
            {
                "title": "Vegetable Farming",
                "description": "Safe and effective solutions for vegetable crop protection.",
                "image": "https://picsum.photos/600/400?random=8",
                "crops": ["Tomatoes", "Chilies", "Cabbage"]
            }
        ];

        const featuredProducts = [
            {
                "name": "HerbiShield Pro",
                "category": "Herbicide",
                "description": "Advanced broad-spectrum weed control",
                "image": "https://picsum.photos/300/300?random=9",
                "features": ["Long-lasting", "Rainfast", "Selective"]
            },
            {
                "name": "FungiGuard Plus",
                "category": "Fungicide",
                "description": "Systemic protection against fungal diseases",
                "image": "https://picsum.photos/300/300?random=10",
                "features": ["Preventive", "Curative", "Systemic"]
            },
            {
                "name": "InsectiStop Max",
                "category": "Insecticide",
                "description": "Fast-acting insect pest elimination",
                "image": "https://picsum.photos/300/300?random=11",
                "features": ["Fast-acting", "Broad-spectrum", "Residual"]
            },
            {
                "name": "Hybrid Rice Gold",
                "category": "Seeds",
                "description": "High-yield hybrid rice variety",
                "image": "https://picsum.photos/300/300?random=12",
                "features": ["High yield", "Disease resistant", "Premium quality"]
            }
        ];

        const newsData = [
            {
                "title": "New Sustainable Farming Initiative",
                "date": "March 15, 2024",
                "excerpt": "Nufarm launches new sustainable agriculture program focusing on reduced chemical usage.",
                "image": "https://picsum.photos/400/250?random=13",
                "category": "Sustainability"
            },
            {
                "title": "Rice Farmers Training Workshop",
                "date": "March 10, 2024",
                "excerpt": "Free training workshop for rice farmers on integrated pest management techniques.",
                "image": "https://picsum.photos/400/250?random=14",
                "category": "Events"
            },
            {
                "title": "New Product Registration Approved",
                "date": "March 5, 2024",
                "excerpt": "Government approves new bio-pesticide formulation for organic farming.",
                "image": "https://picsum.photos/400/250?random=15",
                "category": "Products"
            }
        ];

        const quickLinksData = [
            { "label": "About Nufarm", "href": "#about" },
            { "label": "Careers", "href": "#careers" },
            { "label": "Sustainability", "href": "#sustainability" },
            { "label": "Investor Relations", "href": "#investors" },
            { "label": "News & Media", "href": "#news" }
        ];

        const productLinksData = [
            { "label": "Crop Protection", "href": "#crop-protection" },
            { "label": "Seeds", "href": "#seeds" },
            { "label": "Nutrition", "href": "#nutrition" },
            { "label": "Digital Farming", "href": "#digital-farming" },
            { "label": "Product Catalog", "href": "#catalog" }
        ];

        const contactInfoData = [
            { "icon": "fas fa-map-marker-alt", "text": "Jl. Sudirman No. 123, Jakarta 10220, Indonesia" },
            { "icon": "fas fa-phone", "text": "+62 21 1234 5678" },
            { "icon": "fas fa-envelope", "text": "info@nufarm.co.id" },
            { "icon": "fas fa-clock", "text": "Mon-Fri: 8:00 AM - 5:00 PM" }
        ];

        const socialLinksData = [
            { "icon": "fab fa-facebook-f", "href": "#facebook", "label": "Facebook" },
            { "icon": "fab fa-twitter", "href": "#twitter", "label": "Twitter" },
            { "icon": "fab fa-instagram", "href": "#instagram", "label": "Instagram" },
            { "icon": "fab fa-linkedin-in", "href": "#linkedin", "label": "LinkedIn" },
            { "icon": "fab fa-youtube", "href": "#youtube", "label": "YouTube" }
        ];

        const footerBottomLinks = [
            { "label": "Privacy Policy", "href": "#privacy" },
            { "label": "Terms of Use", "href": "#terms" },
            { "label": "Cookie Policy", "href": "#cookies" },
            { "label": "Sitemap", "href": "#sitemap" }
        ];

        // ========== RENDER FUNCTIONS ==========
        function renderNavigation(items) {
            return items.map(item => 
                `<li>
                    <a href="${item.href}" class="nav-link text-gray-700 hover:text-nufarm-green font-medium flex items-center">
                        <i class="${item.icon} mr-2"></i>${item.label}
                    </a>
                </li>`
            ).join("");
        }

        function renderProductCategories(items) {
            return items.map(item => 
                `<div class="card-hover bg-white rounded-xl shadow-md overflow-hidden border border-gray-200">
                    <div class="h-48 overflow-hidden">
                        <img src="${item.image}" alt="${item.title}" class="w-full h-full object-cover hover:scale-105 transition duration-500" loading="lazy">
                    </div>
                    <div class="p-6">
                        <div class="flex items-center mb-4">
                            <div class="${item.color} p-3 rounded-lg mr-4">
                                <i class="${item.icon} text-xl"></i>
                            </div>
                            <h3 class="text-xl font-bold text-gray-800">${item.title}</h3>
                        </div>
                        <p class="text-gray-600 mb-4">${item.description}</p>
                        <a href="#${item.title.toLowerCase()}" class="text-nufarm-green font-semibold hover:text-nufarm-dark-green flex items-center">
                            Learn More <i class="fas fa-arrow-right ml-2"></i>
                        </a>
                    </div>
                </div>`
            ).join("");
        }

        function renderSolutions(items) {
            return items.map(item => 
                `<div class="card-hover bg-white rounded-xl shadow-lg overflow-hidden">
                    <img src="${item.image}" alt="${item.title}" class="w-full h-56 object-cover" loading="lazy">
                    <div class="p-6">
                        <h3 class="text-2xl font-bold text-gray-800 mb-3">${item.title}</h3>
                        <p class="text-gray-600 mb-4">${item.description}</p>
                        <div class="mb-4">
                            <span class="text-sm font-semibold text-gray-700">Suitable for:</span>
                            <div class="flex flex-wrap gap-2 mt-2">
                                ${item.crops.map(crop => `<span class="bg-gray-100 text-gray-700 px-3 py-1 rounded-full text-sm">${crop}</span>`).join("")}
                            </div>
                        </div>
                        <button class="text-nufarm-green font-semibold hover:text-nufarm-dark-green">
                            View Solution Details <i class="fas fa-arrow-right ml-2"></i>
                        </button>
                    </div>
                </div>`
            ).join("");
        }

        function renderFeaturedProducts(items) {
            return items.map(item => 
                `<div class="card-hover bg-white rounded-lg border border-gray-200 overflow-hidden">
                    <div class="h-48 bg-gray-100 flex items-center justify-center">
                        <img src="${item.image}" alt="${item.name}" class="max-h-full max-w-full object-contain p-4" loading="lazy">
                    </div>
                    <div class="p-5">
                        <div class="flex justify-between items-start mb-2">
                            <div>
                                <span class="text-xs font-semibold text-nufarm-green uppercase tracking-wide">${item.category}</span>
                                <h3 class="text-lg font-bold text-gray-800 mt-1">${item.name}</h3>
                            </div>
                            <button class="text-gray-400 hover:text-nufarm-green">
                                <i class="far fa-heart"></i>
                            </button>
                        </div>
                        <p class="text-gray-600 text-sm mb-4">${item.description}</p>
                        <div class="mb-4">
                            ${item.features.map(feature => `<span class="inline-block bg-gray-100 text-gray-700 text-xs px-2 py-1 rounded mr-2 mb-2">${feature}</span>`).join("")}
                        </div>
                        <div class="flex justify-between items-center">
                            <button class="bg-nufarm-green text-white px-4 py-2 rounded-lg text-sm font-semibold hover:bg-nufarm-dark-green transition">
                                Product Details
                            </button>
                            <button class="text-gray-600 hover:text-nufarm-green">
                                <i class="fas fa-share-alt"></i>
                            </button>
                        </div>
                    </div>
                </div>`
            ).join("");
        }

        function renderNews(items) {
            return items.map(item => 
                `<article class="card-hover bg-white rounded-lg overflow-hidden border border-gray-200">
                    <div class="h-48 overflow-hidden">
                        <img src="${item.image}" alt="${item.title}" class="w-full h-full object-cover hover:scale-105 transition duration-500" loading="lazy">
                    </div>
                    <div class="p-6">
                        <div class="flex justify-between items-center mb-3">
                            <span class="text-xs font-semibold text-nufarm-green uppercase tracking-wide">${item.category}</span>
                            <span class="text-sm text-gray-500">${item.date}</span>
                        </div>
                        <h3 class="text-xl font-bold text-gray-800 mb-3 hover:text-nufarm-green cursor-pointer">${item.title}</h3>
                        <p class="text-gray-600 mb-4">${item.excerpt}</p>
                        <a href="#read-more" class="text-nufarm-green font-semibold hover:text-nufarm-dark-green flex items-center">
                            Read More <i class="fas fa-arrow-right ml-2"></i>
                        </a>
                    </div>
                </article>`
            ).join("");
        }

        function renderLinkList(items) {
            return items.map(item => 
                `<li>
                    <a href="${item.href}" class="text-gray-400 hover:text-white transition flex items-center">
                        <i class="fas fa-chevron-right text-xs mr-2"></i>${item.label}
                    </a>
                </li>`
            ).join("");
        }

        function renderContactInfo(items) {
            return items.map(item => 
                `<li class="flex items-start">
                    <i class="${item.icon} text-nufarm-light-green mt-1 mr-3"></i>
                    <span class="text-gray-400">${item.text}</span>
                </li>`
            ).join("");
        }

        function renderSocialLinks(items) {
            return items.map(item => 
                `<a href="${item.href}" aria-label="${item.label}" 
                   class="w-10 h-10 rounded-full bg-gray-800 flex items-center justify-center text-white hover:bg-nufarm-green transition">
                    <i class="${item.icon}"></i>
                </a>`
            ).join("");
        }

        function renderFooterBottomLinks(items) {
            return items.map(item => 
                `<a href="${item.href}" class="text-gray-400 hover:text-white text-sm transition">
                    ${item.label}
                </a>`
            ).join("");
        }

        // ========== INITIALIZATION ==========
        document.addEventListener('DOMContentLoaded', function() {
            // Render navigation
            document.getElementById('main-nav').innerHTML = renderNavigation(navigationData);
            document.getElementById('mobile-nav-list').innerHTML = renderNavigation(navigationData);
            
            // Render product categories
            document.getElementById('product-categories').innerHTML = renderProductCategories(productCategories);
            
            // Render solutions
            document.getElementById('solutions-grid').innerHTML = renderSolutions(solutionsData);
            
            // Render featured products
            document.getElementById('featured-products').innerHTML = renderFeaturedProducts(featuredProducts);
            
            // Render news
            document.getElementById('news-grid').innerHTML = renderNews(newsData);
            
            // Render footer sections
            document.getElementById('quick-links').innerHTML = renderLinkList(quickLinksData);
            document.getElementById('product-links').innerHTML = renderLinkList(productLinksData);
            document.getElementById('contact-info').innerHTML = renderContactInfo(contactInfoData);
            document.getElementById('social-links').innerHTML = renderSocialLinks(socialLinksData);
            document.getElementById('footer-bottom-links').innerHTML = renderFooterBottomLinks(footerBottomLinks);

            // ========== EVENT HANDLERS ==========
            // Mobile menu toggle
            const mobileMenuToggle = document.getElementById('mobile-menu-toggle');
            const mobileNav = document.getElementById('mobile-nav');
            
            mobileMenuToggle.addEventListener('click', function() {
                mobileNav.classList.toggle('hidden');
                const icon = this.querySelector('i');
                if (mobileNav.classList.contains('hidden')) {
                    icon.className = 'fas fa-bars text-xl';
                } else {
                    icon.className = 'fas fa-times text-xl';
                }
            });

            // Search toggle
            const searchToggle = document.getElementById('search-toggle');
            const searchBar = document.getElementById('search-bar');
            
            searchToggle.addEventListener('click', function() {
                searchBar.classList.toggle('hidden');
                if (!searchBar.classList.contains('hidden')) {
                    searchBar.querySelector('input').focus();
                }
            });

            // Language selector
            const languageSelect = document.getElementById('language-select');
            languageSelect.addEventListener('change', function() {
                alert('Language changed to: ' + this.value);
                // In a real implementation, this would trigger a page reload with new language
            });

            // Delegated event handling for all navigation links
            document.addEventListener('click', function(event) {
                const link = event.target.closest('a[href^="#"]');
                if (!link) return;
                
                event.preventDefault();
                const href = link.getAttribute('href');
                
                if (href === '#home') {
                    window.scrollTo({ top: 0, behavior: 'smooth' });
                } else if (href.startsWith('#')) {
                    const target = document.querySelector(href);
                    if (target) {
                        target.scrollIntoView({ behavior: 'smooth', block: 'start' });
                    }
                }
                
                // Close mobile menu if open
                if (!mobileNav.classList.contains('hidden')) {
                    mobileNav.classList.add('hidden');
                    mobileMenuToggle.querySelector('i').className = 'fas fa-bars text-xl';
                }
            });

            // Button event handlers
            const buttons = {
                'explore-products': 'Scrolling to products section...',
                'contact-sales': 'Opening contact form...',
                'view-all-products': 'Loading all products...',
                'contact-expert': 'Opening expert contact form...',
                'download-catalog': 'Starting catalog download...'
            };

            Object.keys(buttons).forEach(buttonId => {
                const button = document.getElementById(buttonId);
                if (button) {
                    button.addEventListener('click', function() {
                        alert(buttons[buttonId]);
                        // In real implementation, these would trigger modals or navigation
                    });
                }
            });

            // Product card interactions
            document.addEventListener('click', function(event) {
                const productCard = event.target.closest('[id^="featured-products"] .card-hover');
                if (productCard) {
                    const productName = productCard.querySelector('h3')?.textContent;
                    if (productName) {
                        alert(`Viewing details for: ${productName}`);
                    }
                }
            });

            // Initialize with some interactive state
            const currentYear = new Date().getFullYear();
            const copyrightElement = document.querySelector('footer .border-t p');
            if (copyrightElement) {
                copyrightElement.textContent = copyrightElement.textContent.replace('2024', currentYear);
            }
        });
    </script>
</body>
</html>
