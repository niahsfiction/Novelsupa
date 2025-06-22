<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>NovelVerse Pro | Chat Stories & Community</title>
    
    <!-- Optimized Libraries -->
    <script src="https://cdn.tailwindcss.com?plugins=forms,line-clamp,aspect-ratio"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    
    <!-- Firebase (replace with your config) -->
    <script>
        // Initialize Firebase
        const firebaseConfig = {
            apiKey: "AIzaSyYOUR_API_KEY",
            authDomain: "your-project.firebaseapp.com",
            projectId: "your-project-id",
            storageBucket: "your-bucket.appspot.com",
            messagingSenderId: "1234567890",
            appId: "1:1234567890:web:abcdef123456"
        };
        firebase.initializeApp(firebaseConfig);
    </script>
</head>
<body class="bg-gray-50">
    <!-- App Container -->
    <div class="flex flex-col min-h-screen">
        <!-- Navigation -->
        <nav class="bg-indigo-900 text-white shadow-lg sticky top-0 z-50">
            <div class="container mx-auto px-4 py-3 flex justify-between items-center">
                <div class="flex items-center space-x-2">
                    <i class="fas fa-comments text-2xl"></i>
                    <h1 class="text-2xl font-bold">NovelVerse Pro</h1>
                </div>
                <div class="hidden md:flex items-center space-x-6">
                    <a href="#discover" class="hover:text-indigo-200">Discover</a>
                    <a href="#chat-stories" class="font-semibold text-indigo-100">Chat Stories</a>
                    <a href="#community" class="hover:text-indigo-200">Community</a>
                    <a href="#create" class="hover:text-indigo-200">Create</a>
                </div>
                <div class="flex items-center space-x-4">
                    <button class="p-2 rounded-full hover:bg-indigo-800">
                        <i class="fas fa-search"></i>
                    </button>
                    <button class="p-2 rounded-full hover:bg-indigo-800 relative">
                        <i class="fas fa-bell"></i>
                        <span class="absolute top-0 right-0 bg-red-500 text-white text-xs rounded-full h-5 w-5 flex items-center justify-center">3</span>
                    </button>
                    <button class="w-8 h-8 rounded-full bg-indigo-600 flex items-center justify-center">
                        <i class="fas fa-user"></i>
                    </button>
                </div>
            </div>
        </nav>

        <!-- Mobile Bottom Nav -->
        <div class="md:hidden fixed bottom-0 left-0 right-0 bg-white shadow-lg flex justify-around py-3 z-50">
            <a href="#discover" class="flex flex-col items-center text-indigo-600">
                <i class="fas fa-compass"></i>
                <span class="text-xs mt-1">Discover</span>
            </a>
            <a href="#chat-stories" class="flex flex-col items-center text-indigo-600 font-bold">
                <i class="fas fa-comments"></i>
                <span class="text-xs mt-1">Chat</span>
            </a>
            <a href="#community" class="flex flex-col items-center text-gray-600">
                <i class="fas fa-users"></i>
                <span class="text-xs mt-1">Community</span>
            </a>
            <a href="#create" class="flex flex-col items-center text-gray-600">
                <i class="fas fa-plus-circle"></i>
                <span class="text-xs mt-1">Create</span>
            </a>
        </div>

        <!-- Main Content -->
        <main class="flex-grow container mx-auto px-4 py-6 pb-20 md:pb-6">
            <!-- Chat Stories Section -->
            <section id="chat-stories" class="mb-12">
                <div class="flex justify-between items-center mb-6">
                    <h2 class="text-2xl font-bold">Popular Chat Stories</h2>
                    <a href="#" class="text-indigo-600 hover:text-indigo-800 font-medium">See All</a>
                </div>
                
                <!-- Chat Story Cards -->
                <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-6">
                    <!-- Story 1 -->
                    <div class="bg-white rounded-xl shadow-md overflow-hidden hover:shadow-lg transition">
                        <div class="relative aspect-[4/3] bg-gradient-to-r from-pink-500 to-purple-600">
                            <div class="absolute inset-0 flex items-center justify-center text-white opacity-20">
                                <i class="fas fa-comments text-6xl"></i>
                            </div>
                            <div class="absolute bottom-0 left-0 right-0 bg-gradient-to-t from-black to-transparent p-4">
                                <h3 class="text-white font-bold text-lg">Love in the Office</h3>
                                <div class="flex items-center mt-2">
                                    <div class="w-6 h-6 rounded-full bg-gray-200 mr-2"></div>
                                    <span class="text-white text-sm">Emma_Writes</span>
                                </div>
                            </div>
                            <div class="absolute top-2 right-2 bg-yellow-400 text-xs font-bold px-2 py-1 rounded-full">Premium</div>
                        </div>
                        <div class="p-4">
                            <div class="flex justify-between items-center mb-2">
                                <div class="flex items-center">
                                    <i class="fas fa-heart text-red-500 mr-1"></i>
                                    <span class="text-sm">1.2K</span>
                                </div>
                                <span class="text-sm text-gray-500">Updated 2h ago</span>
                            </div>
                            <div class="flex justify-between">
                                <button class="text-indigo-600 hover:text-indigo-800 text-sm font-medium">Read Now</button>
                                <button class="text-gray-500 hover:text-gray-700 text-sm">100 Chapters</button>
                            </div>
                        </div>
                    </div>
                    
                    <!-- Story 2 -->
                    <div class="bg-white rounded-xl shadow-md overflow-hidden hover:shadow-lg transition">
                        <div class="relative aspect-[4/3] bg-gradient-to-r from-blue-500 to-teal-600">
                            <div class="absolute inset-0 flex items-center justify-center text-white opacity-20">
                                <i class="fas fa-comments text-6xl"></i>
                            </div>
                            <div class="absolute bottom-0 left-0 right-0 bg-gradient-to-t from-black to-transparent p-4">
                                <h3 class="text-white font-bold text-lg">Mystery High School</h3>
                                <div class="flex items-center mt-2">
                                    <div class="w-6 h-6 rounded-full bg-gray-200 mr-2"></div>
                                    <span class="text-white text-sm">AlexMystery</span>
                                </div>
                            </div>
                        </div>
                        <div class="p-4">
                            <div class="flex justify-between items-center mb-2">
                                <div class="flex items-center">
                                    <i class="fas fa-heart text-red-500 mr-1"></i>
                                    <span class="text-sm">856</span>
                                </div>
                                <span class="text-sm text-gray-500">Updated 1d ago</span>
                            </div>
                            <div class="flex justify-between">
                                <button class="text-indigo-600 hover:text-indigo-800 text-sm font-medium">Read Now</button>
                                <button class="text-gray-500 hover:text-gray-700 text-sm">45 Chapters</button>
                            </div>
                        </div>
                    </div>
                    
                    <!-- Story 3 -->
                    <div class="bg-white rounded-xl shadow-md overflow-hidden hover:shadow-lg transition">
                        <div class="relative aspect-[4/3] bg-gradient-to-r from-amber-500 to-red-600">
                            <div class="absolute inset-0 flex items-center justify-center text-white opacity-20">
                                <i class="fas fa-comments text-6xl"></i>
                            </div>
                            <div class="absolute bottom-0 left-0 right-0 bg-gradient-to-t from-black to-transparent p-4">
                                <h3 class="text-white font-bold text-lg">Zombie Apocalypse</h3>
                                <div class="flex items-center mt-2">
                                    <div class="w-6 h-6 rounded-full bg-gray-200 mr-2"></div>
                                    <span class="text-white text-sm">SurvivalGuy</span>
                                </div>
                            </div>
                            <div class="absolute top-2 right-2 bg-yellow-400 text-xs font-bold px-2 py-1 rounded-full">Premium</div>
                        </div>
                        <div class="p-4">
                            <div class="flex justify-between items-center mb-2">
                                <div class="flex items-center">
                                    <i class="fas fa-heart text-red-500 mr-1"></i>
                                    <span class="text-sm">2.4K</span>
                                </div>
                                <span class="text-sm text-gray-500">Updated 3h ago</span>
                            </div>
                            <div class="flex justify-between">
                                <button class="text-indigo-600 hover:text-indigo-800 text-sm font-medium">Read Now</button>
                                <button class="text-gray-500 hover:text-gray-700 text-sm">78 Chapters</button>
                            </div>
                        </div>
                    </div>
                </div>
            </section>

            <!-- Community Section -->
            <section id="community" class="mb-12">
                <div class="flex justify-between items-center mb-6">
                    <h2 class="text-2xl font-bold">Active Communities</h2>
                    <a href="#" class="text-indigo-600 hover:text-indigo-800 font-medium">See All</a>
                </div>
                
                <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
                    <!-- Community 1 -->
                    <div class="bg-white rounded-xl shadow-md overflow-hidden">
                        <div class="relative h-40 bg-gradient-to-r from-purple-500 to-pink-600">
                            <div class="absolute bottom-0 left-0 right-0 bg-gradient-to-t from-black to-transparent p-4">
                                <h3 class="text-white font-bold text-lg">Romance Writers</h3>
                            </div>
                        </div>
                        <div class="p-4">
                            <div class="flex items-center mb-3">
                                <div class="w-10 h-10 rounded-full bg-gray-200 mr-3"></div>
                                <div>
                                    <h4 class="font-medium">Led by Sarah_Love</h4>
                                    <p class="text-xs text-gray-500">12.5K members</p>
                                </div>
                            </div>
                            <p class="text-sm text-gray-600 mb-4">A place for romance writers to share tips and collaborate on projects.</p>
                            <div class="flex justify-between items-center">
                                <button class="px-4 py-2 bg-indigo-600 text-white rounded-lg hover:bg-indigo-700 text-sm">Join</button>
                                <span class="text-xs text-gray-500">45 new posts today</span>
                            </div>
                        </div>
                    </div>
                    
                    <!-- Community 2 -->
                    <div class="bg-white rounded-xl shadow-md overflow-hidden">
                        <div class="relative h-40 bg-gradient-to-r from-blue-500 to-cyan-600">
                            <div class="absolute bottom-0 left-0 right-0 bg-gradient-to-t from-black to-transparent p-4">
                                <h3 class="text-white font-bold text-lg">Chat Story Creators</h3>
                            </div>
                        </div>
                        <div class="p-4">
                            <div class="flex items-center mb-3">
                                <div class="w-10 h-10 rounded-full bg-gray-200 mr-3"></div>
                                <div>
                                    <h4 class="font-medium">Led by ChatMaster</h4>
                                    <p class="text-xs text-gray-500">8.2K members</p>
                                </div>
                            </div>
                            <p class="text-sm text-gray-600 mb-4">Exclusive community for chat story writers to exchange ideas.</p>
                            <div class="flex justify-between items-center">
                                <button class="px-4 py-2 bg-indigo-600 text-white rounded-lg hover:bg-indigo-700 text-sm">Join</button>
                                <span class="text-xs text-gray-500">32 new posts today</span>
                            </div>
                        </div>
                    </div>
                    
                    <!-- Community 3 -->
                    <div class="bg-white rounded-xl shadow-md overflow-hidden">
                        <div class="relative h-40 bg-gradient-to-r from-green-500 to-emerald-600">
                            <div class="absolute bottom-0 left-0 right-0 bg-gradient-to-t from-black to-transparent p-4">
                                <h3 class="text-white font-bold text-lg">Fantasy Worldbuilders</h3>
                            </div>
                        </div>
                        <div class="p-4">
                            <div class="flex items-center mb-3">
                                <div class="w-10 h-10 rounded-full bg-gray-200 mr-3"></div>
                                <div>
                                    <h4 class="font-medium">Led by WorldSmith</h4>
                                    <p class="text-xs text-gray-500">15.3K members</p>
                                </div>
                            </div>
                            <p class="text-sm text-gray-600 mb-4">Creating immersive fantasy worlds together.</p>
                            <div class="flex justify-between items-center">
                                <button class="px-4 py-2 bg-indigo-600 text-white rounded-lg hover:bg-indigo-700 text-sm">Join</button>
                                <span class="text-xs text-gray-500">68 new posts today</span>
                            </div>
                        </div>
                    </div>
                </div>
            </section>

            <!-- Creator Dashboard -->
            <section id="create" class="mb-12">
                <div class="bg-white rounded-xl shadow-md overflow-hidden">
                    <div class="border-b p-4">
                        <h2 class="text-xl font-bold">Creator Dashboard</h2>
                    </div>
                    
                    <div class="grid grid-cols-1 md:grid-cols-4">
                        <!-- Sidebar -->
                        <div class="border-r p-4">
                            <div class="flex items-center mb-6">
                                <div class="w-12 h-12 rounded-full bg-indigo-100 flex items-center justify-center mr-3">
                                    <i class="fas fa-user text-indigo-600"></i>
                                </div>
                                <div>
                                    <h3 class="font-medium">YourWorks</h3>
                                    <p class="text-xs text-gray-500">Creator</p>
                                </div>
                            </div>
                            
                            <nav class="space-y-2">
                                <a href="#" class="block px-3 py-2 bg-indigo-100 text-indigo-700 rounded-lg font-medium">Overview</a>
                                <a href="#" class="block px-3 py-2 hover:bg-gray-100 rounded-lg">Stories</a>
                                <a href="#" class="block px-3 py-2 hover:bg-gray-100 rounded-lg">Analytics</a>
                                <a href="#" class="block px-3 py-2 hover:bg-gray-100 rounded-lg">Earnings</a>
                                <a href="#" class="block px-3 py-2 hover:bg-gray-100 rounded-lg">Schedule</a>
                                <a href="#" class="block px-3 py-2 hover:bg-gray-100 rounded-lg">Settings</a>
                            </nav>
                        </div>
                        
                        <!-- Main Content -->
                        <div class="md:col-span-3 p-6">
                            <!-- Creator Calendar -->
                            <div class="mb-8">
                                <h3 class="font-bold mb-4">Writing Calendar</h3>
                                <div class="bg-gray-50 rounded-lg p-4">
                                    <div class="flex justify-between items-center mb-4">
                                        <h4 class="font-medium">November 2023</h4>
                                        <div class="flex space-x-2">
                                            <button class="p-2 hover:bg-gray-200 rounded-lg">
                                                <i class="fas fa-chevron-left"></i>
                                            </button>
                                            <button class="p-2 hover:bg-gray-200 rounded-lg">
                                                <i class="fas fa-chevron-right"></i>
                                            </button>
                                        </div>
                                    </div>
                                    
                                    <div class="grid grid-cols-7 gap-2 text-center">
                                        <div class="text-xs font-medium text-gray-500 py-2">Sun</div>
                                        <div class="text-xs font-medium text-gray-500 py-2">Mon</div>
                                        <div class="text-xs font-medium text-gray-500 py-2">Tue</div>
                                        <div class="text-xs font-medium text-gray-500 py-2">Wed</div>
                                        <div class="text-xs font-medium text-gray-500 py-2">Thu</div>
                                        <div class="text-xs font-medium text-gray-500 py-2">Fri</div>
                                        <div class="text-xs font-medium text-gray-500 py-2">Sat</div>
                                        
                                        <!-- Calendar Days -->
                                        <div class="py-2"></div>
                                        <div class="py-2"></div>
                                        <div class="py-2"></div>
                                        <div class="py-2 rounded-lg bg-indigo-50 text-indigo-700 font-medium">1</div>
                                        <div class="py-2 rounded-lg">2</div>
                                        <div class="py
