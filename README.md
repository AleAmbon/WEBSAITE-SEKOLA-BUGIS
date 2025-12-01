<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SD Negeri 2 Bugis - Profil & Kegiatan</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css" />

    <style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #f8fafc;
            scroll-behavior: smooth;
        }
        /* Header Background menggunakan bugis 03.jpg */
        .header-bg {
            position: relative;
            background-color: #991b1b;
            color: white;
            overflow: hidden;
        }
        .header-bg::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            /* FOTO BACKGROUND UTAMA */
            background: url('bugis 03.jpg') center/cover no-repeat;
            opacity: 0.25; /* Mengatur kecerahan foto background */
            z-index: 0;
        }
        .header-content {
            position: relative;
            z-index: 1;
        }
        .card-hover {
            transition: all 0.3s ease;
        }
        .card-hover:hover {
            transform: translateY(-5px);
            box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.1), 0 10px 10px -5px rgba(0, 0, 0, 0.04);
        }
        .gallery-img-container {
            overflow: hidden;
            position: relative;
            height: 250px;
        }
        .gallery-img-container img {
            transition: transform 0.6s ease;
            width: 100%;
            height: 100%;
            object-fit: cover;
        }
        .gallery-img-container:hover img {
            transform: scale(1.1);
        }
        .overlay-gradient {
            background: linear-gradient(to top, rgba(0,0,0,0.8) 0%, rgba(0,0,0,0) 100%);
        }
    </style>
