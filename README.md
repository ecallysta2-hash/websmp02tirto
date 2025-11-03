<!DOCTYPE html>
<html lang="id" class="scroll-smooth">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Profil Resmi SMPN 02 Tirto</title>
    <!-- Favicon (opsional, ganti dengan logo sekolah) -->
    <link
      rel="icon"
      href="https://placehold.co/32x32/0e7490/ffffff?text=S"
      type="image/png"
    />
    <!-- Tailwind CSS (via CDN) -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Konfigurasi Tailwind (opsional, untuk kustomisasi) -->
    <script>
      tailwind.config = {
        theme: {
          extend: {
            colors: {
              primary: "rgb(14 116 144)", // Cyan-700
              secondary: "rgb(20 184 166)", // Teal-500
            },
            fontFamily: {
              sans: ["Inter", "sans-serif"],
            },
          },
        },
      };
    </script>
    <!-- Font Inter dari Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
    <link
      href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700;800&display=swap"
      rel="stylesheet"
    />
    <!-- Style kustom untuk scrollbar, dll -->
    <style>
      body {
        font-family: "Inter", sans-serif;
      }
      /* Efek smooth pada navbar */
      .navbar-fixed {
        @apply fixed z-[999] bg-white bg-opacity-80 backdrop-blur-sm shadow-md;
        animation: navbar-down 0.5s ease-out;
      }
      @keyframes navbar-down {
        from {
          transform: translateY(-100%);
          opacity: 0;
        }
        to {
          transform: translateY(0);
          opacity: 1;
        }
      }
      /* Tombol hamburger */
      .hamburger-line {
        @apply my-2 block h-[2px] w-[30px] bg-gray-800 transition duration-300 ease-in-out;
      }
      .hamburger-active > span:nth-child(1) {
        @apply -rotate-45;
      }
      .hamburger-active > span:nth-child(2) {
        @apply scale-0;
      }
      .hamburger-active > span:nth-child(3) {
        @apply rotate-45;
      }
    </style>
  </head>

  <body class="bg-white text-gray-800">
    <!-- 
      ================================================================
      HEADER / NAVBAR (Bar di kanan atas)
      Ini adalah bagian yang Anda maksud. Ini tidak saya hilangkan.
      ================================================================
    -->
    <header
      id="beranda"
      class="absolute left-0 top-0 z-10 flex w-full items-center bg-transparent"
    >
      <div class="container mx-auto px-4">
        <div class="relative flex items-center justify-between">
          <!-- Logo -->
          <div class="px-4">
            <a
              href="#beranda"
              class="block py-6 text-lg font-bold text-primary"
              >SMPN 02 TIRTO</a
            >
          </div>
          <!-- Menu & Hamburger -->
          <div class="flex items-center px-4">
            <!-- Tombol Hamburger (Mobile) -->
            <button
              id="hamburger"
              name="hamburger"
              type="button"
              class="absolute right-4 block lg:hidden"
            >
              <span
                class="hamburger-line origin-top-left transition"
              ></span>
              <span class="hamburger-line transition"></span>
              <span
                class="hamburger-line origin-bottom-left transition"
              ></span>
            </button>
            <!-- Menu Navigasi (Desktop) -->
            <nav
              id="nav-menu"
              class="absolute right-4 top-full hidden w-full max-w-[250px] rounded-lg bg-white py-5 shadow-lg lg:static lg:block lg:max-w-full lg:rounded-none lg:bg-transparent lg:shadow-none"
            >
              <ul class="block lg:flex">
                <li class="group">
                  <a
                    href="#beranda"
                    class="mx-8 flex py-2 text-base text-gray-700 group-hover:text-primary"
                    >Beranda</a
                  >
                </li>
                <li class="group">
                  <a
                    href="#ppdb"
                    class="mx-8 flex py-2 text-base text-gray-700 group-hover:text-primary"
                    >INFO PPDB 2025/2026</a
                  >
                </li>
                <li class="group">
                  <a
                    href="#visimisi"
                    class="mx-8 flex py-2 text-base text-gray-700 group-hover:text-primary"
                    >Visi & Misi</a
                  >
                </li>
                <li class="group">
                  <a
                    href="#staff"
                    class="mx-8 flex py-2 text-base text-gray-700 group-hover:text-primary"
                    >Guru</a
                  >
                </li>
                <li class="group">
                  <a
                    href="#kegiatan"
                    class="mx-8 flex py-2 text-base text-gray-700 group-hover:text-primary"
                    >Kegiatan</a
                  >
                </li>
                <li class="group">
                  <a
                    href="#fasilitas"
                    class="mx-8 flex py-2 text-base text-gray-700 group-hover:text-primary"
                    >Fasilitas</a
                  >
                </li>
                <li class="group">
                  <a
                    href="#kontak"
                    class="mx-8 flex py-2 text-base text-gray-700 group-hover:text-primary"
                    >Kontak</a
                  >
                </li>
              </ul>
            </nav>
          </div>
        </div>
      </div>
    </header>

    <!-- Hero/Jumbotron -->
    <section class="relative bg-gray-100 pb-20 pt-36">
      <div class="container mx-auto px-4">
        <div class="flex flex-wrap items-center">
          <!-- Teks Kiri -->
          <div class="w-full self-center px-4 lg:w-1/2">
            <h1 class="text-4xl font-extrabold text-primary md:text-5xl">
              Selamat Datang di SMPN 02 Tirto
            </h1>
            <p class="mb-8 mt-4 text-lg text-gray-600">
              Mencetak generasi cerdas, berakhlak mulia, dan berwawasan global.
            </p>
            <a
              href="#ppdb"
              class="rounded-full bg-primary px-8 py-3 text-base font-semibold text-white transition duration-300 ease-in-out hover:bg-cyan-800 hover:shadow-lg"
            >
              Daftar PPDB Sekarang!
            </a>
          </div>
          <!-- Gambar Kanan -->
          <div class="mt-10 w-full self-end px-4 lg:mt-0 lg:w-1/2">
            <div class="relative">
              <img
                src="https://placehold.co/1200x450/0e7490/ffffff?text=FOTO+GEDUNG+SEKOLAH+SMPN+02+TIRTO"
                alt="Gedung SMPN 02 Tirto"
                class="w-full rounded-lg shadow-lg"
              />
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Info PPDB -->
    <section id="ppdb" class="bg-white py-24">
      <div class="container mx-auto px-4">
        <div class="mx-auto mb-16 max-w-3xl text-center">
          <h2
            class="mb-4 text-3xl font-bold text-primary sm:text-4xl"
          >
            Penerimaan Peserta Didik Baru (PPDB)
          </h2>
          <p class="text-xl font-semibold text-gray-700">
            Tahun Ajaran 2025/2026
          </p>
        </div>

        <div
          class="grid grid-cols-1 gap-8 md:grid-cols-2 lg:grid-cols-3"
        >
          <!-- Card 1: Jadwal -->
          <div
            class="rounded-lg border border-gray-200 bg-gray-50 p-6 shadow-md"
          >
            <div
              class="mb-4 inline-block rounded-full bg-cyan-100 p-3 text-3xl text-primary"
            >
              🗓️
            </div>
            <h3 class="mb-2 text-xl font-semibold">Jadwal Penting</h3>
            <ul class="list-inside list-disc space-y-1 text-gray-600">
              <li>Pendaftaran Online: 1 - 15 Juni 2025</li>
              <li>Verifikasi Dokumen: 16 - 20 Juni 2025</li>
              <li>Pengumuman Hasil: 25 Juni 2025</li>
            </ul>
          </div>
          <!-- Card 2: Syarat -->
          <div
            class="rounded-lg border border-gray-200 bg-gray-50 p-6 shadow-md"
          >
            <div
              class="mb-4 inline-block rounded-full bg-cyan-100 p-3 text-3xl text-primary"
            >
              📄
            </div>
            <h3 class="mb-2 text-xl font-semibold">Persyaratan Umum</h3>
            <ul class="list-inside list-disc space-y-1 text-gray-600">
              <li>Lulusan SD/MI atau sederajat.</li>
              <li>Usia maksimal 15 tahun per 1 Juli 2025.</li>
              <li>Memiliki Akta Kelahiran/Surat Keterangan Lahir.</li>
              <li>Memiliki Kartu Keluarga (KK).</li>
            </ul>
          </div>
          <!-- Card 3: Alur -->
          <div
            class="rounded-lg border border-gray-200 bg-gray-50 p-6 shadow-md"
          >
            <div
              class="mb-4 inline-block rounded-full bg-cyan-100 p-3 text-3xl text-primary"
            >
              ➡️
            </div>
            <h3 class="mb-2 text-xl font-semibold">Alur Pendaftaran</h3>
            <ol class="list-inside list-decimal space-y-1 text-gray-600">
              <li>Buka laman PPDB resmi kota.</li>
              <li>Isi formulir pendaftaran dan unggah berkas.</li>
              <li>Cetak Tanda Bukti Pendaftaran.</li>
              <li>Pantau status verifikasi dan hasil seleksi.</li>
            </ol>
          </div>
        </div>

        <!-- Tombol Aksi PPDB Dihapus -->
        <div class="mt-16 text-center">
          <p class="mt-4 text-gray-600">
            Untuk pertanyaan lebih lanjut, silakan hubungi kontak sekolah kami.
          </p>
        </div>
      </div>
    </section>

    <!-- Visi Misi -->
    <section id="visimisi" class="bg-gray-100 py-24">
      <div class="container mx-auto px-4">
        <div class="mx-auto mb-16 max-w-3xl text-center">
          <h2
            class="mb-4 text-3xl font-bold text-primary sm:text-4xl"
          >
            Visi & Misi
          </h2>
        </div>
        <div class="flex flex-wrap justify-center gap-8">
          <!-- Visi -->
          <div class="w-full lg:w-2/5">
            <div
              class="rounded-lg bg-white p-8 shadow-lg"
              style="min-height: 280px"
            >
              <h3 class="mb-4 text-2xl font-semibold">Visi</h3>
              <blockquote
                class="border-l-4 border-primary pl-4 text-lg italic text-gray-600"
              >
                "Terwujudnya Peserta Didik yang Unggul dalam Prestasi, Berbudaya
                Lingkungan, dan Berlandaskan Iman dan Taqwa."
              </blockquote>
            </div>
          </div>
          <!-- Misi -->
          <div class="w-full lg:w-2/5">
            <div
              class="rounded-lg bg-white p-8 shadow-lg"
              style="min-height: 280px"
            >
              <h3 class="mb-4 text-2xl font-semibold">Misi</h3>
              <ul class="space-y-2 text-gray-600">
                <li class="flex items-start">
                  <span class="mr-2 text-primary">✓</span>
                  <span>
                    Meningkatkan mutu pembelajaran dan pembinaan secara efektif.
                  </span>
                </li>
                <li class="flex items-start">
                  <span class="mr-2 text-primary">✓</span>
                  <span>
                    Mengembangkan potensi diri peserta didik di bidang akademik
                    dan non-akademik.
                  </span>
                </li>
                <li class="flex items-start">
                  <span class="mr-2 text-primary">✓</span>
                  <span> Membentuk karakter religius dan mandiri. </span>
                </li>
                <li class="flex items-start">
                  <span class="mr-2 text-primary">✓</span>
                  <span>
                    Menciptakan lingkungan sekolah yang bersih, indah, dan
                    nyaman.
                  </span>
                </li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Staf Pengajar -->
    <section id="staff" class="bg-white py-24">
      <div class="container mx-auto px-4">
        <div class="mx-auto mb-16 max-w-3xl text-center">
          <h2
            class="mb-4 text-3xl font-bold text-primary sm:text-4xl"
          >
            Staf Pengajar (Guru)
          </h2>
        </div>
        <!-- Daftar Guru -->
        <div
          class="grid grid-cols-1 gap-8 sm:grid-cols-2 lg:grid-cols-4"
        >
          <!-- Guru 1 -->
          <div
            class="transform rounded-lg bg-gray-50 p-6 text-center shadow-md transition duration-300 hover:scale-105 hover:shadow-xl"
          >
            <img
              src="https://placehold.co/120x120/0e7490/ffffff?text=Bapak"
              alt="Foto Bapak Budi Santoso"
              class="mx-auto mb-4 h-32 w-32 rounded-full border-4 border-white object-cover shadow-md"
            />
            <h4 class="text-xl font-semibold text-primary">
              Bapak Budi Santoso
            </h4>
            <p class="text-gray-600">Kepala Sekolah</p>
            <p class="text-sm text-gray-500">Pendidikan Agama</p>
          </div>
          <!-- Guru 2 -->
          <div
            class="transform rounded-lg bg-gray-50 p-6 text-center shadow-md transition duration-300 hover:scale-105 hover:shadow-xl"
          >
            <img
              src="https://placehold.co/120x120/14b8a6/ffffff?text=Ibu"
              alt="Foto Ibu Siti Aminah"
              class="mx-auto mb-4 h-32 w-32 rounded-full border-4 border-white object-cover shadow-md"
            />
            <h4 class="text-xl font-semibold text-primary">
              Ibu Siti Aminah
            </h4>
            <p class="text-gray-600">Guru Matematika</p>
            <p class="text-sm text-gray-500">Wali Kelas IX-A</p>
          </div>
          <!-- Guru 3 -->
          <div
            class="transform rounded-lg bg-gray-50 p-6 text-center shadow-md transition duration-300 hover:scale-105 hover:shadow-xl"
          >
            <img
              src="https://placehold.co/120x120/0e7490/ffffff?text=Bapak"
              alt="Foto Bapak Joko Susilo"
              class="mx-auto mb-4 h-32 w-32 rounded-full border-4 border-white object-cover shadow-md"
            />
            <h4 class="text-xl font-semibold text-primary">
              Bapak Joko Susilo
            </h4>
            <p class="text-gray-600">Guru Bahasa Inggris</p>
            <p class="text-sm text-gray-500">Pembina OSIS</p>
          </div>
          <!-- Guru 4 -->
          <div
            class="transform rounded-lg bg-gray-50 p-6 text-center shadow-md transition duration-300 hover:scale-105 hover:shadow-xl"
          >
            <img
              src="https://placehold.co/120x120/14b8a6/ffffff?text=Ibu"
              alt="Foto Ibu Rina Dewi"
              class="mx-auto mb-4 h-32 w-32 rounded-full border-4 border-white object-cover shadow-md"
            />
            <h4 class="text-xl font-semibold text-primary">
              Ibu Rina Dewi
            </h4>
            <p class="text-gray-600">Guru IPA</p>
            <p class="text-sm text-gray-500">Koordinator Lab</p>
          </div>

          <!-- Staf Tambahan (Awalnya Tersembunyi) -->
          <!-- Guru 5 (Tersembunyi) -->
          <div
            class="staff-tambahan hidden transform rounded-lg bg-gray-50 p-6 text-center shadow-md transition duration-300 hover:scale-105 hover:shadow-xl"
          >
            <img
              src="https://placehold.co/120x120/0e7490/ffffff?text=Bapak"
              alt="Foto Bapak Ahmad"
              class="mx-auto mb-4 h-32 w-32 rounded-full border-4 border-white object-cover shadow-md"
            />
            <h4 class="text-xl font-semibold text-primary">
              Bapak Ahmad Hidayat
            </h4>
            <p class="text-gray-600">Guru IPS</p>
            <p class="text-sm text-gray-500">Wali Kelas VIII-B</p>
          </div>
          <!-- Guru 6 (Tersembunyi) -->
          <div
            class="staff-tambahan hidden transform rounded-lg bg-gray-50 p-6 text-center shadow-md transition duration-300 hover:scale-105 hover:shadow-xl"
          >
            <img
              src="https://placehold.co/120x120/14b8a6/ffffff?text=Ibu"
              alt="Foto Ibu Wulan"
              class="mx-auto mb-4 h-32 w-32 rounded-full border-4 border-white object-cover shadow-md"
            />
            <h4 class="text-xl font-semibold text-primary">
              Ibu Wulan Sari
            </h4>
            <p class="text-gray-600">Guru Bahasa Indonesia</p>
            <p class="text-sm text-gray-500">Pembina Mading</p>
          </div>
          <!-- Guru 7 (Tersembunyi) -->
          <div
            class="staff-tambahan hidden transform rounded-lg bg-gray-50 p-6 text-center shadow-md transition duration-300 hover:scale-105 hover:shadow-xl"
          >
            <img
              src="https://placehold.co/120x120/0e7490/ffffff?text=Bapak"
              alt="Foto Bapak Eko"
              class="mx-auto mb-4 h-32 w-32 rounded-full border-4 border-white object-cover shadow-md"
            />
            <h4 class="text-xl font-semibold text-primary">
              Bapak Eko Prasetyo
            </h4>
            <p class="text-gray-600">Guru PJOK</p>
            <p class="text-sm text-gray-500">Pelatih Futsal</p>
          </div>
          <!-- Guru 8 (Tersembunyi) -->
          <div
            class="staff-tambahan hidden transform rounded-lg bg-gray-50 p-6 text-center shadow-md transition duration-300 hover:scale-105 hover:shadow-xl"
          >
            <img
              src="https://placehold.co/120x120/14b8a6/ffffff?text=Ibu"
              alt="Foto Ibu Dewi"
              class="mx-auto mb-4 h-32 w-32 rounded-full border-4 border-white object-cover shadow-md"
            />
            <h4 class="text-xl font-semibold text-primary">
              Ibu Dewi Lestari
            </h4>
            <p class="text-gray-600">Guru Seni Budaya</p>
            <p class="text-sm text-gray-500">Pelatih Tari</p>
          </div>
        </div>

        <!-- Tombol Aksi Staf -->
        <div class="mt-16 text-center">
          <button
            id="tombol-staff"
            type="button"
            class="rounded-full bg-primary px-10 py-4 text-lg font-semibold text-white transition duration-300 ease-in-out hover:bg-cyan-800 hover:shadow-lg"
          >
            Lihat Daftar Lengkap Staf Pengajar
          </button>
        </div>
      </div>
    </section>

    <!-- Kegiatan / Ekstrakurikuler -->
    <section id="kegiatan" class="bg-gray-100 py-24">
      <div class="container mx-auto px-4">
        <div class="mx-auto mb-16 max-w-3xl text-center">
          <h2
            class="mb-4 text-3xl font-bold text-primary sm:text-4xl"
          >
            Kegiatan & Ekstrakurikuler
          </h2>
        </div>
        <div
          class="grid grid-cols-1 gap-8 md:grid-cols-2 lg:grid-cols-3"
        >
          <!-- Kegiatan 1 -->
          <div class="rounded-lg bg-white p-6 shadow-md">
            <div
              class="mb-4 inline-block rounded-full bg-cyan-100 p-3 text-3xl text-primary"
            >
              ⚽
            </div>
            <h3 class="mb-2 text-xl font-semibold">
              Ekstrakurikuler Futsal
            </h3>
            <p class="text-gray-600">
              Tim futsal sekolah rutin berlatih dan mengikuti kompetisi antar
              sekolah di tingkat kabupaten, menumbuhkan jiwa sportivitas.
            </p>
          </div>
          <!-- Kegiatan 2 -->
          <div class="rounded-lg bg-white p-6 shadow-md">
            <div
              class="mb-4 inline-block rounded-full bg-cyan-100 p-3 text-3xl text-primary"
            >
              🎨
            </div>
            <h3 class="mb-2 text-xl font-semibold">Pentas Seni Tahunan</h3>
            <p class="text-gray-600">
              Acara tahunan menampilkan bakat siswa dalam seni tari, musik,
              drama, dan paduan suara, wadah kreativitas tanpa batas.
            </p>
          </div>
          <!-- Kegiatan 3 -->
          <div class="rounded-lg bg-white p-6 shadow-md">
            <div
              class="mb-4 inline-block rounded-full bg-cyan-100 p-3 text-3xl text-primary"
            >
              🌿
            </div>
            <h3 class="mb-2 text-xl font-semibold">
              Jum'at Bersih dan Hijau
            </h3>
            <p class="text-gray-600">
              Kegiatan rutin untuk menanam dan merawat taman sekolah, mendukung
              program sekolah Adiwiyata dan peduli lingkungan.
            </p>
          </div>
        </div>
      </div>
    </section>

    <!-- Prestasi -->
    <section id="prestasi" class="bg-white py-24">
      <div class="container mx-auto px-4">
        <div class="mx-auto mb-16 max-w-3xl text-center">
          <h2
            class="mb-4 text-3xl font-bold text-primary sm:text-4xl"
          >
            Prestasi Sekolah & Siswa
          </h2>
        </div>
        <div
          class="grid grid-cols-1 gap-8 md:grid-cols-2 lg:grid-cols-3"
        >
          <!-- Prestasi 1 -->
          <div
            class="rounded-lg border-l-4 border-primary bg-gray-50 p-6 shadow-sm"
          >
            <div class="mb-2 text-3xl">🥇</div>
            <h3 class="text-lg font-semibold">
              Juara 1 Lomba Sains Tingkat Kabupaten
            </h3>
            <p class="text-sm text-gray-600">
              Diraih oleh Ananda Sarah (Kelas IX) pada tahun 2024. Pencapaian
              yang membanggakan!
            </p>
          </div>
          <!-- Prestasi 2 -->
          <div
            class="rounded-lg border-l-4 border-primary bg-gray-50 p-6 shadow-sm"
          >
            <div class="mb-2 text-3xl">🏆</div>
            <h3 class="text-lg font-semibold">Sekolah Adiwiyata Provinsi</h3>
            <p class="text-sm text-gray-600">
              Penghargaan atas komitmen sekolah terhadap pelestarian lingkungan
              dan budaya hijau.
            </p>
          </div>
          <!-- Prestasi 3 -->
          <div
            class="rounded-lg border-l-4 border-primary bg-gray-50 p-6 shadow-sm"
          >
            <div class="mb-2 text-3xl">🏅</div>
            <h3 class="text-lg font-semibold">
              Juara Umum Turnamen Bola Voli SMP Se-Karesidenan
            </h3>
            <p class="text-sm text-gray-600">
              Tim Voli Putra SMPN 02 Tirto tahun 2023, menunjukkan dominasi di
              bidang olahraga.
            </p>
          </div>
        </div>
      </div>
    </section>

    <!-- Fasilitas -->
    <section id="fasilitas" class="bg-gray-100 py-24">
      <div class="container mx-auto px-4">
        <div class="mx-auto mb-16 max-w-3xl text-center">
          <h2
            class="mb-4 text-3xl font-bold text-primary sm:text-4xl"
          >
            Fasilitas Sekolah
          </h2>
        </div>
        <div
          class="grid grid-cols-1 gap-8 md:grid-cols-2 lg:grid-cols-4"
        >
          <!-- Fasilitas 1 -->
          <div class="rounded-lg bg-white p-6 shadow-md">
            <div
              class="mb-4 inline-block rounded-full bg-cyan-100 p-3 text-3xl text-primary"
            >
              💻
            </div>
            <h3 class="mb-2 text-xl font-semibold">
              Laboratorium Komputer
            </h3>
            <p class="text-gray-600">
              Dilengkapi 30 unit PC dengan akses internet cepat untuk menunjang
              kegiatan TIK.
            </p>
          </div>
          <!-- Fasilitas 2 -->
          <div class="rounded-lg bg-white p-6 shadow-md">
            <div
              class="mb-4 inline-block rounded-full bg-cyan-100 p-3 text-3xl text-primary"
            >
              🔬
            </div>
            <h3 class="mb-2 text-xl font-semibold">Laboratorium IPA</h3>
            <p class="text-gray-600">
              Alat peraga dan bahan praktikum fisika, kimia, biologi lengkap dan
              modern.
            </p>
          </div>
          <!-- Fasilitas 3 -->
          <div class="rounded-lg bg-white p-6 shadow-md">
            <div
              class="mb-4 inline-block rounded-full bg-cyan-100 p-3 text-3xl text-primary"
            >
              📚
            </div>
            <h3 class="mb-2 text-xl font-semibold">Perpustakaan Digital</h3>
            <p class="text-gray-600">
              Koleksi buku cetak dan *e-book* yang memadai serta ruang baca yang
              nyaman.
            </SA>
          </div>
          <!-- Fasilitas 4 -->
          <div class="rounded-lg bg-white p-6 shadow-md">
            <div
              class="mb-4 inline-block rounded-full bg-cyan-100 p-3 text-3xl text-primary"
            >
              🏀
            </div>
            <h3 class="mb-2 text-xl font-semibold">Lapangan Olahraga</h3>
            <p class="text-gray-600">
              Lapangan multifungsi untuk basket, voli, dan futsal, mendukung
              kegiatan fisik siswa.
            </p>
          </div>
        </div>
      </div>
    </section>

    <!-- Kontak -->
    <section id="kontak" class="bg-primary py-24 text-white">
      <div class="container mx-auto px-4">
        <div class="mx-auto mb-16 max-w-3xl text-center">
          <h2 class="mb-4 text-3xl font-bold sm:text-4xl">
            Hubungi Kami
          </h2>
        </div>
        <div
          class="flex flex-wrap rounded-lg bg-white/10 p-8 shadow-xl backdrop-blur-sm"
        >
          <!-- Info Kiri -->
          <div class="w-full lg:w-1/2">
            <h3 class="mb-6 text-2xl font-semibold">Informasi Kontak</h3>
            <div class="mb-4 flex items-start">
              <span class="mr-4 text-2xl">📍</span>
              <div>
                <h4 class="font-semibold">Alamat</h4>
                <p>
                  Jl. Pendidikan No. 02, Tirto, [Nama Kota]
                </p>
              </div>
            </div>
            <div class="mb-4 flex items-start">
              <span class="mr-4 text-2xl">✉️</span>
              <div>
                <h4 class="font-semibold">Email</h4>
                <p>smpn02tirto@sekolah.id</p>
              </div>
            </div>
            <div class="mb-4 flex items-start">
              <span class="mr-4 text-2xl">📞</span>
              <div>
                <h4 class="font-semibold">Telepon</h4>
                <p>(0285) 123456</p>
              </div>
            </div>
          </div>
          <!-- Form Kanan -->
          <div class="mt-10 w-full lg:mt-0 lg:w-1/2">
            <h3 class="mb-6 text-2xl font-semibold">Kirim Pesan Cepat</h3>
            <form action="#" method="POST">
              <div class="mb-4">
                <label for="nama" class="mb-2 block">Nama Lengkap</label>
                <input
                  type="text"
                  id="nama"
                  name="nama"
                  class="w-full rounded-md bg-white/20 px-4 py-2 text-white placeholder-gray-300 focus:outline-none focus:ring-2 focus:ring-white"
                  placeholder="Nama Anda"
                />
              </div>
              <div class="mb-4">
                <label for="email" class="mb-2 block">Email</label>
                <input
                  type;
                  "email"
                  id="email"
                  name="email"
                  class="w-full rounded-md bg-white/20 px-4 py-2 text-white placeholder-gray-300 focus:outline-none focus:ring-2 focus:ring-white"
                  placeholder="email@anda.com"
                />
              </div>
              <div class="mb-4">
                <label for="pesan" class="mb-2 block">Pesan</label>
                <textarea
                  id="pesan"
                  name="pesan"
                  rows="4"
                  class="w-full rounded-md bg-white/20 px-4 py-2 text-white placeholder-gray-300 focus:outline-none focus:ring-2 focus:ring-white"
                  placeholder="Tuliskan pesan Anda..."
                ></textarea>
              </div>
              <div>
                <button
                  type="submit"
                  class="rounded-full bg-white px-8 py-3 font-semibold text-primary transition duration-300 ease-in-out hover:bg-gray-200"
                >
                  Kirim Pesan
                </button>
              </div>
            </form>
          </div>
        </div>
      </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-800 py-8 text-center text-gray-400">
      <div class="container mx-auto px-4">
        <p>© 2025 SMPN 02 Tirto. | Semua Hak Cipta Dilindungi.</p>
        <p class="text-sm">Dibuat dengan semangat pendidikan.</p>
      </div>
    </footer>

    <!-- Skrip JavaScript -->
    <script>
      // Efek Navbar Fixed saat di-scroll
      window.onscroll = function () {
        const header = document.querySelector("header");
        const fixedNav = header.offsetTop;

        if (window.pageYOffset > fixedNav) {
          header.classList.add("navbar-fixed");
        } else {
          header.classList.remove("navbar-fixed");
        }
      };

      // Logika Tombol Hamburger
      const hamburger = document.querySelector("#hamburger");
      const navMenu = document.querySelector("#nav-menu");

      hamburger.addEventListener("click", function () {
        hamburger.classList.toggle("hamburger-active");
        navMenu.classList.toggle("hidden");
      });

      // Klik di luar hamburger
      window.addEventListener("click", function (e) {
        if (
          e.target != hamburger &&
          !hamburger.contains(e.target) &&
          e.target != navMenu &&
          !navMenu.contains(e.target)
        ) {
          hamburger.classList.remove("hamburger-active");
          navMenu.classList.add("hidden");
        }
      });

      // Logika untuk tombol "Lihat Staf"
      const tombolStaff = document.querySelector("#tombol-staff");
      const staffTambahan = document.querySelectorAll(".staff-tambahan");

      tombolStaff.addEventListener("click", function () {
        // Toggle (perlihatkan/sembunyikan) setiap kartu staf tambahan
        staffTambahan.forEach(function (staff) {
          staff.classList.toggle("hidden");
        });

        // Cek status setelah di-toggle
        // Kita cek elemen pertama saja sebagai referensi
        const isHidden = staffTambahan[0].classList.contains("hidden");

        // Ubah teks tombol berdasarkan status
        if (isHidden) {
          tombolStaff.textContent = "Lihat Daftar Lengkap Staf Pengajar";
        } else {
          tombolStaff.textContent = "Sembunyikan Daftar";
        }
      });
    </script>
  </body>
</html>

