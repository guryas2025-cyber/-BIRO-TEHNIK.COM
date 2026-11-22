# -BIRO-TEHNIK.COM
<!DOCTYPE html>
<html lang="id" class="scroll-smooth">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>BIRO TEHNIK.COM | Jasa Service Elektronik & Peralatan Rumah Tangga Cianjur</title>
  
  <!-- SEO Dasar -->
  <meta name="description" content="BIRO TEHNIK.COM - Solusi Terpercaya untuk Segala Kebutuhan Service Elektronik Anda di Cianjur & Sukaresmi. Melayani service AC, peralatan dapur, water heater, mesin air, jok kursi, dan peralatan rumah tangga lainnya. Hubungi Dadang Saputra via WhatsApp." />
  <meta name="keywords" content="jasa service elektronik Cianjur, service AC Sukaresmi, service elektronik Cibadak, Biro Tehnik, service water heater Cianjur, service mesin air Sukaresmi, service jok kursi Cianjur, Dadang Saputra" />
  <meta name="author" content="BIRO TEHNIK.COM - Dadang Saputra" />
  <meta name="robots" content="index, follow" />

  <!-- Google Fonts: Inter -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">

  <!-- Tailwind CSS -->
  <script src="https://cdn.tailwindcss.com"></script>
  <script>
    tailwind.config = {
      theme: {
        extend: {
          fontFamily: {
            sans: ['Inter', 'sans-serif'],
          },
          colors: {
            navy: {
              50: '#f0f4f9',
              100: '#dce5f2',
              200: '#b8cbe5',
              300: '#8baad4',
              400: '#5c85be',
              500: '#3965a3',
              600: '#274c82',
              700: '#1d3a66',
              800: '#142a4d',
              900: '#0b1930',
            },
            skytech: {
              50: '#f0f9ff',
              100: '#e0f2fe',
              200: '#bae6fd',
              500: '#0ea5e9',
              600: '#0284c7',
            },
            accent: {
              400: '#fb923c',
              500: '#f97316',
              600: '#ea580c',
            }
          }
        }
      }
    }
  </script>

  <!-- Lucide Icons -->
  <script src="https://unpkg.com/lucide@latest"></script>

  <style>
    /* Kustomisasi scrollbar & animasi halus */
    ::-webkit-scrollbar {
      width: 8px;
    }
    ::-webkit-scrollbar-track {
      background: #f1f5f9;
    }
    ::-webkit-scrollbar-thumb {
      background: #1d3a66;
      border-radius: 4px;
    }
    ::-webkit-scrollbar-thumb:hover {
      background: #0b1930;
    }

    @keyframes pulse-ring {
      0% {
        transform: scale(0.95);
        opacity: 0.75;
      }
      70% {
        transform: scale(1.25);
        opacity: 0;
      }
      100% {
        transform: scale(1.25);
        opacity: 0;
      }
    }
    .wa-pulse::before {
      content: '';
      position: absolute;
      inset: 0;
      border-radius: 9999px;
      background-color: #22c55e;
      z-index: -1;
      animation: pulse-ring 2s infinite;
    }
  </style>