</head>
<body class="text-gray-800">

    <nav class="sticky top-0 z-50 bg-white/95 backdrop-blur-md shadow-md border-b border-gray-100">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center h-16">
                <div class="flex items-center gap-2">
                    <i class="fas fa-school text-red-600 text-2xl"></i>
                    <span class="text-xl font-bold text-red-700 tracking-tight">SDN 2 BUGIS</span>
                </div>
                <div class="hidden md:flex space-x-8">
                    <a href="#home" class="text-gray-600 hover:text-red-600 font-medium transition">Beranda</a>
                    <a href="#profile" class="text-gray-600 hover:text-red-600 font-medium transition">Profil</a>
                    <a href="#gallery" class="text-gray-600 hover:text-red-600 font-medium transition">Kegiatan</a>
                    <a href="#contact" class="text-gray-600 hover:text-red-600 font-medium transition">Kontak</a>
                </div>
                <div class="md:hidden">
                    <button id="mobile-menu-btn" class="text-gray-600 hover:text-red-600 focus:outline-none">
                        <i class="fas fa-bars text-xl"></i>
                    </button>
                </div>
            </div>
        </div>
        <div id="mobile-menu" class="hidden md:hidden bg-white border-t">
            <div class="px-4 pt-2 pb-4 space-y-1">
                <a href="#home" class="block py-2 text-gray-700 hover:text-red-600">Beranda</a>
                <a href="#profile" class="block py-2 text-gray-700 hover:text-red-600">Profil</a>
                <a href="#gallery" class="block py-2 text-gray-700 hover:text-red-600">Kegiatan</a>
                <a href="#contact" class="block py-2 text-gray-700 hover:text-red-600">Kontak</a>
            </div>
        </div>
    </nav>

    <section id="home" class="header-bg py-24 sm:py-32">
        <div class="max-w-7xl mx-auto px-4 text-center header-content">
            <span class="inline-block py-1 px-3 rounded-full bg-red-800/50 border border-red-400 text-red-100 text-sm font-semibold mb-4 backdrop-blur-sm">
                Selamat Datang di Website Resmi
            </span>
            <h1 class="text-4xl sm:text-6xl font-extrabold mb-6 leading-tight drop-shadow-lg">
                SD NEGERI 2 BUGIS
            </h1>
            <p class="text-lg sm:text-2xl mb-10 font-light text-gray-100 max-w-2xl mx-auto drop-shadow-md">
                Mewujudkan Generasi yang Cerdas, Berkarakter, dan Berakhlak Mulia.
            </p>
            <div class="flex justify-center gap-4">
                <a href="#gallery" class="bg-white text-red-700 font-bold py-3 px-8 rounded-full shadow-lg hover:bg-gray-100 transition transform hover:scale-105">
                    Lihat Kegiatan
                </a>
                <a href="#contact" class="bg-transparent border-2 border-white text-white font-bold py-3 px-8 rounded-full hover:bg-white hover:text-red-700 transition">
                    Hubungi Kami
                </a>
            </div>
        </div>
    </section>

    <section id="profile" class="py-16 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid md:grid-cols-2 gap-12 items-center">
                <div>
                    <h2 class="text-3xl font-bold text-gray-900 mb-6 border-l-4 border-red-600 pl-4">
                        Lingkungan Belajar Nyaman
                    </h2>
                    <p class="text-gray-600 text-lg leading-relaxed mb-6">
                        SD Negeri 2 Bugis berkomitmen menyediakan fasilitas pendidikan yang layak dan aman. Gedung sekolah kami yang terawat dengan nuansa merah putih menumbuhkan semangat kebangsaan dan kenyamanan bagi para siswa dalam menuntut ilmu.
                    </p>
                    <ul class="space-y-4">
                        <li class="flex items-center text-gray-700">
                            <i class="fas fa-check-circle text-green-500 mr-3 text-lg"></i> Gedung Permanen & Terawat
                        </li>
                        <li class="flex items-center text-gray-700">
                            <i class="fas fa-check-circle text-green-500 mr-3 text-lg"></i> Halaman Luas & Aman
                        </li>
                        <li class="flex items-center text-gray-700">
                            <i class="fas fa-check-circle text-green-500 mr-3 text-lg"></i> Lokasi Strategis di Desa Bugis
                        </li>
                    </ul>
                </div>
                
                <div class="grid gap-4 grid-cols-2">
                    <div class="rounded-xl overflow-hidden shadow-lg h-48 transform translate-y-8">
                        <img src="foto_bugis/bugis02.jpg" alt="Plang Sekolah SDN 2 Bugis" class="w-full h-full object-cover hover:scale-110 transition duration-500">
                    </div>
                    <div class="rounded-xl overflow-hidden shadow-lg h-48">
                        <img src="foto_bugis/bugis01.jpg" alt="Teras Gedung Sekolah" class="w-full h-full object-cover hover:scale-110 transition duration-500">
                    </div>
                </div>
            </div>
        </div>
    </section>

    <section id="gallery" class="py-20 bg-gray-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16">
                <span class="text-red-600 font-bold tracking-wider uppercase text-sm">Dokumentasi</span>
                <h2 class="text-3xl sm:text-4xl font-bold text-gray-900 mt-2">Galeri Kegiatan Sekolah</h2>
                <div class="w-20 h-1 bg-red-600 mx-auto mt-4 rounded-full"></div>
                <p class="mt-4 text-gray-600 max-w-2xl mx-auto">
                    Potret aktivitas siswa, guru, dan lingkungan SD Negeri 2 Bugis dalam keseharian.
                </p>
            </div>

            <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-8">
                
                <div class="bg-white rounded-2xl shadow-md overflow-hidden card-hover group">
                    <div class="gallery-img-container">
                        <img src="foto_bugis/bugis05.png" alt="Foto Bersama Siswa dan Guru">
                        <div class="absolute inset-0 overlay-gradient opacity-0 group-hover:opacity-100 transition duration-300 flex items-end p-6">
                            <span class="text-white font-semibold text-lg">Kecerian Kelas</span>
                        </div>
                    </div>
                    <div class="p-6">
                        <h3 class="font-bold text-xl mb-2 text-gray-800">Kegiatan Belajar Mengajar</h3>
                        <p class="text-gray-600 text-sm">Keakraban antara guru dan siswa menciptakan suasana belajar yang menyenangkan dan interaktif di dalam kelas.</p>
                    </div>
                </div>

                <div class="bg-white rounded-2xl shadow-md overflow-hidden card-hover group">
                    <div class="gallery-img-container">
                        <img src="foto_bugis/bugis04.png" alt="Kegiatan Vaksinasi Siswa">
                        <div class="absolute inset-0 overlay-gradient opacity-0 group-hover:opacity-100 transition duration-300 flex items-end p-6">
                            <span class="text-white font-semibold text-lg">Program Kesehatan</span>
                        </div>
                    </div>
                    <div class="p-6">
                        <h3 class="font-bold text-xl mb-2 text-gray-800">Kesehatan Siswa</h3>
                        <p class="text-gray-600 text-sm">Pelaksanaan program kesehatan dan vaksinasi untuk memastikan seluruh siswa tetap sehat dan siap belajar.</p>
                    </div>
                </div>

                <div class="bg-white rounded-2xl shadow-md overflow-hidden card-hover group">
                    <div class="gallery-img-container">
                        <img src="foto_bugis/bugis 03.jpg" alt="Tampak Depan Sekolah">
                        <div class="absolute inset-0 overlay-gradient opacity-0 group-hover:opacity-100 transition duration-300 flex items-end p-6">
                            <span class="text-white font-semibold text-lg">Lingkungan Sekolah</span>
                        </div>
                    </div>
                    <div class="p-6">
                        <h3 class="font-bold text-xl mb-2 text-gray-800">Fasilitas Sekolah</h3>
                        <p class="text-gray-600 text-sm">Gedung sekolah yang representatif, bersih, dan asri dilihat dari jalan utama Desa Bugis.</p>
                    </div>
                </div>

                 <div class="bg-white rounded-2xl shadow-md overflow-hidden card-hover group">
                    <div class="gallery-img-container">
                        <img src="foto_bugis/bugis02.jpg" alt="Identitas Sekolah">
                        <div class="absolute inset-0 overlay-gradient opacity-0 group-hover:opacity-100 transition duration-300 flex items-end p-6">
                            <span class="text-white font-semibold text-lg">Identitas Resmi</span>
                        </div>
                    </div>
                    <div class="p-6">
                        <h3 class="font-bold text-xl mb-2 text-gray-800">Profil Kelembagaan</h3>
                        <p class="text-gray-600 text-sm">Terdaftar resmi sebagai UPTD SD Negeri 2 Bugis, siap melayani pendidikan dasar bagi masyarakat sekitar.</p>
                    </div>
                </div>

                <div class="bg-white rounded-2xl shadow-md overflow-hidden card-hover group">
                    <div class="gallery-img-container">
                        <img src="foto_bugis/bugis 03.jpg" alt="Detail Bangunan">
                        <div class="absolute inset-0 overlay-gradient opacity-0 group-hover:opacity-100 transition duration-300 flex items-end p-6">
                            <span class="text-white font-semibold text-lg">Gedung Sekolah</span>
                        </div>
                    </div>
                    <div class="p-6">
                        <h3 class="font-bold text-xl mb-2 text-gray-800">Sarana Prasarana</h3>
                        <p class="text-gray-600 text-sm">Kondisi bangunan yang kokoh dan estetis dengan cat kombinasi merah putih yang baru diperbarui.</p>
                    </div>
                </div>
                
                <div class="bg-red-600 rounded-2xl shadow-md overflow-hidden card-hover flex flex-col items-center justify-center p-8 text-center text-white">
                    <i class="fas fa-quote-left text-4xl mb-4 opacity-50"></i>
                    <p class="text-lg italic font-medium mb-4">"Pendidikan adalah senjata paling ampuh untuk mengubah dunia."</p>
                    <p class="font-bold text-yellow-300">- Nelson Mandela</p>
                    <div class="mt-8 border-t border-red-400 pt-4 w-full">
                        <p class="text-sm opacity-90">Bergabunglah bersama kami di SDN 2 Bugis.</p>
                    </div>
                </div>

            </div>
        </div>
    </section>

    <footer id="contact" class="bg-gray-900 text-white pt-16 pb-8">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid md:grid-cols-3 gap-8 mb-12">
                <div>
                    <h4 class="text-2xl font-bold text-red-500 mb-4">SD N 2 BUGIS</h4>
                    <p class="text-gray-400 leading-relaxed">
                        Jl. Sukatani Laban, Desa Bugis, <br>
                        Kec. Anjatan, Kab. Indramayu,<br>
                        Jawa Barat 45256
                    </p>
                </div>
                <div>
                    <h4 class="text-lg font-bold mb-4">Kontak Kami</h4>
                    <ul class="space-y-3 text-gray-400">
                        <li class="flex items-center"><i class="fas fa-phone mr-3 text-red-500"></i> (0234)082237889061</li>
                        <li class="flex items-center"><i class="fas fa-envelope mr-3 text-red-500"></i> info@sdn2bugis.sch.id</li>
                        <li class="flex items-center"><i class="fas fa-clock mr-3 text-red-500"></i> Senin - Sabtu: 07.00 - 13.00</li>
                    </ul>
                </div>
                <div>
                    <h4 class="text-lg font-bold mb-4">Peta Lokasi</h4>
                    <div class="rounded-lg overflow-hidden h-40 bg-gray-800">
                        <iframe 
                            src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3964.832269661448!2d107.9547!3d-6.4156!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x0%3A0x0!2zNsKwMjQnNTYuMiJTIDEwN8KwNTcnMTYuOSJF!5e0!3m2!1sid!2sid!4v1620000000000!5m2!1sid!2sid" 
                            width="100%" height="100%" style="border:0;" allowfullscreen="" loading="lazy">
                        </iframe>
                    </div>
                    <small class="text-gray-500 mt-2 block">*Peta area Kecamatan Anjatan</small>
                </div>
            </div>
            <div class="border-t border-gray-800 pt-8 text-center text-gray-500 text-sm">
                <p>&copy; 2025 SD Negeri 2 Bugis. All rights reserved.</p>
                <p class="mt-1">Prototipe Web Sekolah.</p>
            </div>
        </div>
    </footer>

    <script>
        // Script untuk Mobile Menu Toggle
        const menuBtn = document.getElementById('mobile-menu-btn');
        const mobileMenu = document.getElementById('mobile-menu');

        menuBtn.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
        });

        // Menutup menu saat link diklik
        document.querySelectorAll('#mobile-menu a').forEach(link => {
            link.addEventListener('click', () => {
                mobileMenu.classList.add('hidden');
            });
        });
    </script>
</body>
</html>
