<!DOCTYPE html>
<html lang="id" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bananabites - Ganjal Perut Praktis, Energi Murni Tanpa Telat Kuliah!</title>
    
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    
    <!-- Google Fonts & Font Awesome Icons -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@400;500;600;700;800&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        banana: {
                            100: '#FFFBEB',
                            300: '#FDE047',
                            400: '#FACC15',
                            500: '#EAB308',
                        },
                        cream: '#FFFDF7',
                        choco: {
                            700: '#5A3825',
                            800: '#422617',
                            900: '#2C180E',
                        },
                        gold: '#D97706',
                    },
                    fontFamily: {
                        sans: ['"Plus Jakarta Sans"', 'sans-serif'],
                    }
                }
            }
        }
    </script>
</head>
<body class="bg-cream text-choco-900 font-sans antialiased selection:bg-banana-400 selection:text-choco-900">

    <!-- NAVIGATION BAR -->
    <nav class="sticky top-0 z-40 bg-white/90 backdrop-blur-md border-b border-banana-300/40 shadow-sm">
        <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex items-center justify-between h-16">
                <!-- Logo -->
                <a href="#" class="flex items-center gap-2 font-extrabold text-2xl tracking-tight text-choco-900">
                    <span class="w-9 h-9 bg-banana-400 text-choco-900 rounded-full flex items-center justify-center text-xl shadow-inner">🍌</span>
                    Banana<span class="text-gold">bites</span>
                </a>

                <!-- Desktop Menu -->
                <div class="hidden md:flex items-center space-x-8 font-semibold text-sm">
                    <a href="#masalah" class="hover:text-gold transition-colors">Problem</a>
                    <a href="#solusi" class="hover:text-gold transition-colors">Keunggulan</a>
                    <a href="#produk" class="hover:text-gold transition-colors">Pilihan Varian</a>
                    <a href="#cara-pesan" class="hover:text-gold transition-colors">Cara Pesan</a>
                </div>

                <!-- Cart Icon Button -->
                <button onclick="toggleCart()" class="relative bg-banana-400 hover:bg-banana-500 text-choco-900 px-4 py-2 rounded-full font-bold transition-all shadow-md flex items-center gap-2 active:scale-95">
                    <i class="fa-solid fa-cart-shopping"></i>
                    <span class="hidden sm:inline">Keranjang</span>
                    <span id="cartCount" class="bg-choco-900 text-white text-xs w-5 h-5 rounded-full flex items-center justify-center font-bold">0</span>
                </button>
            </div>
        </div>
    </nav>

    <!-- BANNER HERO SECTION -->
    <section class="relative overflow-hidden bg-gradient-to-b from-banana-100 via-cream to-cream py-12 md:py-20">
        <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-1 md:grid-cols-2 gap-12 items-center">
                
                <!-- Hero Left Column -->
                <div class="space-y-6 text-center md:text-left">
                    <div class="inline-flex items-center gap-2 bg-white border border-banana-400/60 shadow-sm rounded-full px-4 py-1.5 text-xs sm:text-sm font-bold text-choco-800">
                        <span class="bg-red-500 text-white px-2 py-0.5 rounded-full text-[10px] uppercase font-extrabold animate-pulse">PROMO MAHASISWA</span>
                        <span>Mulai Rp 8.000 / Pouch!</span>
                    </div>

                    <h1 class="text-3xl sm:text-4xl md:text-5xl font-extrabold leading-tight text-choco-900">
                        Ganjal Perut Praktis, Energi Murni <span class="bg-gradient-to-r from-banana-500 to-gold bg-clip-text text-transparent">Tanpa Telat Kuliah!</span>
                    </h1>

                    <p class="text-choco-800/80 text-base sm:text-lg leading-relaxed font-medium">
                        <strong>Bananabites</strong> adalah kue kering renyah olahan pisang murni & mentega gurih berbentuk bulat lezat. Diciptakan khusus sebagai solusi sarapan praktis, sehat, dan terjangkau untuk mahasiswa yang terburu-buru mengejar kelas pagi!
                    </p>

                    <div class="flex flex-col sm:flex-row items-center justify-center md:justify-start gap-4 pt-2">
                        <a href="#produk" class="w-full sm:w-auto bg-banana-400 hover:bg-banana-500 text-choco-900 font-extrabold px-8 py-4 rounded-2xl shadow-lg shadow-banana-400/40 hover:shadow-xl transition-all text-center flex items-center justify-center gap-2 active:scale-95">
                            <i class="fa-solid fa-bolt text-choco-900"></i>
                            Pesan Solusi Sarapan Hemat
                        </a>
                        <a href="#masalah" class="w-full sm:w-auto border-2 border-choco-800/20 hover:border-choco-900 text-choco-900 font-bold px-6 py-4 rounded-2xl transition-all text-center">
                            Pelajari Selengkapnya
                        </a>
                    </div>

                    <!-- Micro Social Proof -->
                    <div class="pt-4 flex items-center justify-center md:justify-start gap-6 text-xs text-choco-800/70 font-semibold">
                        <span class="flex items-center gap-1"><i class="fa-solid fa-check-circle text-green-600"></i> Bisa COD Kampus/Kos</span>
                        <span class="flex items-center gap-1"><i class="fa-solid fa-check-circle text-green-600"></i> Fresh Baked Daily</span>
                    </div>
                </div>

                <!-- Hero Right Column (Image Showcase) -->
                <div class="relative">
                    <div class="absolute -top-6 -left-6 w-72 h-72 bg-banana-300 rounded-full filter blur-3xl opacity-50 -z-10"></div>
                    <div class="relative rounded-3xl overflow-hidden shadow-2xl border-4 border-white">
                        <img src="https://images.unsplash.com/photo-1558961363-fa8fdf82db35?auto=format&fit=crop&w=800&q=80" 
                             alt="Bananabites Cookies Pisang Mentega" 
                             class="w-full h-[350px] sm:h-[420px] object-cover hover:scale-105 transition-transform duration-500">
                        <div class="absolute bottom-4 left-4 right-4 bg-white/90 backdrop-blur-md p-4 rounded-2xl shadow-lg border border-white/50 flex items-center gap-4">
                            <img src="https://images.unsplash.com/photo-1528825871115-3581a5387919?auto=format&fit=crop&w=200&q=80" alt="Pisang Segar" class="w-12 h-12 rounded-full object-cover border-2 border-banana-400">
                            <div>
                                <p class="text-xs text-choco-800/70 font-bold">Resep Nutrisi Alami</p>
                                <p class="text-sm font-extrabold text-choco-900">100% Olahan Pisang Murni & Butter</p>
                            </div>
                        </div>
                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- MASALAH YANG DISLESAIKAN -->
    <section id="masalah" class="py-16 bg-white">
        <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-12">
                <h2 class="text-xs font-extrabold uppercase tracking-widest text-gold mb-2">Relatable Buat Anak Kos & Mahasiswa</h2>
                <h3 class="text-2xl sm:text-3xl font-extrabold text-choco-900">Sering Skip Sarapan Gara-Gara Dosen Pagi?</h3>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                <!-- Problem 1 -->
                <div class="bg-banana-100/50 p-6 rounded-3xl border border-banana-300/40 hover:shadow-md transition-all">
                    <div class="w-12 h-12 bg-red-100 text-red-600 rounded-2xl flex items-center justify-center text-xl font-bold mb-4">
                        <i class="fa-solid fa-clock font-bold"></i>
                    </div>
                    <h4 class="font-extrabold text-lg text-choco-900 mb-2">Waktu Mepet Banget</h4>
                    <p class="text-sm text-choco-800/80 leading-relaxed">Bangun tidur langsung buru-buru mandi dan berangkat. Enggak sempat lagi ngantri beli sarapan berat di luar.</p>
                </div>

                <!-- Problem 2 -->
                <div class="bg-banana-100/50 p-6 rounded-3xl border border-banana-300/40 hover:shadow-md transition-all">
                    <div class="w-12 h-12 bg-amber-100 text-amber-600 rounded-2xl flex items-center justify-center text-xl font-bold mb-4">
                        <i class="fa-solid fa-face-frown"></i>
                    </div>
                    <h4 class="font-extrabold text-lg text-choco-900 mb-2">Lemas & Kena Asam Lambung</h4>
                    <p class="text-sm text-choco-800/80 leading-relaxed">Perut kosong pas kuliah bikin fokus buyar, mengantuk, bahkan perut melilit perih kena asam lambung.</p>
                </div>

                <!-- Problem 3 -->
                <div class="bg-banana-100/50 p-6 rounded-3xl border border-banana-300/40 hover:shadow-md transition-all">
                    <div class="w-12 h-12 bg-emerald-100 text-emerald-600 rounded-2xl flex items-center justify-center text-xl font-bold mb-4">
                        <i class="fa-solid fa-wallet"></i>
                    </div>
                    <h4 class="font-extrabold text-lg text-choco-900 mb-2">Sarapan Mahal Bikin Boros</h4>
                    <p class="text-sm text-choco-800/80 leading-relaxed">Beli makanan berat tiap pagi bisa bikin kantong jebol sebelum akhir bulan. Perlu alternatif ganjal perut yang ekonomis!</p>
                </div>
            </div>
        </div>
    </section>

    <!-- SOLUSI & KEUNGGULAN PRODUK -->
    <section id="solusi" class="py-16 bg-cream">
        <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-12">
                <span class="bg-banana-400/30 text-choco-900 px-4 py-1.5 rounded-full text-xs font-extrabold uppercase">Solusi Terbaik Untukmu</span>
                <h2 class="text-3xl font-extrabold text-choco-900 mt-3">Kenapa Harus Bananabites?</h2>
            </div>

            <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-6">
                <!-- Feature 1 -->
                <div class="bg-white p-6 rounded-3xl shadow-sm border border-banana-300/50 hover:-translate-y-1 transition-all">
                    <div class="w-12 h-12 bg-banana-400 text-choco-900 rounded-2xl flex items-center justify-center text-xl mb-4">
                        <i class="fa-solid fa-seedling"></i>
                    </div>
                    <h3 class="font-extrabold text-choco-900 mb-2">1. Nutrisi Pisang Asli</h3>
                    <p class="text-xs text-choco-800/80 leading-relaxed">Kaya karbohidrat kompleks, serat, & potasium dari pisang murni. Bikin cepat kenyang & bertenaga tahan lama.</p>
                </div>

                <!-- Feature 2 -->
                <div class="bg-white p-6 rounded-3xl shadow-sm border border-banana-300/50 hover:-translate-y-1 transition-all">
                    <div class="w-12 h-12 bg-banana-400 text-choco-900 rounded-2xl flex items-center justify-center text-xl mb-4">
                        <i class="fa-solid fa-bag-shopping"></i>
                    </div>
                    <h3 class="font-extrabold text-choco-900 mb-2">2. Praktis "Grab & Go"</h3>
                    <p class="text-xs text-choco-800/80 leading-relaxed">Kemasan pouch simpel mudah diselipkan di tas. Bebas dinikmati di jalan, kantin, atau saat nunggu dosen.</p>
                </div>

                <!-- Feature 3 -->
                <div class="bg-white p-6 rounded-3xl shadow-sm border border-banana-300/50 hover:-translate-y-1 transition-all">
                    <div class="w-12 h-12 bg-banana-400 text-choco-900 rounded-2xl flex items-center justify-center text-xl mb-4">
                        <i class="fa-solid fa-cookie"></i>
                    </div>
                    <h3 class="font-extrabold text-choco-900 mb-2">3. Kelezatan Banana Butter</h3>
                    <p class="text-xs text-choco-800/80 leading-relaxed">Perpaduan manis alami pisang & gurihnya butter impor. Tekstur bulat renyah, lumer di mulut tanpa perlu banyak minum.</p>
                </div>

                <!-- Feature 4 -->
                <div class="bg-white p-6 rounded-3xl shadow-sm border border-banana-300/50 hover:-translate-y-1 transition-all">
                    <div class="w-12 h-12 bg-banana-400 text-choco-900 rounded-2xl flex items-center justify-center text-xl mb-4">
                        <i class="fa-solid fa-shield-heart"></i>
                    </div>
                    <h3 class="font-extrabold text-choco-900 mb-2">4. Tanpa Pengawet Buatan</h3>
                    <p class="text-xs text-choco-800/80 leading-relaxed">Menggunakan manis alami pisang matang tanpa pemanis sintetis. Aman dan nyaman untuk lambung di pagi hari.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- KATALOG PILIHAN VARIAN & HARGA -->
    <section id="produk" class="py-16 bg-white">
        <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-12">
                <h2 class="text-xs font-extrabold uppercase tracking-widest text-gold mb-2">Pilihan Varian Hemat</h2>
                <h3 class="text-3xl font-extrabold text-choco-900">Harga Terjangkau & Pas Buat Mahasiswa</h3>
                <p class="text-sm text-choco-800/70 mt-2">Dapatkan promo terbatas khusus hari ini!</p>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                
                <!-- Varian 1 -->
                <div class="bg-cream rounded-3xl border-2 border-banana-300 p-6 flex flex-col justify-between hover:shadow-xl transition-all relative">
                    <span class="absolute top-4 right-4 bg-red-500 text-white text-[10px] font-extrabold uppercase px-2.5 py-1 rounded-full">Hemat 33%</span>
                    <div>
                        <div class="h-44 rounded-2xl overflow-hidden mb-4 bg-banana-100 flex items-center justify-center">
                            <img src="https://images.unsplash.com/photo-1590080875515-8a3a8dc5735e?auto=format&fit=crop&w=500&q=80" alt="Mini Pouch Bananabites" class="w-full h-full object-cover">
                        </div>
                        <h4 class="font-extrabold text-xl text-choco-900">Mini Pouch (50gr)</h4>
                        <p class="text-xs text-choco-800/70 font-semibold mb-3">Pas Cuma Buat Ganjal Perut Pagi</p>
                        <div class="flex items-baseline gap-2 mb-4">
                            <span class="text-2xl font-extrabold text-choco-900">Rp 8.000</span>
                            <span class="text-sm text-gray-400 line-through">Rp 12.000</span>
                        </div>
                    </div>
                    <button onclick="addToCart('Mini Pouch (50gr)', 8000)" class="w-full bg-banana-400 hover:bg-banana-500 text-choco-900 font-extrabold py-3 rounded-xl transition-all flex items-center justify-center gap-2 active:scale-95 shadow-md">
                        <i class="fa-solid fa-cart-plus"></i> Tambah Ke Keranjang
                    </button>
                </div>

                <!-- Varian 2 (Best Seller) -->
                <div class="bg-gradient-to-b from-banana-100 to-cream rounded-3xl border-2 border-gold p-6 flex flex-col justify-between hover:shadow-2xl transition-all relative transform md:-translate-y-2">
                    <span class="absolute -top-3 left-1/2 -translate-x-1/2 bg-gold text-white text-[11px] font-extrabold uppercase px-4 py-1 rounded-full shadow">Paling Favorit 🔥</span>
                    <div>
                        <div class="h-44 rounded-2xl overflow-hidden mb-4 bg-banana-200 flex items-center justify-center">
                            <img src="https://images.unsplash.com/photo-1558961363-fa8fdf82db35?auto=format&fit=crop&w=500&q=80" alt="Daily Pack Bananabites" class="w-full h-full object-cover">
                        </div>
                        <h4 class="font-extrabold text-xl text-choco-900">Daily Pack (120gr)</h4>
                        <p class="text-xs text-choco-800/70 font-semibold mb-3">Kenyang & Hemat Buat Nyemil Sehari</p>
                        <div class="flex items-baseline gap-2 mb-4">
                            <span class="text-2xl font-extrabold text-gold">Rp 15.000</span>
                            <span class="text-sm text-gray-400 line-through">Rp 20.000</span>
                        </div>
                    </div>
                    <button onclick="addToCart('Daily Pack (120gr)', 15000)" class="w-full bg-gold hover:bg-amber-600 text-white font-extrabold py-3 rounded-xl transition-all flex items-center justify-center gap-2 active:scale-95 shadow-md">
                        <i class="fa-solid fa-cart-plus"></i> Tambah Ke Keranjang
                    </button>
                </div>

                <!-- Varian 3 -->
                <div class="bg-cream rounded-3xl border-2 border-banana-300 p-6 flex flex-col justify-between hover:shadow-xl transition-all relative">
                    <span class="absolute top-4 right-4 bg-green-600 text-white text-[10px] font-extrabold uppercase px-2.5 py-1 rounded-full">Super Hemat</span>
                    <div>
                        <div class="h-44 rounded-2xl overflow-hidden mb-4 bg-banana-100 flex items-center justify-center">
                            <img src="https://images.unsplash.com/photo-1548365328-8c6db4b63388?auto=format&fit=crop&w=500&q=80" alt="Bundel Kost Bananabites" class="w-full h-full object-cover">
                        </div>
                        <h4 class="font-extrabold text-xl text-choco-900">Bundel Kost (3x 120gr)</h4>
                        <p class="text-xs text-choco-800/70 font-semibold mb-3">Patungan Sama Temen Kos (~11.600/pack)</p>
                        <div class="flex items-baseline gap-2 mb-4">
                            <span class="text-2xl font-extrabold text-choco-900">Rp 35.000</span>
                            <span class="text-sm text-gray-400 line-through">Rp 45.000</span>
                        </div>
                    </div>
                    <button onclick="addToCart('Bundel Hemat Kost (3x Pack 120gr)', 35000)" class="w-full bg-banana-400 hover:bg-banana-500 text-choco-900 font-extrabold py-3 rounded-xl transition-all flex items-center justify-center gap-2 active:scale-95 shadow-md">
                        <i class="fa-solid fa-cart-plus"></i> Tambah Ke Keranjang
                    </button>
                </div>

            </div>
        </div>
    </section>

    <!-- CARA PESAN -->
    <section id="cara-pesan" class="py-16 bg-banana-100/60">
        <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-12">
                <h2 class="text-3xl font-extrabold text-choco-900">5 Langkah Mudah Pemesanan</h2>
                <p class="text-sm text-choco-800/70 mt-2">Pesan sekarang, siap antar langsung ke Kampus / Kosanmu!</p>
            </div>

            <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-5 gap-4">
                <div class="bg-white p-5 rounded-2xl shadow-sm border border-banana-300/40 text-center">
                    <div class="w-8 h-8 bg-banana-400 text-choco-900 font-extrabold rounded-full flex items-center justify-center mx-auto mb-3">1</div>
                    <p class="text-xs font-bold text-choco-900">Pilih Varian Bananabites</p>
                </div>
                <div class="bg-white p-5 rounded-2xl shadow-sm border border-banana-300/40 text-center">
                    <div class="w-8 h-8 bg-banana-400 text-choco-900 font-extrabold rounded-full flex items-center justify-center mx-auto mb-3">2</div>
                    <p class="text-xs font-bold text-choco-900">Masukkan Keranjang Belanja</p>
                </div>
                <div class="bg-white p-5 rounded-2xl shadow-sm border border-banana-300/40 text-center">
                    <div class="w-8 h-8 bg-banana-400 text-choco-900 font-extrabold rounded-full flex items-center justify-center mx-auto mb-3">3</div>
                    <p class="text-xs font-bold text-choco-900">Klik "Pesan via WhatsApp"</p>
                </div>
                <div class="bg-white p-5 rounded-2xl shadow-sm border border-banana-300/40 text-center">
                    <div class="w-8 h-8 bg-banana-400 text-choco-900 font-extrabold rounded-full flex items-center justify-center mx-auto mb-3">4</div>
                    <p class="text-xs font-bold text-choco-900">Bayar (Transfer / QRIS / Cash COD)</p>
                </div>
                <div class="bg-white p-5 rounded-2xl shadow-sm border border-banana-300/40 text-center">
                    <div class="w-8 h-8 bg-banana-400 text-choco-900 font-extrabold rounded-full flex items-center justify-center mx-auto mb-3">5</div>
                    <p class="text-xs font-bold text-choco-900">Pesanan Siap Diantar / Diambil</p>
                </div>
            </div>
        </div>
    </section>

    <!-- FOOTER -->
    <footer class="bg-choco-900 text-white py-12">
        <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex flex-col md:flex-row items-center justify-between gap-6 pb-8 border-b border-choco-800">
                <div>
                    <h3 class="text-2xl font-extrabold flex items-center gap-2">
                        <span>🍌</span> Bananabites
                    </h3>
                    <p class="text-xs text-banana-300 mt-1">“Ganjal Perut Praktis, Energi Murni Tanpa Telat Kuliah!”</p>
                </div>
                <div class="flex items-center gap-4 text-sm font-semibold">
                    <a href="https://wa.me/6283853447171" target="_blank" class="bg-green-500 hover:bg-green-600 text-white px-5 py-2.5 rounded-xl font-bold flex items-center gap-2 transition-all">
                        <i class="fa-brands fa-whatsapp text-lg"></i> 083853447171
                    </a>
                </div>
            </div>
            <div class="pt-8 text-center sm:text-left flex flex-col sm:flex-row items-center justify-between text-xs text-gray-400 gap-4">
                <p>&copy; 2026 Bananabites - Snack Banana Butter Cookies Mahasiswa. All Rights Reserved.</p>
                <p>Bisa COD area Kampus & Kos sekitarnya 🛵</p>
            </div>
        </div>
    </footer>

    <!-- CART DRAWER MODAL -->
    <div id="cartModal" class="fixed inset-0 bg-black/60 z-50 hidden opacity-0 transition-opacity duration-300" onclick="toggleCart()">
        <div class="fixed inset-y-0 right-0 max-w-full flex pl-10" onclick="event.stopPropagation()">
            <div class="w-screen max-w-md bg-white p-6 flex flex-col justify-between shadow-2xl">
                <div>
                    <div class="flex items-center justify-between border-b pb-4 mb-4">
                        <h3 class="text-xl font-extrabold text-choco-900 flex items-center gap-2">
                            <i class="fa-solid fa-cart-shopping text-gold"></i> Keranjang Belanja
                        </h3>
                        <button onclick="toggleCart()" class="text-gray-400 hover:text-gray-600 text-xl font-bold">&times;</button>
                    </div>

                    <div id="cartItemsList" class="space-y-4 max-h-[50vh] overflow-y-auto pr-1">
                        <!-- Items dynamically generated -->
                        <p class="text-sm text-gray-500 text-center py-8">Keranjang belanjaanmu masih kosong nih!</p>
                    </div>
                </div>

                <div class="border-t pt-4 space-y-4">
                    <div class="space-y-2">
                        <label class="block text-xs font-bold text-choco-900">Lokasi Pengantaran / Catatan COD:</label>
                        <input type="text" id="deliveryLocation" placeholder="Contoh: Kos Cantik No. 5 / Depan Gedung A Kampus" class="w-full text-xs p-3 border rounded-xl focus:ring-2 focus:ring-banana-400 outline-none">
                    </div>

                    <div class="flex justify-between items-center text-lg font-extrabold text-choco-900">
                        <span>Total Bayar:</span>
                        <span id="cartTotalPrice" class="text-gold">Rp 0</span>
                    </div>

                    <button onclick="checkoutWhatsApp()" class="w-full bg-green-500 hover:bg-green-600 text-white font-extrabold py-3.5 rounded-xl transition-all flex items-center justify-center gap-2 shadow-lg active:scale-95">
                        <i class="fa-brands fa-whatsapp text-xl"></i> Pesan via WhatsApp
                    </button>
                </div>
            </div>
        </div>
    </div>

    <!-- JAVASCRIPT LOGIC -->
    <script>
        let cart = [];

        function addToCart(name, price) {
            const existingIndex = cart.findIndex(item => item.name === name);
            if (existingIndex > -1) {
                cart[existingIndex].qty += 1;
            } else {
                cart.push({ name, price, qty: 1 });
            }
            updateCartUI();
            
            // Open cart drawer on addition
            const modal = document.getElementById('cartModal');
            if(modal.classList.contains('hidden')) {
                toggleCart();
            }
        }

        function changeQty(index, delta) {
            cart[index].qty += delta;
            if (cart[index].qty <= 0) {
                cart.splice(index, 1);
            }
            updateCartUI();
        }

        function updateCartUI() {
            const listContainer = document.getElementById('cartItemsList');
            const cartCountEl = document.getElementById('cartCount');
            const totalPriceEl = document.getElementById('cartTotalPrice');

            let totalQty = 0;
            let totalPrice = 0;

            if (cart.length === 0) {
                listContainer.innerHTML = `<p class="text-sm text-gray-500 text-center py-8">Keranjang belanjaanmu masih kosong nih!</p>`;
            } else {
                listContainer.innerHTML = '';
                cart.forEach((item, index) => {
                    totalQty += item.qty;
                    totalPrice += item.price * item.qty;

                    listContainer.innerHTML += `
                        <div class="flex items-center justify-between bg-banana-100/40 p-3 rounded-2xl border border-banana-200">
                            <div>
                                <h5 class="text-xs font-extrabold text-choco-900">${item.name}</h5>
                                <p class="text-xs text-gold font-bold">Rp ${(item.price * item.qty).toLocaleString('id-ID')}</p>
                            </div>
                            <div class="flex items-center gap-2 bg-white rounded-lg px-2 py-1 border shadow-sm">
                                <button onclick="changeQty(${index}, -1)" class="text-xs font-extrabold text-choco-900 px-1">-</button>
                                <span class="text-xs font-bold px-1">${item.qty}</span>
                                <button onclick="changeQty(${index}, 1)" class="text-xs font-extrabold text-choco-900 px-1">+</button>
                            </div>
                        </div>
                    `;
                });
            }

            cartCountEl.innerText = totalQty;
            totalPriceEl.innerText = `Rp ${totalPrice.toLocaleString('id-ID')}`;
        }

        function toggleCart() {
            const modal = document.getElementById('cartModal');
            if (modal.classList.contains('hidden')) {
                modal.classList.remove('hidden');
                setTimeout(() => modal.classList.remove('opacity-0'), 10);
            } else {
                modal.classList.add('opacity-0');
                setTimeout(() => modal.classList.add('hidden'), 300);
            }
        }

        function checkoutWhatsApp() {
            if (cart.length === 0) {
                alert("Keranjang kamu masih kosong. Pilih varian Bananabites terlebih dahulu!");
                return;
            }

            const location = document.getElementById('deliveryLocation').value || 'COD Kampus / Kos';
            let message = `Halo Kak, saya mau pesan Bananabites untuk ganjal perut sarapan! 🍌🍪\n\n*Rincian Pesanan:*\n`;

            let total = 0;
            cart.forEach((item, i) => {
                const subtotal = item.price * item.qty;
                total += subtotal;
                message += `${i + 1}. ${item.name} (${item.qty}x) = Rp ${subtotal.toLocaleString('id-ID')}\n`;
            });

            message += `\n*Total Pembayaran:* Rp ${total.toLocaleString('id-ID')}`;
            message += `\n*Lokasi Pengantaran / COD:* ${location}`;
            message += `\n\nMohon konfirmasi dan info metode pembayarannya ya, terima kasih!`;

            const encodedMessage = encodeURIComponent(message);
            window.open(`https://wa.me/6283853447171?text=${encodedMessage}`, '_blank');
        }
    </script>
</body>
</html>