</head>
<body class="font-sans text-slate-700 bg-white antialiased selection:bg-skytech-200 selection:text-navy-900">

  <!-- ================= NAVBAR ================= -->
  <header id="navbar" class="fixed top-0 left-0 right-0 z-50 bg-white/95 backdrop-blur-md border-b border-slate-100 transition-all duration-300">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="flex items-center justify-between h-20">
        <!-- Brand Logo -->
        <a href="#beranda" class="flex items-center gap-3 group">
          <div class="w-11 h-11 rounded-xl bg-navy-900 text-white flex items-center justify-center shadow-md group-hover:bg-accent-500 transition-colors duration-300">
            <i data-lucide="wrench" class="w-6 h-6"></i>
          </div>
          <div>
            <span class="block text-lg sm:text-xl font-extrabold tracking-tight text-navy-900 leading-none">
              BIRO TEHNIK<span class="text-accent-500">.COM</span>
            </span>
            <span class="block text-[11px] font-medium text-slate-500 mt-1">
              Jasa Service Elektronik & Rumah Tangga
            </span>
          </div>
        </a>

        <!-- Desktop Navigation -->
        <nav class="hidden md:flex items-center space-x-8">
          <a href="#beranda" class="nav-link text-sm font-semibold text-navy-900 hover:text-accent-500 transition-colors">Beranda</a>
          <a href="#layanan" class="nav-link text-sm font-semibold text-slate-600 hover:text-accent-500 transition-colors">Layanan</a>
          <a href="#tentang-kami" class="nav-link text-sm font-semibold text-slate-600 hover:text-accent-500 transition-colors">Tentang Kami</a>
          <a href="#jam-operasional" class="nav-link text-sm font-semibold text-slate-600 hover:text-accent-500 transition-colors">Jam Operasional</a>
          <a href="#kontak" class="nav-link text-sm font-semibold text-slate-600 hover:text-accent-500 transition-colors">Kontak</a>
        </nav>

        <!-- Desktop CTA -->
        <div class="hidden md:flex items-center">
          <a href="https://wa.me/6281318308185?text=Halo%20Biro%20Tehnik%2C%20saya%20ingin%20konsultasi%20mengenai%20jasa%20service." 
             target="_blank" 
             rel="noopener noreferrer"
             class="inline-flex items-center gap-2 bg-accent-500 hover:bg-accent-600 text-white text-sm font-semibold px-5 py-2.5 rounded-xl shadow-sm hover:shadow transition-all duration-200">
            <i data-lucide="message-circle" class="w-4 h-4"></i>
            <span>Chat Teknisi</span>
          </a>
        </div>

        <!-- Mobile Menu Button -->
        <div class="md:hidden flex items-center">
          <button id="mobile-menu-btn" aria-label="Buka Menu" class="p-2.5 rounded-xl text-navy-900 hover:bg-slate-100 focus:outline-none transition-colors">
            <i data-lucide="menu" id="menu-icon-open" class="w-6 h-6"></i>
            <i data-lucide="x" id="menu-icon-close" class="w-6 h-6 hidden"></i>
          </button>
        </div>
      </div>
    </div>

    <!-- Mobile Navigation Dropdown -->
    <div id="mobile-menu" class="hidden md:hidden bg-white border-b border-slate-200 px-4 pt-2 pb-6 space-y-2 shadow-lg">
      <a href="#beranda" class="mobile-nav-link block px-4 py-3 rounded-xl text-base font-semibold text-navy-900 hover:bg-skytech-50">Beranda</a>
      <a href="#layanan" class="mobile-nav-link block px-4 py-3 rounded-xl text-base font-semibold text-slate-700 hover:bg-skytech-50">Layanan</a>
      <a href="#tentang-kami" class="mobile-nav-link block px-4 py-3 rounded-xl text-base font-semibold text-slate-700 hover:bg-skytech-50">Tentang Kami</a>
      <a href="#jam-operasional" class="mobile-nav-link block px-4 py-3 rounded-xl text-base font-semibold text-slate-700 hover:bg-skytech-50">Jam Operasional</a>
      <a href="#kontak" class="mobile-nav-link block px-4 py-3 rounded-xl text-base font-semibold text-slate-700 hover:bg-skytech-50">Kontak</a>
      <div class="pt-3 px-2">
        <a href="https://wa.me/6281318308185?text=Halo%20Biro%20Tehnik%2C%20saya%20ingin%20konsultasi%20mengenai%20jasa%20service." 
           target="_blank" 
           rel="noopener noreferrer"
           class="w-full flex items-center justify-center gap-2 bg-accent-500 hover:bg-accent-600 text-white font-semibold py-3.5 px-5 rounded-xl shadow transition-colors">
          <i data-lucide="phone-call" class="w-5 h-5"></i>
          <span>Hubungi Teknisi via WhatsApp</span>
        </a>
      </div>
    </div>
  </header>

  <!-- ================= HERO SECTION ================= -->
  <section id="beranda" class="relative pt-28 pb-16 lg:pt-36 lg:pb-24 bg-gradient-to-br from-navy-900 via-navy-800 to-navy-900 text-white overflow-hidden">
    <!-- Decorative Background Elements -->
    <div class="absolute top-0 right-0 -mr-20 -mt-20 w-96 h-96 rounded-full bg-skytech-500/10 blur-3xl pointer-events-none"></div>
    <div class="absolute bottom-0 left-0 -ml-20 -mb-20 w-80 h-80 rounded-full bg-accent-500/10 blur-3xl pointer-events-none"></div>

    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10">
      <div class="grid grid-cols-1 lg:grid-cols-12 gap-10 lg:gap-12 items-center">
        
        <!-- Left Text Column -->
        <div class="lg:col-span-7 space-y-6 text-center lg:text-left">
          <div class="inline-flex items-center gap-2 px-4 py-2 rounded-full bg-white/10 border border-white/15 text-skytech-200 text-xs sm:text-sm font-medium backdrop-blur-sm">
            <span class="w-2 h-2 rounded-full bg-green-400 animate-pulse"></span>
            <span>Buka Setiap Hari (08.00–16.00 WIB) • Cianjur & Sekitarnya</span>
          </div>

          <div class="space-y-3">
            <p class="text-accent-400 font-bold tracking-wider uppercase text-sm sm:text-base">
              BIRO TEHNIK.COM
            </p>
            <h1 class="text-3xl sm:text-4xl lg:text-5xl font-extrabold leading-tight tracking-tight text-white">
              "Solusi Terpercaya untuk Segala Kebutuhan Service Elektronik Anda"
            </h1>
          </div>

          <p class="text-base sm:text-lg text-slate-200 leading-relaxed max-w-2xl mx-auto lg:mx-0">
            Melayani jasa perbaikan berbagai macam peralatan elektronik, peralatan rumah tangga, AC, water heater, mesin air, service jok kursi, dan berbagai kebutuhan teknis lainnya.
          </p>

          <!-- Action Buttons -->
          <div class="flex flex-col sm:flex-row items-center justify-center lg:justify-start gap-4 pt-2">
            <a href="https://wa.me/6281318308185?text=Halo%20Biro%20Tehnik%2C%20saya%20ingin%20konsultasi%20mengenai%20jasa%20service." 
               target="_blank" 
               rel="noopener noreferrer"
               class="w-full sm:w-auto inline-flex items-center justify-center gap-2.5 bg-accent-500 hover:bg-accent-600 text-white font-bold text-base px-7 py-4 rounded-xl shadow-lg shadow-accent-500/25 hover:-translate-y-0.5 transition-all duration-200">
              <i data-lucide="message-circle" class="w-5 h-5"></i>
              <span>HUBUNGI TEKNISI</span>
            </a>

            <a href="#layanan" 
               class="w-full sm:w-auto inline-flex items-center justify-center gap-2.5 bg-white/10 hover:bg-white/20 text-white border border-white/25 font-semibold text-base px-7 py-4 rounded-xl backdrop-blur-sm transition-all duration-200">
              <span>LIHAT LAYANAN</span>
              <i data-lucide="arrow-down" class="w-5 h-5"></i>
            </a>
          </div>

          <!-- Quick Contact Info -->
          <div class="pt-4 flex flex-wrap items-center justify-center lg:justify-start gap-6 text-sm text-slate-300 border-t border-white/10">
            <div class="flex items-center gap-2">
              <i data-lucide="user-check" class="w-4 h-4 text-skytech-400"></i>
              <span>Teknisi: <strong class="text-white">Dadang Saputra</strong></span>
            </div>
            <div class="flex items-center gap-2">
              <i data-lucide="phone" class="w-4 h-4 text-skytech-400"></i>
              <span>WA: <strong class="text-white">081318308185</strong></span>
            </div>
          </div>
        </div>

        <!-- Right Image Column -->
        <div class="lg:col-span-5">
          <div class="relative mx-auto max-w-md lg:max-w-none">
            <div class="rounded-2xl overflow-hidden shadow-2xl border-4 border-white/15 bg-navy-800 aspect-[4/3] sm:aspect-[16/11] lg:aspect-[4/4]">
              <img 
                src="https://images.unsplash.com/photo-1581092921461-eab62e97a780?auto=format&fit=crop&w=900&q=80" 
                onerror="this.onerror=null;this.src='https://placehold.co/800x800/142a4d/ffffff?text=Teknisi+BIRO+TEHNIK.COM';"
                alt="Teknisi profesional BIRO TEHNIK.COM memperbaiki perangkat elektronik" 
                class="w-full h-full object-cover object-center hover:scale-105 transition-transform duration-700"
              />
            </div>

            <!-- Floating Card Badge -->
            <div class="mt-4 sm:mt-0 sm:absolute sm:-bottom-5 sm:-left-5 bg-white text-navy-900 p-4 rounded-2xl shadow-xl border border-slate-100 flex items-center gap-3.5">
              <div class="w-12 h-12 rounded-xl bg-skytech-100 text-skytech-600 flex items-center justify-center shrink-0">
                <i data-lucide="headphones" class="w-6 h-6"></i>
              </div>
              <div>
                <p class="text-xs font-semibold text-slate-500 uppercase tracking-wide">Konsultasi Langsung</p>
                <p class="text-sm font-bold text-navy-900">Respon Cepat via WhatsApp</p>
              </div>
            </div>
          </div>
        </div>

      </div>
    </div>
  </section>

  <!-- ================= LAYANAN KAMI ================= -->
  <section id="layanan" class="py-16 sm:py-24 bg-slate-50">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <!-- Section Header -->
      <div class="text-center max-w-3xl mx-auto mb-14 space-y-3">
        <span class="inline-block px-3.5 py-1.5 rounded-full bg-skytech-100 text-skytech-600 text-xs font-bold uppercase tracking-wider">
          Daftar Layanan
        </span>
        <h2 class="text-3xl sm:text-4xl font-extrabold text-navy-900 tracking-tight">
          Layanan Perbaikan & Service Kami
        </h2>
        <p class="text-slate-600 text-base sm:text-lg">
          Pilih jenis layanan yang Anda butuhkan dan konsultasikan langsung keluhan perangkat Anda dengan teknisi kami.
        </p>
      </div>

      <!-- Service Cards Grid -->
      <div id="services-grid" class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-7">
        <!-- Kartu layanan akan dirender secara dinamis melalui JavaScript agar rapi dan konsisten -->
      </div>

      <!-- Keterangan Tambahan Layanan -->
      <div class="mt-12 bg-white rounded-2xl p-6 sm:p-8 border border-skytech-200 shadow-sm flex flex-col md:flex-row items-center justify-between gap-6">
        <div class="flex items-start sm:items-center gap-4 text-center sm:text-left flex-col sm:flex-row">
          <div class="w-12 h-12 rounded-xl bg-navy-900 text-white flex items-center justify-center shrink-0 mx-auto sm:mx-0">
            <i data-lucide="wrench" class="w-6 h-6"></i>
          </div>
          <p class="text-navy-900 font-medium text-base sm:text-lg leading-relaxed">
            "Dan menerima berbagai jenis pekerjaan service elektronik lainnya. Silakan konsultasikan kebutuhan Anda kepada teknisi kami."
          </p>
        </div>
        <a href="https://wa.me/6281318308185?text=Halo%20Biro%20Tehnik%2C%20saya%20ingin%20konsultasi%20mengenai%20service%20peralatan%20elektronik%20lainnya." 
           target="_blank" 
           rel="noopener noreferrer"
           class="w-full md:w-auto shrink-0 inline-flex items-center justify-center gap-2 bg-navy-900 hover:bg-navy-800 text-white font-semibold px-6 py-3.5 rounded-xl transition-colors">
          <i data-lucide="message-square" class="w-4 h-4"></i>
          <span>Tanya Teknisi</span>
        </a>
      </div>
    </div>
  </section>

  <!-- ================= KEUNGGULAN KAMI ================= -->
  <section class="py-16 sm:py-24 bg-white border-y border-slate-100">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="text-center max-w-3xl mx-auto mb-14 space-y-3">
        <span class="inline-block px-3.5 py-1.5 rounded-full bg-accent-500/10 text-accent-600 text-xs font-bold uppercase tracking-wider">
          Keunggulan Pelayanan
        </span>
        <h2 class="text-3xl sm:text-4xl font-extrabold text-navy-900 tracking-tight">
          Mengapa Memilih BIRO TEHNIK.COM?
        </h2>
        <p class="text-slate-600 text-base sm:text-lg">
          Kami mengutamakan komunikasi yang jelas dan kemudahan akses bagi setiap pelanggan yang membutuhkan perbaikan.
        </p>
      </div>

      <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-6">
        <!-- Item 1 -->
        <div class="p-6 rounded-2xl bg-slate-50 border border-slate-100 hover:border-skytech-300 hover:shadow-md transition-all duration-300">
          <div class="w-12 h-12 rounded-xl bg-skytech-100 text-skytech-600 flex items-center justify-center mb-4">
            <i data-lucide="cpu" class="w-6 h-6"></i>
          </div>
          <h3 class="text-lg font-bold text-navy-900 mb-2">Melayani Berbagai Jenis Perbaikan Elektronik</h3>
          <p class="text-slate-600 text-sm leading-relaxed">
            Menangani beragam kerusakan peralatan elektronik, mesin air, AC, water heater, peralatan dapur, hingga perbaikan jok kursi dalam satu tempat.
          </p>
        </div>

        <!-- Item 2 -->
        <div class="p-6 rounded-2xl bg-slate-50 border border-slate-100 hover:border-skytech-300 hover:shadow-md transition-all duration-300">
          <div class="w-12 h-12 rounded-xl bg-skytech-100 text-skytech-600 flex items-center justify-center mb-4">
            <i data-lucide="user-check" class="w-6 h-6"></i>
          </div>
          <h3 class="text-lg font-bold text-navy-900 mb-2">Komunikasi Langsung dengan Teknisi</h3>
          <p class="text-slate-600 text-sm leading-relaxed">
            Anda dapat menjelaskan detail keluhan perangkat secara langsung kepada teknisi tanpa perantara yang berbelit.
          </p>
        </div>

        <!-- Item 3 -->
        <div class="p-6 rounded-2xl bg-slate-50 border border-slate-100 hover:border-skytech-300 hover:shadow-md transition-all duration-300">
          <div class="w-12 h-12 rounded-xl bg-skytech-100 text-skytech-600 flex items-center justify-center mb-4">
            <i data-lucide="smile" class="w-6 h-6"></i>
          </div>
          <h3 class="text-lg font-bold text-navy-900 mb-2">Pelayanan Ramah dan Responsif</h3>
          <p class="text-slate-600 text-sm leading-relaxed">
            Setiap pertanyaan dan konsultasi pelanggan dilayani dengan ramah, sopan, dan tanggap sesuai jam operasional kami.
          </p>
        </div>

        <!-- Item 4 -->
        <div class="p-6 rounded-2xl bg-slate-50 border border-slate-100 hover:border-skytech-300 hover:shadow-md transition-all duration-300">
          <div class="w-12 h-12 rounded-xl bg-skytech-100 text-skytech-600 flex items-center justify-center mb-4">
            <i data-lucide="sliders" class="w-6 h-6"></i>
          </div>
          <h3 class="text-lg font-bold text-navy-900 mb-2">Solusi Perbaikan Sesuai Kebutuhan Pelanggan</h3>
          <p class="text-slate-600 text-sm leading-relaxed">
            Penanganan disesuaikan dengan kondisi kerusakan perangkat serta kebutuhan teknis di rumah maupun tempat usaha Anda.
          </p>
        </div>

        <!-- Item 5 -->
        <div class="p-6 rounded-2xl bg-slate-50 border border-slate-100 hover:border-skytech-300 hover:shadow-md transition-all duration-300">
          <div class="w-12 h-12 rounded-xl bg-skytech-100 text-skytech-600 flex items-center justify-center mb-4">
            <i data-lucide="calendar-check" class="w-6 h-6"></i>
          </div>
          <h3 class="text-lg font-bold text-navy-900 mb-2">Jam Pelayanan Setiap Hari</h3>
          <p class="text-slate-600 text-sm leading-relaxed">
            Buka setiap hari dari Senin hingga Minggu pukul 08.00–16.00 WIB sehingga memudahkan Anda mengatur waktu konsultasi.
          </p>
        </div>

        <!-- Item 6 -->
        <div class="p-6 rounded-2xl bg-slate-50 border border-slate-100 hover:border-skytech-300 hover:shadow-md transition-all duration-300">
          <div class="w-12 h-12 rounded-xl bg-skytech-100 text-skytech-600 flex items-center justify-center mb-4">
            <i data-lucide="smartphone" class="w-6 h-6"></i>
          </div>
          <h3 class="text-lg font-bold text-navy-900 mb-2">Mudah Dihubungi Melalui WhatsApp</h3>
          <p class="text-slate-600 text-sm leading-relaxed">
            Cukup satu klik pada tombol WhatsApp yang tersedia untuk langsung terhubung ke nomor 081318308185.
          </p>
        </div>
      </div>
    </div>
  </section>

  <!-- ================= TENTANG KAMI ================= -->
  <section id="tentang-kami" class="py-16 sm:py-24 bg-skytech-50/70">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="grid grid-cols-1 lg:grid-cols-12 gap-10 lg:gap-14 items-center">
        
        <!-- Left Image -->
        <div class="lg:col-span-5">
          <div class="relative rounded-2xl overflow-hidden shadow-xl border-4 border-white aspect-[4/3]">
            <img 
              src="https://images.unsplash.com/photo-1621905251189-08b45d6a269e?auto=format&fit=crop&w=900&q=80" 
              onerror="this.onerror=null;this.src='https://placehold.co/800x600/1d3a66/ffffff?text=Tentang+BIRO+TEHNIK.COM';"
              alt="Peralatan kerja teknisi service elektronik" 
              class="w-full h-full object-cover"
            />
          </div>
        </div>

        <!-- Right Content -->
        <div class="lg:col-span-7 space-y-6">
          <div class="space-y-3">
            <span class="inline-block px-3.5 py-1.5 rounded-full bg-navy-900 text-white text-xs font-bold uppercase tracking-wider">
              Profil Usaha
            </span>
            <h2 class="text-3xl sm:text-4xl font-extrabold text-navy-900 tracking-tight">
              Tentang BIRO TEHNIK.COM
            </h2>
          </div>

          <div class="space-y-4 text-slate-700 text-base sm:text-lg leading-relaxed">
            <p>
              <strong>BIRO TEHNIK.COM</strong> merupakan usaha jasa teknisi yang bergerak di bidang perbaikan dan perawatan berbagai macam peralatan elektronik serta perlengkapan rumah tangga.
            </p>
            <p>
              Kami hadir untuk membantu masyarakat mendapatkan solusi atas berbagai permasalahan kerusakan elektronik, mulai dari peralatan dapur, AC, water heater, mesin air, service jok kursi, hingga berbagai jenis peralatan lainnya.
            </p>
            <p>
              Dengan pelayanan yang ramah dan komunikasi yang mudah, kami siap membantu kebutuhan service Anda.
            </p>
          </div>

          <!-- Owner Info Card -->
          <div class="p-5 rounded-2xl bg-white border border-slate-200 shadow-sm flex flex-col sm:flex-row sm:items-center justify-between gap-4">
            <div class="flex items-center gap-4">
              <div class="w-12 h-12 rounded-full bg-navy-900 text-white flex items-center justify-center font-bold text-lg shrink-0">
                DS
              </div>
              <div>
                <p class="text-xs font-semibold uppercase tracking-wider text-slate-500">Pemilik / Teknisi</p>
                <p class="text-lg font-bold text-navy-900">Dadang Saputra</p>
              </div>
            </div>
            <a href="https://wa.me/6281318308185?text=Halo%20Pak%20Dadang%20(Biro%20Tehnik)%2C%20saya%20ingin%20konsultasi%20service." 
               target="_blank" 
               rel="noopener noreferrer"
               class="inline-flex items-center justify-center gap-2 bg-accent-500 hover:bg-accent-600 text-white text-sm font-semibold px-5 py-3 rounded-xl transition-colors">
              <i data-lucide="message-circle" class="w-4 h-4"></i>
              <span>Hubungi Dadang Saputra</span>
            </a>
          </div>
        </div>

      </div>
    </div>
  </section>

  <!-- ================= JAM OPERASIONAL ================= -->
  <section id="jam-operasional" class="py-16 sm:py-24 bg-white">
    <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="bg-navy-900 rounded-3xl p-6 sm:p-10 lg:p-12 text-white shadow-2xl relative overflow-hidden">
        <!-- Decorative circle -->
        <div class="absolute -top-24 -right-24 w-64 h-64 rounded-full bg-skytech-500/15 blur-2xl pointer-events-none"></div>

        <div class="text-center space-y-3 mb-8 relative z-10">
          <div class="inline-flex items-center gap-2 px-4 py-1.5 rounded-full bg-accent-500 text-white text-xs sm:text-sm font-extrabold tracking-wider uppercase shadow">
            <i data-lucide="clock" class="w-4 h-4"></i>
            <span>BUKA SETIAP HARI</span>
          </div>
          <h2 class="text-2xl sm:text-3xl lg:text-4xl font-extrabold tracking-tight">
            Jadwal & Jam Operasional
          </h2>
          <p class="text-slate-300 text-sm sm:text-base max-w-xl mx-auto">
            Kami siap melayani konsultasi dan pekerjaan service setiap hari dari Senin hingga Minggu.
          </p>
        </div>

        <!-- Schedule List -->
        <div class="bg-white/10 backdrop-blur-md rounded-2xl border border-white/15 divide-y divide-white/10 relative z-10">
          <div class="flex items-center justify-between px-5 sm:px-8 py-3.5">
            <span class="font-semibold text-white">Senin</span>
            <span class="font-bold text-skytech-200">08.00–16.00 WIB</span>
          </div>
          <div class="flex items-center justify-between px-5 sm:px-8 py-3.5">
            <span class="font-semibold text-white">Selasa</span>
            <span class="font-bold text-skytech-200">08.00–16.00 WIB</span>
          </div>
          <div class="flex items-center justify-between px-5 sm:px-8 py-3.5">
            <span class="font-semibold text-white">Rabu</span>
            <span class="font-bold text-skytech-200">08.00–16.00 WIB</span>
          </div>
          <div class="flex items-center justify-between px-5 sm:px-8 py-3.5">
            <span class="font-semibold text-white">Kamis</span>
            <span class="font-bold text-skytech-200">08.00–16.00 WIB</span>
          </div>
          <div class="flex items-center justify-between px-5 sm:px-8 py-3.5">
            <span class="font-semibold text-white">Jumat</span>
            <span class="font-bold text-skytech-200">08.00–16.00 WIB</span>
          </div>
          <div class="flex items-center justify-between px-5 sm:px-8 py-3.5">
            <span class="font-semibold text-white">Sabtu</span>
            <span class="font-bold text-skytech-200">08.00–16.00 WIB</span>
          </div>
          <div class="flex items-center justify-between px-5 sm:px-8 py-3.5">
            <span class="font-semibold text-white">Minggu</span>
            <span class="font-bold text-skytech-200">08.00–16.00 WIB</span>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- ================= KONTAK & LOKASI ================= -->
  <section id="kontak" class="py-16 sm:py-24 bg-slate-50 border-t border-slate-200/70">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="text-center max-w-3xl mx-auto mb-14 space-y-3">
        <span class="inline-block px-3.5 py-1.5 rounded-full bg-skytech-100 text-skytech-600 text-xs font-bold uppercase tracking-wider">
          Kontak & Lokasi Usaha
        </span>
        <h2 class="text-3xl sm:text-4xl font-extrabold text-navy-900 tracking-tight">
          Hubungi Kami
        </h2>
        <p class="text-slate-600 text-base sm:text-lg">
          Silakan hubungi kami melalui WhatsApp atau kunjungi alamat usaha kami untuk informasi dan konsultasi lebih lanjut.
        </p>
      </div>

      <div class="grid grid-cols-1 lg:grid-cols-12 gap-8 items-stretch">
        
        <!-- Contact Details Card -->
        <div class="lg:col-span-5 bg-white rounded-3xl p-6 sm:p-8 shadow-sm border border-slate-200 flex flex-col justify-between space-y-8">
          <div class="space-y-6">
            <div>
              <h3 class="text-2xl font-extrabold text-navy-900">BIRO TEHNIK.COM</h3>
              <p class="text-sm font-semibold text-skytech-600 mt-1">Teknisi: Dadang Saputra</p>
            </div>

            <div class="space-y-5">
              <!-- Alamat -->
              <div class="flex items-start gap-4">
                <div class="w-11 h-11 rounded-xl bg-skytech-100 text-skytech-600 flex items-center justify-center shrink-0 mt-0.5">
                  <i data-lucide="map-pin" class="w-5 h-5"></i>
                </div>
                <div>
                  <p class="text-xs font-bold uppercase tracking-wider text-slate-400">Alamat</p>
                  <p class="text-slate-700 font-medium text-sm sm:text-base leading-relaxed mt-0.5">
                    Kp. Cibadak Warudoyong 002/002, Desa Cibadak, Kecamatan Sukaresmi, Kabupaten Cianjur, Jawa Barat.
                  </p>
                </div>
              </div>

              <!-- WhatsApp -->
              <div class="flex items-start gap-4">
                <div class="w-11 h-11 rounded-xl bg-green-100 text-green-600 flex items-center justify-center shrink-0 mt-0.5">
                  <i data-lucide="phone" class="w-5 h-5"></i>
                </div>
                <div>
                  <p class="text-xs font-bold uppercase tracking-wider text-slate-400">WhatsApp</p>
                  <div class="flex items-center gap-3 mt-0.5">
                    <p class="text-navy-900 font-bold text-lg">081318308185</p>
                    <button type="button" onclick="copyPhoneNumber()" class="text-xs font-semibold px-2.5 py-1 rounded-lg bg-slate-100 hover:bg-slate-200 text-slate-700 transition-colors">
                      Salin
                    </button>
                  </div>
                </div>
              </div>

              <!-- Jam Pelayanan -->
              <div class="flex items-start gap-4">
                <div class="w-11 h-11 rounded-xl bg-accent-500/10 text-accent-600 flex items-center justify-center shrink-0 mt-0.5">
                  <i data-lucide="clock" class="w-5 h-5"></i>
                </div>
                <div>
                  <p class="text-xs font-bold uppercase tracking-wider text-slate-400">Jam Pelayanan</p>
                  <p class="text-slate-700 font-medium text-sm sm:text-base mt-0.5">
                    Setiap hari, 08.00–16.00 WIB.
                  </p>
                </div>
              </div>
            </div>
          </div>

          <!-- Big WhatsApp Button -->
          <div class="pt-2">
            <a href="https://wa.me/6281318308185" 
               target="_blank" 
               rel="noopener noreferrer"
               class="w-full flex items-center justify-center gap-3 bg-accent-500 hover:bg-accent-600 text-white font-extrabold text-base sm:text-lg py-4 px-6 rounded-2xl shadow-lg shadow-accent-500/25 hover:-translate-y-0.5 transition-all duration-200 text-center">
              <i data-lucide="message-circle" class="w-6 h-6 shrink-0"></i>
              <span>HUBUNGI KAMI VIA WHATSAPP</span>
            </a>
          </div>
        </div>

        <!-- Google Maps Embed (Pencarian berdasarkan alamat yang diberikan) -->
        <div class="lg:col-span-7 bg-white rounded-3xl p-3 shadow-sm border border-slate-200 flex flex-col">
          <div class="w-full h-80 sm:h-96 lg:h-full min-h-[340px] rounded-2xl overflow-hidden bg-slate-100 relative">
            <iframe 
              title="Lokasi BIRO TEHNIK.COM - Desa Cibadak, Kecamatan Sukaresmi, Kabupaten Cianjur"
              src="https://maps.google.com/maps?q=Kp.%20Cibadak%20Warudoyong%2C%20Desa%20Cibadak%2C%20Kecamatan%20Sukaresmi%2C%20Kabupaten%20Cianjur%2C%20Jawa%20Barat&t=&z=14&ie=UTF8&iwloc=&output=embed"
              class="w-full h-full border-0"
              loading="lazy"
              referrerpolicy="no-referrer-when-downgrade">
            </iframe>
          </div>
          <div class="pt-3 px-2 pb-1 flex flex-wrap items-center justify-between gap-2 text-xs text-slate-500">
            <span>Area Layanan: Desa Cibadak, Kec. Sukaresmi, Kab. Cianjur</span>
            <a href="https://www.google.com/maps/search/?api=1&query=Kp.+Cibadak+Warudoyong,+Desa+Cibadak,+Kecamatan+Sukaresmi,+Kabupaten+Cianjur,+Jawa+Barat" 
               target="_blank" 
               rel="noopener noreferrer"
               class="inline-flex items-center gap-1 font-semibold text-skytech-600 hover:text-navy-900">
              <span>Buka di Google Maps</span>
              <i data-lucide="external-link" class="w-3.5 h-3.5"></i>
            </a>
          </div>
        </div>

      </div>
    </div>
  </section>

  <!-- ================= FOOTER ================= -->
  <footer class="bg-navy-900 text-slate-300 pt-14 pb-10 border-t border-navy-800">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="grid grid-cols-1 md:grid-cols-12 gap-8 pb-10 border-b border-white/10">
        
        <!-- Brand Info -->
        <div class="md:col-span-5 space-y-4">
          <div class="flex items-center gap-3">
            <div class="w-10 h-10 rounded-xl bg-accent-500 text-white flex items-center justify-center">
              <i data-lucide="wrench" class="w-5 h-5"></i>
            </div>
            <span class="text-xl font-extrabold tracking-tight text-white">
              BIRO TEHNIK<span class="text-accent-400">.COM</span>
            </span>
          </div>
          <p class="text-slate-300 text-sm sm:text-base leading-relaxed">
            "Solusi Service Elektronik dan Peralatan Rumah Tangga Anda."
          </p>
          <p class="text-sm font-semibold text-white">
            Pemilik / Teknisi: Dadang Saputra
          </p>
        </div>

        <!-- Quick Links -->
        <div class="md:col-span-3 space-y-3">
          <h4 class="text-white font-bold text-sm uppercase tracking-wider">Navigasi</h4>
          <ul class="space-y-2 text-sm">
            <li><a href="#beranda" class="hover:text-accent-400 transition-colors">Beranda</a></li>
            <li><a href="#layanan" class="hover:text-accent-400 transition-colors">Layanan</a></li>
            <li><a href="#tentang-kami" class="hover:text-accent-400 transition-colors">Tentang Kami</a></li>
            <li><a href="#jam-operasional" class="hover:text-accent-400 transition-colors">Jam Operasional</a></li>
            <li><a href="#kontak" class="hover:text-accent-400 transition-colors">Kontak</a></li>
          </ul>
        </div>

        <!-- Contact Footer -->
        <div class="md:col-span-4 space-y-3">
          <h4 class="text-white font-bold text-sm uppercase tracking-wider">Alamat & Kontak</h4>
          <p class="text-sm leading-relaxed text-slate-300">
            Kp. Cibadak Warudoyong, Desa Cibadak, Kecamatan Sukaresmi, Kabupaten Cianjur.
          </p>
          <p class="text-sm font-semibold text-white">
            WhatsApp: <a href="https://wa.me/6281318308185" target="_blank" rel="noopener noreferrer" class="text-accent-400 hover:underline">081318308185</a>
          </p>
          <p class="text-xs text-slate-400">
            Buka Setiap Hari: 08.00–16.00 WIB
          </p>
        </div>

      </div>

      <!-- Bottom Copyright -->
      <div class="pt-8 flex flex-col sm:flex-row items-center justify-between gap-4 text-xs sm:text-sm text-slate-400 text-center sm:text-left">
        <p>Copyright © 2026 BIRO TEHNIK.COM. All Rights Reserved.</p>
        <p>Melayani Jasa Service Elektronik & Peralatan Rumah Tangga</p>
      </div>
    </div>
  </footer>

  <!-- ================= FLOATING BUTTONS & TOAST ================= -->
  <!-- Toast Notification (Pengganti alert) -->
  <div id="toast-notification" class="fixed bottom-24 left-1/2 -translate-x-1/2 z-50 bg-navy-900 text-white text-sm font-medium px-5 py-3 rounded-xl shadow-xl border border-white/15 opacity-0 pointer-events-none transition-opacity duration-300">
    Nomor WhatsApp berhasil disalin!
  </div>

  <!-- Back to Top Button -->
  <button id="back-to-top" aria-label="Kembali ke atas" class="fixed bottom-24 right-5 z-40 w-11 h-11 rounded-full bg-navy-900 hover:bg-navy-800 text-white shadow-lg border border-white/15 flex items-center justify-center opacity-0 pointer-events-none transition-all duration-300">
    <i data-lucide="chevron-up" class="w-5 h-5"></i>
  </button>

  <!-- Floating WhatsApp Button -->
  <a href="https://wa.me/6281318308185?text=Halo%20Biro%20Tehnik%2C%20saya%20ingin%20konsultasi%20mengenai%20jasa%20service." 
     target="_blank" 
     rel="noopener noreferrer"
     aria-label="Chat WhatsApp BIRO TEHNIK.COM"
     class="wa-pulse fixed bottom-5 right-5 z-50 flex items-center gap-2.5 bg-green-500 hover:bg-green-600 text-white font-bold px-4 py-3.5 sm:px-5 sm:py-3.5 rounded-full shadow-2xl transition-transform duration-200 hover:scale-105">
    <svg class="w-6 h-6 fill-current shrink-0" viewBox="0 0 24 24" aria-hidden="true">
      <path d="M12.031 6.172c-3.181 0-5.767 2.586-5.768 5.766-.001 1.298.38 2.27 1.019 3.287l-.582 2.128 2.182-.573c.978.58 1.911.928 3.145.929 3.178 0 5.767-2.587 5.768-5.766.001-3.187-2.575-5.77-5.764-5.771zm3.392 8.244c-.144.405-.837.774-1.17.824-.299.045-.677.063-1.092-.069-.252-.08-.575-.187-.988-.365-1.739-.751-2.874-2.502-2.961-2.617-.087-.116-.708-.94-.708-1.793s.448-1.273.607-1.446c.159-.173.346-.217.462-.217l.332.006c.106.005.249-.04.39.298.144.347.491 1.2.534 1.287.043.087.072.188.014.304-.058.116-.087.188-.173.289l-.26.304c-.087.086-.177.18-.076.354.101.174.449.741.964 1.201.662.591 1.221.774 1.394.86s.274.072.376-.043c.101-.116.433-.506.549-.68.116-.173.231-.145.39-.087s1.011.477 1.184.564.289.13.332.202c.045.072.045.419-.1.824zM12 2C6.477 2 2 6.477 2 12c0 1.89.525 3.66 1.438 5.168L2.546 20.2c-.151.512.332.993.844.84l3.025-.903A9.93 9.93 0 0012 22c5.523 0 10-4.477 10-10S17.523 2 12 2z"/>
    </svg>
    <span class="hidden sm:inline text-sm">WhatsApp Teknisi</span>
  </a>

  <!-- ================= JAVASCRIPT ================= -->
  <script>
    // Data 7 Layanan Utama sesuai permintaan
    const servicesData = [
      {
        title: "Service Elektronik",
        description: "Perbaikan berbagai macam peralatan elektronik rumah tangga.",
        icon: "tv",
        image: "https://images.unsplash.com/photo-1597872200969-2b65d56bd16b?auto=format&fit=crop&w=700&q=80",
        fallback: "https://placehold.co/700x450/1d3a66/ffffff?text=Service+Elektronik",
        waMessage: "Halo Biro Tehnik, saya ingin konsultasi mengenai layanan Service Elektronik."
      },
      {
        title: "Service Peralatan Dapur",
        description: "Perbaikan berbagai peralatan dapur elektronik dan perlengkapan memasak.",
        icon: "flame",
        image: "https://images.unsplash.com/photo-1556911220-bff31c812dba?auto=format&fit=crop&w=700&q=80",
        fallback: "https://placehold.co/700x450/1d3a66/ffffff?text=Service+Peralatan+Dapur",
        waMessage: "Halo Biro Tehnik, saya ingin konsultasi mengenai layanan Service Peralatan Dapur."
      },
      {
        title: "Service AC",
        description: "Melayani perbaikan dan penanganan berbagai kerusakan AC.",
        icon: "wind",
        image: "https://images.unsplash.com/photo-1621905252507-b35492cc74b4?auto=format&fit=crop&w=700&q=80",
        fallback: "https://placehold.co/700x450/1d3a66/ffffff?text=Service+AC",
        waMessage: "Halo Biro Tehnik, saya ingin konsultasi mengenai layanan Service AC."
      },
      {
        title: "Service Jok Kursi",
        description: "Melayani perbaikan dan pembenahan jok kursi agar kembali nyaman dan menarik.",
        icon: "armchair",
        image: "https://images.unsplash.com/photo-1555041469-a586c61ea9bc?auto=format&fit=crop&w=700&q=80",
        fallback: "https://placehold.co/700x450/1d3a66/ffffff?text=Service+Jok+Kursi",
        waMessage: "Halo Biro Tehnik, saya ingin konsultasi mengenai layanan Service Jok Kursi."
      },
      {
        title: "Service Water Heater",
        description: "Perbaikan dan penanganan masalah pemanas air.",
        icon: "droplets",
        image: "https://images.unsplash.com/photo-1584622650111-993a426fbf0a?auto=format&fit=crop&w=700&q=80",
        fallback: "https://placehold.co/700x450/1d3a66/ffffff?text=Service+Water+Heater",
        waMessage: "Halo Biro Tehnik, saya ingin konsultasi mengenai layanan Service Water Heater."
      },
      {
        title: "Service Mesin Air",
        description: "Perbaikan pompa air dan berbagai permasalahan mesin air.",
        icon: "gauge",
        image: "https://images.unsplash.com/photo-1504328345606-18bbc8c9d7d1?auto=format&fit=crop&w=700&q=80",
        fallback: "https://placehold.co/700x450/1d3a66/ffffff?text=Service+Mesin+Air",
        waMessage: "Halo Biro Tehnik, saya ingin konsultasi mengenai layanan Service Mesin Air."
      },
      {
        title: "Service Peralatan Rumah Tangga",
        description: "Perbaikan berbagai peralatan elektronik dan kebutuhan rumah tangga lainnya.",
        icon: "home",
        image: "https://images.unsplash.com/photo-1626806787461-102c1bfaaea1?auto=format&fit=crop&w=700&q=80",
        fallback: "https://placehold.co/700x450/1d3a66/ffffff?text=Service+Peralatan+Rumah+Tangga",
        waMessage: "Halo Biro Tehnik, saya ingin konsultasi mengenai layanan Service Peralatan Rumah Tangga."
      }
    ];

    // Render Service Cards
    function renderServiceCards() {
      const grid = document.getElementById('services-grid');
      if (!grid) return;

      grid.innerHTML = servicesData.map(service => {
        const waUrl = `https://wa.me/6281318308185?text=${encodeURIComponent(service.waMessage)}`;
        return `
          <article class="group bg-white rounded-2xl overflow-hidden border border-slate-200/80 shadow-sm hover:shadow-xl hover:-translate-y-1 transition-all duration-300 flex flex-col">
            <div class="relative h-48 overflow-hidden bg-navy-900">
              <img 
                src="${service.image}" 
                onerror="this.onerror=null;this.src='${service.fallback}';"
                alt="${service.title} - BIRO TEHNIK.COM" 
                class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-500"
              />
              <div class="absolute inset-0 bg-gradient-to-t from-navy-900/60 via-transparent to-transparent"></div>
              <div class="absolute bottom-3 left-4 w-11 h-11 rounded-xl bg-white text-navy-900 shadow-md flex items-center justify-center group-hover:bg-accent-500 group-hover:text-white transition-colors duration-300">
                <i data-lucide="${service.icon}" class="w-5 h-5"></i>
              </div>
            </div>

            <div class="p-6 flex-1 flex flex-col justify-between space-y-5">
              <div class="space-y-2">
                <h3 class="text-xl font-bold text-navy-900 group-hover:text-skytech-600 transition-colors">
                  ${service.title}
                </h3>
                <p class="text-slate-600 text-sm leading-relaxed">
                  ${service.description}
                </p>
              </div>

              <a href="${waUrl}" 
                 target="_blank" 
                 rel="noopener noreferrer"
                 class="w-full inline-flex items-center justify-center gap-2 bg-skytech-50 hover:bg-accent-500 text-navy-900 hover:text-white border border-skytech-200 hover:border-accent-500 font-semibold text-sm py-3 px-4 rounded-xl transition-all duration-200">
                <i data-lucide="message-circle" class="w-4 h-4"></i>
                <span>Konsultasi Sekarang</span>
              </a>
            </div>
          </article>
        `;
      }).join('');
    }

    // Salin Nomor Telepon ke Clipboard tanpa alert()
    function copyPhoneNumber() {
      const phone = "081318308185";
      const tempInput = document.createElement("input");
      tempInput.value = phone;
      document.body.appendChild(tempInput);
      tempInput.select();
      try {
        document.execCommand("copy");
        showToast("Nomor WhatsApp 081318308185 berhasil disalin!");
      } catch (err) {
        showToast("Nomor WhatsApp: 081318308185");
      }
      document.body.removeChild(tempInput);
    }

    function showToast(message) {
      const toast = document.getElementById("toast-notification");
      if (!toast) return;
      toast.textContent = message;
      toast.classList.remove("opacity-0");
      toast.classList.add("opacity-100");
      setTimeout(() => {
        toast.classList.remove("opacity-100");
        toast.classList.add("opacity-0");
      }, 2800);
    }

    // Inisialisasi saat halaman dimuat
    document.addEventListener("DOMContentLoaded", () => {
      renderServiceCards();
      lucide.createIcons();

      // Toggle Mobile Menu
      const mobileMenuBtn = document.getElementById("mobile-menu-btn");
      const mobileMenu = document.getElementById("mobile-menu");
      const iconOpen = document.getElementById("menu-icon-open");
      const iconClose = document.getElementById("menu-icon-close");
      const mobileLinks = document.querySelectorAll(".mobile-nav-link");

      function toggleMenu() {
        const isHidden = mobileMenu.classList.contains("hidden");
        if (isHidden) {
          mobileMenu.classList.remove("hidden");
          iconOpen.classList.add("hidden");
          iconClose.classList.remove("hidden");
        } else {
          mobileMenu.classList.add("hidden");
          iconOpen.classList.remove("hidden");
          iconClose.classList.add("hidden");
        }
      }

      if (mobileMenuBtn) {
        mobileMenuBtn.addEventListener("click", toggleMenu);
      }

      mobileLinks.forEach(link => {
        link.addEventListener("click", () => {
          mobileMenu.classList.add("hidden");
          iconOpen.classList.remove("hidden");
          iconClose.classList.add("hidden");
        });
      });

      // Back to Top & Navbar Shadow on Scroll
      const backToTopBtn = document.getElementById("back-to-top");
      const navbar = document.getElementById("navbar");

      window.addEventListener("scroll", () => {
        if (window.scrollY > 300) {
          backToTopBtn.classList.remove("opacity-0", "pointer-events-none");
          backToTopBtn.classList.add("opacity-100");
          navbar.classList.add("shadow-md");
        } else {
          backToTopBtn.classList.add("opacity-0", "pointer-events-none");
          backToTopBtn.classList.remove("opacity-100");
          navbar.classList.remove("shadow-md");
        }
      });

      if (backToTopBtn) {
        backToTopBtn.addEventListener("click", () => {
          window.scrollTo({ top: 0, behavior: "smooth" });
        });
      }
    });
  </script>
</body>
</html>
