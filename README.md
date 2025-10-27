
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Profil Resmi SMPN 02 Tirto</title>
    <!-- Memuat Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Konfigurasi untuk menggunakan Font Inter -->
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@100..900&display=swap');
        body {
            font-family: 'Inter', sans-serif;
            background-color: #f7f7f7;
            /* body: scroll-behavior: smooth; tidak didukung di semua browser, jadi kita gunakan JS */
        }
        /* Style untuk menonaktifkan scroll saat menu mobile terbuka */
        .overflow-hidden { overflow: hidden; }
        .nav-link:hover {
            color: #ffffff; /* Warna putih saat hover */
            background-color: #14b8a6; /* Warna teal saat hover */
            transition: all 0.3s ease;
        }
    </style>
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        'primary': '#0e7490', // Biru Teal Tua (dari placeholder)
                        'secondary': '#14b8a6', // Teal Muda
                        'accent': '#fbbf24', // Kuning Aksen
                    }
                }
            }
        }
    </script>
</head>
<body class="text-gray-800">

    <!-- Navbar/Header (Sticky dan Responsive) -->
    <header class="bg-primary shadow-lg sticky top-0 z-50">
        <nav class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center h-16">
                <!-- Logo/Nama Sekolah -->
                <div class="flex-shrink-0 text-white font-extrabold text-xl tracking-wider">
                    SMPN 02 TIRTO
                </div>

                <!-- Link Navigasi Desktop -->
                <div class="hidden md:flex space-x-4 items-center">
                    <a href="#beranda" class="text-white px-3 py-2 rounded-md text-sm font-medium nav-link">Beranda</a>
                    <!-- Link PPDB Baru -->
                    <a href="#ppdb" class="text-white bg-accent px-4 py-2 rounded-full text-sm font-bold shadow-md hover:bg-yellow-400 transition duration-300">
                        INFO PPDB 2025/2026
                    </a>
                    <a href="#visimisi" class="text-white px-3 py-2 rounded-md text-sm font-medium nav-link">Visi & Misi</a>
                    <a href="#staf" class="text-white px-3 py-2 rounded-md text-sm font-medium nav-link">Guru</a>
                    <a href="#kegiatan" class="text-white px-3 py-2 rounded-md text-sm font-medium nav-link">Kegiatan</a>
                    <a href="#fasilitas" class="text-white px-3 py-2 rounded-md text-sm font-medium nav-link">Fasilitas</a>
                    <a href="#kontak" class="text-white px-3 py-2 rounded-md text-sm font-medium nav-link">Kontak</a>
                </div>

                <!-- Tombol Menu Mobile -->
                <div class="md:hidden">
                    <button id="menu-button" type="button" class="inline-flex items-center justify-center p-2 rounded-md text-white hover:bg-secondary focus:outline-none focus:ring-2 focus:ring-inset focus:ring-white" aria-controls="mobile-menu" aria-expanded="false">
                        <!-- Ikon Hamburger (Menu) -->
                        <svg id="menu-icon-open" class="block h-6 w-6" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor" aria-hidden="true">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
                        </svg>
                        <!-- Ikon Silang (Tutup) -->
                        <svg id="menu-icon-close" class="hidden h-6 w-6" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor" aria-hidden="true">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12" />
                        </svg>
                    </button>
                </div>
            </div>
        </nav>

        <!-- Menu Mobile (Tersembunyi secara default) -->
        <div id="mobile-menu" class="hidden md:hidden bg-primary/95 absolute w-full shadow-xl">
            <div class="px-2 pt-2 pb-3 space-y-1 sm:px-3">
                <a href="#beranda" class="text-white block px-3 py-2 rounded-md text-base font-medium hover:bg-secondary">Beranda</a>
                <!-- Link PPDB Mobile -->
                <a href="#ppdb" class="text-primary bg-accent block px-3 py-2 rounded-md text-base font-bold text-center hover:bg-yellow-400">INFO PPDB 2025/2026</a>
                <a href="#visimisi" class="text-white block px-3 py-2 rounded-md text-base font-medium hover:bg-secondary">Visi & Misi</a>
                <a href="#staf" class="text-white block px-3 py-2 rounded-md text-base font-medium hover:bg-secondary">Guru</a>
                <a href="#kegiatan" class="text-white block px-3 py-2 rounded-md text-base font-medium hover:bg-secondary">Kegiatan</a>
                <a href="#fasilitas" class="text-white block px-3 py-2 rounded-md text-base font-medium hover:bg-secondary">Fasilitas</a>
                <a href="#kontak" class="text-white block px-3 py-2 rounded-md text-base font-medium hover:bg-secondary">Kontak</a>
            </div>
        </div>
    </header>

    <main>
        <!-- Bagian Beranda (Hero Section) -->
        <section id="beranda" class="relative bg-white pt-16 pb-20 overflow-hidden">
            <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
                <div class="text-center">
                    <h1 class="text-4xl sm:text-5xl lg:text-6xl font-extrabold text-primary mb-4 animate-fadeIn">
                        Selamat Datang di <span class="text-secondary">SMPN 02 Tirto</span>
                    </h1>
                    <p class="text-lg sm:text-xl text-gray-600 mb-8 max-w-3xl mx-auto">
                        Mencetak generasi cerdas, berakhlak mulia, dan berwawasan global.
                    </p>
                    <!-- Tombol PPDB yang menonjol di Hero Section -->
                    <a href="#ppdb" class="inline-block bg-accent text-primary font-bold text-xl py-3 px-8 rounded-full shadow-2xl transition duration-300 transform hover:scale-105 hover:bg-yellow-400 focus:outline-none focus:ring-4 focus:ring-accent focus:ring-opacity-50">
                        Daftar PPDB Sekarang!
                    </a>
                </div>
                <!-- Gambar Sekolah (Placeholder disempurnakan) -->
                <div class="mt-10 rounded-xl shadow-2xl overflow-hidden transform hover:scale-[1.005] transition duration-500">
                    <img src="https://placehold.co/1200x450/0e7490/ffffff?text=FOTO+GEDUNG+SEKOLAH+SMPN+02+TIRTO" alt="Gedung SMPN 02 Tirto" class="w-full h-auto object-cover" onerror="this.onerror=null; this.src='https://placehold.co/1200x450/0e7490/ffffff?text=FOTO+SEKOLAH+TIDAK+DITEMUKAN';">
                </div>
            </div>
        </section>
        
        <!-- Bagian PPDB (Penerimaan Peserta Didik Baru) - BARU -->
        <section id="ppdb" class="py-16 bg-secondary text-white">
            <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
                <div class="text-center mb-10">
                    <h2 class="text-4xl font-extrabold mb-3 text-white">
                        Penerimaan Peserta Didik Baru (PPDB)
                    </h2>
                    <p class="text-xl font-light text-gray-100">Tahun Ajaran 2025/2026</p>
                </div>
                
                <div class="grid md:grid-cols-3 gap-8">
                    <!-- Kartu Jadwal -->
                    <div class="bg-primary p-6 rounded-xl shadow-2xl border-b-4 border-accent">
                        <div class="text-4xl mb-4 text-accent">🗓️</div>
                        <h3 class="text-2xl font-bold mb-3">Jadwal Penting</h3>
                        <ul class="space-y-2 text-sm">
                            <li class="flex justify-between items-center border-b border-white/20 pb-1">Pendaftaran Online: <span class="font-bold">1 - 15 Juni 2025</span></li>
                            <li class="flex justify-between items-center border-b border-white/20 pb-1">Verifikasi Dokumen: <span class="font-bold">16 - 20 Juni 2025</span></li>
                            <li class="flex justify-between items-center pb-1">Pengumuman Hasil: <span class="font-bold">25 Juni 2025</span></li>
                        </ul>
                    </div>
                    
                    <!-- Kartu Persyaratan -->
                    <div class="bg-primary p-6 rounded-xl shadow-2xl border-b-4 border-accent">
                        <div class="text-4xl mb-4 text-accent">📄</div>
                        <h3 class="text-2xl font-bold mb-3">Persyaratan Umum</h3>
                        <ul class="space-y-2 text-sm list-disc pl-5">
                            <li>Lulusan SD/MI atau sederajat.</li>
                            <li>Usia maksimal 15 tahun per 1 Juli 2025.</li>
                            <li>Memiliki Akta Kelahiran/Surat Keterangan Lahir.</li>
                            <li>Memiliki Kartu Keluarga (KK).</li>
                        </ul>
                    </div>
                    
                    <!-- Kartu Alur Pendaftaran -->
                    <div class="bg-primary p-6 rounded-xl shadow-2xl border-b-4 border-accent">
                        <div class="text-4xl mb-4 text-accent">➡️</div>
                        <h3 class="text-2xl font-bold mb-3">Alur Pendaftaran</h3>
                        <ol class="space-y-2 text-sm list-decimal pl-5">
                            <li>Buka laman PPDB resmi kota.</li>
                            <li>Isi formulir pendaftaran dan unggah berkas.</li>
                            <li>Cetak Tanda Bukti Pendaftaran.</li>
                            <li>Pantau status verifikasi dan hasil seleksi.</li>
                        </ol>
                    </div>
                </div>

                <div class="text-center mt-12">
                    <a href="https://ppdb.dinas-pendidikan-tirto.go.id" target="_blank" class="inline-block bg-accent text-primary font-extrabold text-xl py-3 px-8 rounded-full shadow-2xl transition duration-300 transform hover:scale-105 hover:bg-yellow-400">
                        Kunjungi Portal Pendaftaran Resmi
                    </a>
                    <p class="mt-4 text-gray-200 text-sm">Untuk pertanyaan lebih lanjut, silakan hubungi kontak sekolah kami.</p>
                </div>
                
            </div>
        </section>

        <!-- Bagian Visi & Misi (posisi bergeser ke bawah PPDB) -->
        <section id="visimisi" class="py-16 bg-white">
            <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
                <h2 class="text-3xl font-bold text-center text-primary mb-12 border-b-2 border-accent inline-block pb-1">
                    Visi & Misi
                </h2>
                <div class="grid md:grid-cols-2 gap-8">
                    <!-- Visi Card -->
                    <div class="bg-gray-50 p-8 rounded-xl shadow-lg border-t-4 border-secondary transform hover:translate-y-[-5px] transition duration-300">
                        <div class="flex items-center space-x-3 mb-4">
                             <!-- Icon SVG untuk Visi -->
                            <svg class="w-8 h-8 text-secondary" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12l2 2 4-4m5.618-4.016A11.955 111.955 0 0112 2.944a11.955 11.955 0 01-8.618 3.04A12.002 12.002 0 0012 21.001c1.888-2.333 2.87-3.79 3-4.5h.001c.148.048.297.092.446.131.95.253 1.948.37 2.949.37.761 0 1.503-.075 2.232-.218.423-.08.835-.176 1.233-.284M12 12v.01"></path></svg>
                            <h3 class="text-2xl font-semibold text-primary">Visi</h3>
                        </div>
                        <blockquote class="italic text-gray-700 leading-relaxed border-l-4 border-accent pl-4">
                            "Terwujudnya Peserta Didik yang Unggul dalam Prestasi, Berbudaya Lingkungan, dan Berlandaskan Iman dan Taqwa."
                        </blockquote>
                    </div>

                    <!-- Misi Card -->
                    <div class="bg-gray-50 p-8 rounded-xl shadow-lg border-t-4 border-secondary transform hover:translate-y-[-5px] transition duration-300">
                        <div class="flex items-center space-x-3 mb-4">
                            <!-- Icon SVG untuk Misi -->
                            <svg class="w-8 h-8 text-secondary" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 10V3L4 14h7v7l9-11h-7z"></path></svg>
                            <h3 class="text-2xl font-semibold text-primary">Misi</h3>
                        </div>
                        <ul class="space-y-3 list-none p-0 text-gray-700">
                            <li class="flex items-start">
                                <span class="text-secondary mr-2 font-bold">&#10003;</span>
                                Meningkatkan mutu pembelajaran dan pembinaan secara efektif.
                            </li>
                            <li class="flex items-start">
                                <span class="text-secondary mr-2 font-bold">&#10003;</span>
                                Mengembangkan potensi diri peserta didik di bidang akademik dan non-akademik.
                            </li>
                            <li class="flex items-start">
                                <span class="text-secondary mr-2 font-bold">&#10003;</span>
                                Membentuk karakter religius dan mandiri.
                            </li>
                            <li class="flex items-start">
                                <span class="text-secondary mr-2 font-bold">&#10003;</span>
                                Menciptakan lingkungan sekolah yang bersih, indah, dan nyaman.
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
        </section>

        <!-- Bagian Staf Pengajar -->
        <section id="staf" class="py-16 bg-gray-100">
            <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
                <h2 class="text-3xl font-bold text-center text-primary mb-12 border-b-2 border-accent inline-block pb-1">
                    Staf Pengajar (Guru)
                </h2>

                <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-8">
                    <!-- Kartu Staf 1 -->
                    <div class="bg-white rounded-xl shadow-xl p-6 text-center border-t-4 border-primary hover:shadow-2xl transition duration-300">
                        <img src="https://placehold.co/120x120/0e7490/ffffff?text=Bapak" alt="Foto Bapak Budi Santoso" class="w-24 h-24 rounded-full mx-auto mb-4 object-cover border-4 border-accent">
                        <h4 class="text-xl font-bold text-primary">Bapak Budi Santoso</h4>
                        <p class="text-sm font-semibold text-secondary">Kepala Sekolah</p>
                        <p class="text-sm text-gray-600">Pendidikan Agama</p>
                    </div>

                    <!-- Kartu Staf 2 -->
                    <div class="bg-white rounded-xl shadow-xl p-6 text-center border-t-4 border-primary hover:shadow-2xl transition duration-300">
                        <img src="https://placehold.co/120x120/14b8a6/ffffff?text=Ibu" alt="Foto Ibu Siti Aminah" class="w-24 h-24 rounded-full mx-auto mb-4 object-cover border-4 border-accent">
                        <h4 class="text-xl font-bold text-primary">Ibu Siti Aminah</h4>
                        <p class="text-sm font-semibold text-secondary">Guru Matematika</p>
                        <p class="text-sm text-gray-600">Wali Kelas IX-A</p>
                    </div>

                    <!-- Kartu Staf 3 -->
                    <div class="bg-white rounded-xl shadow-xl p-6 text-center border-t-4 border-primary hover:shadow-2xl transition duration-300">
                        <img src="https://placehold.co/120x120/0e7490/ffffff?text=Bapak" alt="Foto Bapak Joko Susilo" class="w-24 h-24 rounded-full mx-auto mb-4 object-cover border-4 border-accent">
                        <h4 class="text-xl font-bold text-primary">Bapak Joko Susilo</h4>
                        <p class="text-sm font-semibold text-secondary">Guru Bahasa Inggris</p>
                        <p class="text-sm text-gray-600">Pembina OSIS</p>
                    </div>

                    <!-- Kartu Staf 4 -->
                    <div class="bg-white rounded-xl shadow-xl p-6 text-center border-t-4 border-primary hover:shadow-2xl transition duration-300">
                        <img src="https://placehold.co/120x120/14b8a6/ffffff?text=Ibu" alt="Foto Ibu Rina Dewi" class="w-24 h-24 rounded-full mx-auto mb-4 object-cover border-4 border-accent">
                        <h4 class="text-xl font-bold text-primary">Ibu Rina Dewi</h4>
                        <p class="text-sm font-semibold text-secondary">Guru IPA</p>
                        <p class="text-sm text-gray-600">Koordinator Lab</p>
                    </div>
                </div>

                <div class="text-center mt-10">
                    <a href="#" class="inline-block bg-secondary text-white font-medium py-3 px-6 rounded-lg shadow-md hover:bg-primary transition duration-300">
                        Lihat Daftar Lengkap Staf Pengajar
                    </a>
                </div>
            </div>
        </section>

        <!-- Bagian Kegiatan & Ekstrakurikuler -->
        <section id="kegiatan" class="py-16 bg-white">
            <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
                <h2 class="text-3xl font-bold text-center text-primary mb-12 border-b-2 border-accent inline-block pb-1">
                    Kegiatan & Ekstrakurikuler
                </h2>
                <div class="grid md:grid-cols-3 gap-8">

                    <!-- Kegiatan 1: Futsal -->
                    <div class="bg-gray-50 p-6 rounded-xl shadow-lg hover:shadow-2xl transform hover:scale-[1.02] transition duration-300">
                        <div class="text-4xl text-accent mb-3">⚽</div>
                        <h4 class="text-xl font-bold text-primary mb-2">Ekstrakurikuler Futsal</h4>
                        <p class="text-gray-700">Tim futsal sekolah rutin berlatih dan mengikuti kompetisi antar sekolah di tingkat kabupaten, menumbuhkan jiwa sportivitas.</p>
                    </div>

                    <!-- Kegiatan 2: Pentas Seni -->
                    <div class="bg-gray-50 p-6 rounded-xl shadow-lg hover:shadow-2xl transform hover:scale-[1.02] transition duration-300">
                        <div class="text-4xl text-accent mb-3">🎨</div>
                        <h4 class="text-xl font-bold text-primary mb-2">Pentas Seni Tahunan</h4>
                        <p class="text-gray-700">Acara tahunan menampilkan bakat siswa dalam seni tari, musik, drama, dan paduan suara, wadah kreativitas tanpa batas.</p>
                    </div>

                    <!-- Kegiatan 3: Jum'at Bersih -->
                    <div class="bg-gray-50 p-6 rounded-xl shadow-lg hover:shadow-2xl transform hover:scale-[1.02] transition duration-300">
                        <div class="text-4xl text-accent mb-3">🌿</div>
                        <h4 class="text-xl font-bold text-primary mb-2">Jum'at Bersih dan Hijau</h4>
                        <p class="text-gray-700">Kegiatan rutin untuk menanam dan merawat taman sekolah, mendukung program sekolah Adiwiyata dan peduli lingkungan.</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Bagian Prestasi -->
        <section id="prestasi" class="py-16 bg-gray-100">
            <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
                <h2 class="text-3xl font-bold text-center text-primary mb-12 border-b-2 border-accent inline-block pb-1">
                    Prestasi Sekolah & Siswa
                </h2>

                <div class="space-y-6 max-w-4xl mx-auto">
                    <!-- Prestasi 1 -->
                    <div class="flex items-center bg-white p-6 rounded-lg shadow-md border-l-4 border-secondary">
                        <div class="text-4xl text-accent mr-4">🥇</div>
                        <div>
                            <p class="font-semibold text-lg text-primary">Juara 1 Lomba Sains Tingkat Kabupaten</p>
                            <p class="text-gray-600 text-sm">Diraih oleh Ananda Sarah (Kelas IX) pada tahun 2024. Pencapaian yang membanggakan!</p>
                        </div>
                    </div>

                    <!-- Prestasi 2 -->
                    <div class="flex items-center bg-white p-6 rounded-lg shadow-md border-l-4 border-secondary">
                        <div class="text-4xl text-accent mr-4">🏆</div>
                        <div>
                            <p class="font-semibold text-lg text-primary">Sekolah Adiwiyata Provinsi</p>
                            <p class="text-gray-600 text-sm">Penghargaan atas komitmen sekolah terhadap pelestarian lingkungan dan budaya hijau.</p>
                        </div>
                    </div>

                    <!-- Prestasi 3 -->
                    <div class="flex items-center bg-white p-6 rounded-lg shadow-md border-l-4 border-secondary">
                        <div class="text-4xl text-accent mr-4">🏅</div>
                        <div>
                            <p class="font-semibold text-lg text-primary">Juara Umum Turnamen Bola Voli SMP Se-Karesidenan</p>
                            <p class="text-gray-600 text-sm">Tim Voli Putra SMPN 02 Tirto tahun 2023, menunjukkan dominasi di bidang olahraga.</p>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Bagian Fasilitas -->
        <section id="fasilitas" class="py-16 bg-white">
            <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
                <h2 class="text-3xl font-bold text-center text-primary mb-12 border-b-2 border-accent inline-block pb-1">
                    Fasilitas Sekolah
                </h2>
                <div class="grid md:grid-cols-2 lg:grid-cols-4 gap-8">

                    <!-- Fasilitas 1: Komputer -->
                    <div class="bg-gray-50 p-6 rounded-xl shadow-lg text-center transform hover:scale-105 transition duration-300">
                        <div class="text-5xl text-primary mb-4">💻</div>
                        <h4 class="text-xl font-bold mb-2">Laboratorium Komputer</h4>
                        <p class="text-gray-700 text-sm">Dilengkapi 30 unit PC dengan akses internet cepat untuk menunjang kegiatan TIK.</p>
                    </div>

                    <!-- Fasilitas 2: IPA -->
                    <div class="bg-gray-50 p-6 rounded-xl shadow-lg text-center transform hover:scale-105 transition duration-300">
                        <div class="text-5xl text-primary mb-4">🔬</div>
                        <h4 class="text-xl font-bold mb-2">Laboratorium IPA</h4>
                        <p class="text-gray-700 text-sm">Alat peraga dan bahan praktikum fisika, kimia, biologi lengkap dan modern.</p>
                    </div>

                    <!-- Fasilitas 3: Perpustakaan -->
                    <div class="bg-gray-50 p-6 rounded-xl shadow-lg text-center transform hover:scale-105 transition duration-300">
                        <div class="text-5xl text-primary mb-4">📚</div>
                        <h4 class="text-xl font-bold mb-2">Perpustakaan Digital</h4>
                        <p class="text-gray-700 text-sm">Koleksi buku cetak dan *e-book* yang memadai serta ruang baca yang nyaman.</p>
                    </div>

                    <!-- Fasilitas 4: Olahraga -->
                    <div class="bg-gray-50 p-6 rounded-xl shadow-lg text-center transform hover:scale-105 transition duration-300">
                        <div class="text-5xl text-primary mb-4">🏀</div>
                        <h4 class="text-xl font-bold mb-2">Lapangan Olahraga</h4>
                        <p class="text-gray-700 text-sm">Lapangan multifungsi untuk basket, voli, dan futsal, mendukung kegiatan fisik siswa.</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Bagian Kontak -->
        <section id="kontak" class="py-16 bg-primary text-white">
            <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
                <h2 class="text-3xl font-bold text-center mb-10 border-b-2 border-accent inline-block pb-1">
                    Hubungi Kami
                </h2>
                <div class="grid md:grid-cols-2 gap-10">
                    <div>
                        <h3 class="text-2xl font-semibold mb-4 text-accent">Informasi Kontak</h3>
                        <p class="mb-2 flex items-center">
                            <!-- Icon Lokasi -->
                            <svg class="w-6 h-6 mr-3 text-secondary" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17.657 16.657L13.414 20.9a1.998 1.998 0 01-2.828 0l-4.243-4.243m11.314 0A8.001 8.001 0 0121 12a8.001 8.001 0 01-16.974 4.657M12 21v-8M15 9a3 3 0 11-6 0 3 3 0 016 0z"></path></svg>
                            Jl. Pendidikan No. 02, Tirto, [Nama Kota]
                        </p>
                        <p class="mb-2 flex items-center">
                            <!-- Icon Email -->
                            <svg class="w-6 h-6 mr-3 text-secondary" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"></path></svg>
                            Email: smpn02tirto@sekolah.id
                        </p>
                        <p class="mb-2 flex items-center">
                            <!-- Icon Telepon -->
                            <svg class="w-6 h-6 mr-3 text-secondary" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 5a2 2 0 012-2h3.28a1 1 0 01.948.684l1.498 4.493a1 1 0 01-.502 1.21l-2.257 1.128a11.056 11.056 0 0010.428 10.428l1.128-2.257a1 1 0 011.21-.502l4.493 1.498a1 1 0 01.684.949V19a2 2 0 01-2 2h-3.28a1 1 0 01-.948-.684l-1.498-4.493a1 1 0 01.502-1.21l2.257-1.128a11.056 11.056 0 00-10.428-10.428z"></path></svg>
                            Telp: (0285) 123456
                        </p>
                    </div>
                    
                    <!-- Form Kontak Sederhana (Opsional) -->
                    <div class="bg-primary/80 p-6 rounded-xl shadow-2xl">
                        <h3 class="text-2xl font-semibold mb-4 text-accent">Kirim Pesan Cepat</h3>
                        <form action="#" method="POST" onsubmit="alert('Pesan berhasil terkirim! (Aksi ini hanya simulasi)'); return false;">
                            <input type="text" placeholder="Nama Anda" class="w-full p-3 mb-4 rounded-md text-gray-800 focus:ring-accent focus:border-accent border-gray-300" required>
                            <textarea placeholder="Pesan Anda..." rows="3" class="w-full p-3 mb-4 rounded-md text-gray-800 focus:ring-accent focus:border-accent border-gray-300" required></textarea>
                            <button type="submit" class="w-full bg-accent text-primary font-bold py-3 rounded-md hover:bg-yellow-400 transition duration-300">
                                Kirim Pesan
                            </button>
                        </form>
                    </div>
                </div>

                <!-- Social Media Icons -->
                <div class="flex justify-center space-x-6 mt-10">
                    <a href="#" class="text-secondary hover:text-white transition duration-300 text-3xl">
                        <!-- Placeholder Icon Instagram (SVG) -->
                        <svg class="w-8 h-8" fill="currentColor" viewBox="0 0 24 24" aria-hidden="true" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M12.315 2c2.43 0 2.723.012 3.696.048 2.043.088 3.105.47 3.845.749a5.152 5.152 0 011.397.915 5.151 5.151 0 01.915 1.397c.279.74.661 1.792.749 3.845.036.973.048 1.266.048 3.696v1.17c0 2.43-.012 2.723-.048 3.696-.088 2.043-.47 3.105-.749 3.845a5.152 5.152 0 01-.915 1.397 5.151 5.151 0 01-1.397.915c-.74.279-1.792.661-3.845.749-.973.036-1.266.048-3.696.048h-1.17c-2.43 0-2.723-.012-3.696-.048-2.043-.088-.47-3.105-.749-3.845a5.152 5.152 0 01-1.397-.915 5.151 5.151 0 01-.915-1.397c-.279-.74-.661-1.792-.749-3.845-.036-.973-.048-1.266-.048-3.696v-1.17c0-2.43.012-2.723.048-3.696.088-2.043.47-3.105.749-3.845a5.152 5.152 0 01.915-1.397 5.151 5.151 0 011.397-.915c.74-.279 1.792-.661 3.845-.749.973-.036 1.266-.048 3.696-.048h1.17zm0 2.375h-1.17c-2.41 0-2.695.012-3.64.048-1.995.085-3.04.455-3.77.725a2.775 2.775 0 00-1.005.697 2.775 2.775 0 00-.697 1.005c-.27.73-.42 1.775-.5 3.77-.036.945-.048 1.23-.048 3.64v1.17c0 2.41.012 2.695.048 3.64.085 1.995.455 3.04.725 3.77.16.425.355.775.697 1.005a2.775 2.775 0 001.005.697c.73.27 1.775.42 3.77.5.945.036 1.23.048 3.64.048h1.17c2.41 0 2.695-.012 3.64-.048 1.995-.085 3.04-.455 3.77-.725.335-.16.685-.355 1.005-.697a2.775 2.775 0 00.697-1.005c.27-.73.42-1.775.5-3.77.036-.945.048-1.23.048-3.64v-1.17c0-2.41-.012-2.695-.048-3.64-.085-1.995-.455-3.04-.725-3.77a2.775 2.775 0 00-.697-1.005 2.775 2.775 0 00-1.005-.697c-.73-.27-1.775-.42-3.77-.5-.945-.036-1.23-.048-3.64-.048zM12 7.765a4.235 4.235 0 110 8.47 4.235 4.235 0 010-8.47zm0 2.375a1.86 1.86 0 100 3.72 1.86 1.86 0 000-3.72zM20.692 7.425a1.144 1.144 0 11-2.288 0 1.144 1.144 0 012.288 0z" clip-rule="evenodd" /></svg>
                    </a>
                    <a href="#" class="text-secondary hover:text-white transition duration-300 text-3xl">
                        <!-- Placeholder Icon Facebook (SVG) -->
                        <svg class="w-8 h-8" fill="currentColor" viewBox="0 0 24 24" aria-hidden="true" xmlns="http://www.w3.org/2000/svg"><path d="M14 10.5h2.5L17 7h-4V5c0-.96.6-1.4 1.45-1.4H17V.45A21.72 21.72 0 0013.9 0C11.35 0 9.5 1.55 9.5 4v3.5H7v3.5h2.5V24h5V10.5z" clip-rule="evenodd" /></svg>
                    </a>
                    <a href="#" class="text-secondary hover:text-white transition duration-300 text-3xl">
                        <!-- Placeholder Icon YouTube (SVG) -->
                        <svg class="w-8 h-8" fill="currentColor" viewBox="0 0 24 24" aria-hidden="true" xmlns="http://www.w3.org/2000/svg"><path d="M22.06 6.88a2.52 2.52 0 00-1.77-1.77C18.59 4.7 12 4.7 12 4.7s-6.59 0-8.29.41A2.52 2.52 0 001.94 6.88c-.41 1.7-.41 5.2-.41 5.2s0 3.5.41 5.2a2.52 2.52 0 001.77 1.77c1.7.41 8.29.41 8.29.41s6.59 0 8.29-.41a2.52 2.52 0 001.77-1.77c.41-1.7.41-5.2.41-5.2s0-3.5-.41-5.2zM9.8 15.5V8.5l6.4 3.5-6.4 3.5z"/></svg>
                    </a>
                </div>
            </div>
        </section>
    </main>

    <!-- Footer -->
    <footer class="bg-gray-800 text-white py-6">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center text-sm">
            <p>&copy; 2025 SMPN 02 Tirto. | Semua Hak Cipta Dilindungi.</p>
            <p class="mt-1 text-gray-400">Dibuat dengan semangat pendidikan.</p>
        </div>
    </footer>

    <!-- JavaScript untuk Navigasi Mobile dan Smooth Scroll -->
    <script>
        document.addEventListener('DOMContentLoaded', () => {
            const menuButton = document.getElementById('menu-button');
            const mobileMenu = document.getElementById('mobile-menu');
            const menuIconOpen = document.getElementById('menu-icon-open');
            const menuIconClose = document.getElementById('menu-icon-close');
            
            // Mengambil semua link navigasi, baik di desktop maupun mobile
            const allNavLinks = document.querySelectorAll('a[href^="#"]');

            // Fungsi untuk mengaktifkan/menonaktifkan menu mobile
            const toggleMenu = () => {
                const isExpanded = menuButton.getAttribute('aria-expanded') === 'true';
                menuButton.setAttribute('aria-expanded', !isExpanded);
                mobileMenu.classList.toggle('hidden');
                menuIconOpen.classList.toggle('hidden');
                menuIconClose.classList.toggle('hidden');

                // Mengunci scroll saat menu terbuka di mobile
                if (!isExpanded) {
                    document.body.classList.add('overflow-hidden');
                } else {
                    document.body.classList.remove('overflow-hidden');
                }
            };

            // Event listener untuk tombol menu
            menuButton.addEventListener('click', toggleMenu);

            // ---------------------------------------------
            // Implementasi SMOOTH SCROLLING
            // ---------------------------------------------
            allNavLinks.forEach(anchor => {
                anchor.addEventListener('click', function (e) {
                    // Hanya berlaku untuk link internal yang dimulai dengan '#'
                    if (this.getAttribute('href').startsWith('#')) {
                        e.preventDefault(); // Mencegah lompatan standar

                        const targetId = this.getAttribute('href');
                        const targetElement = document.querySelector(targetId);

                        if (targetElement) {
                            // Menggunakan metode scrollIntoView dengan behavior 'smooth'
                            targetElement.scrollIntoView({
                                behavior: 'smooth',
                                block: 'start' // Gulir hingga bagian atas elemen target sejajar dengan bagian atas viewport
                            });
                        }
                        
                        // Setelah mengklik, jika ini adalah menu mobile, tutup menu tersebut
                        if (!mobileMenu.classList.contains('hidden') && window.innerWidth < 768) {
                            toggleMenu();
                        }
                    }
                });
            });
        });
    </script>
</body>
</html>
