<!DOCTYPE html>
<html lang="ms" class="dark scroll-smooth">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Esport Tour Smart Ummah Perak Tengah 2026</title>
  
  <!-- Tailwind CSS -->
  <script src="https://cdn.tailwindcss.com"></script>
  <script>
    tailwind.config = {
      darkMode: 'class',
      theme: {
        extend: {
          colors: {
            brand: {
              dark: '#080d16',
              card: '#111827',
              border: '#1f293d',
              emerald: '#10b981',
              emeraldHover: '#059669',
              gold: '#fbbf24',
              goldDark: '#d97706',
              cyan: '#06b6d4'
            }
          },
          fontFamily: {
            heading: ['Orbitron', 'sans-serif'],
            body: ['Plus Jakarta Sans', 'sans-serif']
          }
        }
      }
    }
  </script>

  <!-- Google Fonts -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@500;700;800;900&family=Plus+Jakarta+Sans:wght@400;500;600;700;800&display=swap" rel="stylesheet">
  
  <!-- Font Awesome -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

  <style>
    body {
      font-family: 'Plus Jakarta Sans', sans-serif;
      background-color: #080d16;
      color: #f3f4f6;
    }
    .font-heading {
      font-family: 'Orbitron', sans-serif;
    }
    .glow-emerald {
      box-shadow: 0 0 25px rgba(16, 185, 129, 0.25);
    }
    .glow-gold {
      box-shadow: 0 0 25px rgba(251, 191, 36, 0.25);
    }
    .bg-grid-pattern {
      background-image: radial-gradient(rgba(16, 185, 129, 0.12) 1px, transparent 0);
      background-size: 24px 24px;
    }
    .glass-panel {
      background: rgba(17, 24, 39, 0.75);
      backdrop-filter: blur(12px);
      border: 1px solid rgba(255, 255, 255, 0.08);
    }
    /* Custom Scrollbar */
    ::-webkit-scrollbar {
      width: 8px;
    }
    ::-webkit-scrollbar-track {
      background: #080d16;
    }
    ::-webkit-scrollbar-thumb {
      background: #1f293d;
      border-radius: 4px;
    }
    ::-webkit-scrollbar-thumb:hover {
      background: #10b981;
    }
  </style>
</head>
<body class="bg-brand-dark text-gray-100 min-h-screen flex flex-col selection:bg-brand-emerald selection:text-black">

  <!-- HEADER / NAVBAR -->
  <header class="sticky top-0 z-40 w-full glass-panel border-b border-gray-800/80">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 h-20 flex items-center justify-between">
      
      <!-- Logo & Branding -->
      <a href="#" class="flex items-center gap-3 group">
        <div class="w-12 h-12 rounded-xl bg-gradient-to-br from-brand-emerald via-teal-500 to-brand-gold p-0.5 shadow-lg group-hover:scale-105 transition-transform duration-300">
          <div class="w-full h-full bg-brand-dark rounded-[10px] flex items-center justify-center">
            <i class="fa-solid fa-gamepad text-brand-emerald text-xl group-hover:text-brand-gold transition-colors"></i>
          </div>
        </div>
        <div class="flex flex-col">
          <span class="font-heading font-black text-lg tracking-wider text-white leading-tight">
            SMART<span class="text-brand-emerald">UMMAH</span>
          </span>
          <span class="text-[10px] tracking-widest uppercase text-brand-gold font-bold">
            Perak Tengah 2026
          </span>
        </div>
      </a>

      <!-- Desktop Navigation -->
      <nav class="hidden md:flex items-center gap-6 text-sm font-semibold text-gray-300">
        <a href="#info" class="hover:text-brand-emerald transition-colors">Info</a>
        <a href="#kategori" class="hover:text-brand-emerald transition-colors">Kategori & Yuran</a>
        <a href="#format" class="hover:text-brand-emerald transition-colors">Format & Peraturan</a>
        <a href="#cara-daftar" class="hover:text-brand-emerald transition-colors">Cara Daftar</a>
        <a href="#faq" class="hover:text-brand-emerald transition-colors">FAQ</a>
        <a href="#hubungi" class="hover:text-brand-emerald transition-colors">Hubungi</a>
      </nav>

      <!-- Action Buttons -->
      <div class="flex items-center gap-3">
        <button onclick="toggleAdminModal()" class="px-3 py-1.5 text-xs font-bold rounded-lg border border-brand-emerald/40 text-brand-emerald hover:bg-brand-emerald/10 transition flex items-center gap-2">
          <i class="fa-solid fa-user-shield"></i>
          <span class="hidden sm:inline">Admin</span>
        </button>
        <a href="#pendaftaran" class="px-4 py-2 text-xs sm:text-sm font-bold rounded-lg bg-gradient-to-r from-brand-emerald to-teal-500 text-black shadow-lg hover:brightness-110 active:scale-95 transition-all flex items-center gap-2">
          <i class="fa-solid fa-bolt"></i>
          <span>DAFTAR</span>
        </a>
        <!-- Mobile Menu Toggle -->
        <button id="mobileMenuBtn" onclick="toggleMobileMenu()" class="md:hidden text-gray-300 hover:text-white p-2">
          <i class="fa-solid fa-bars text-xl"></i>
        </button>
      </div>
    </div>

    <!-- Mobile Navigation Dropdown -->
    <div id="mobileMenu" class="hidden md:hidden bg-brand-card/95 border-b border-gray-800 px-4 pt-2 pb-6 space-y-3 font-medium">
      <a href="#info" onclick="toggleMobileMenu()" class="block py-2 text-gray-300 hover:text-brand-emerald border-b border-gray-800">Info Pertandingan</a>
      <a href="#kategori" onclick="toggleMobileMenu()" class="block py-2 text-gray-300 hover:text-brand-emerald border-b border-gray-800">Kategori & Yuran</a>
      <a href="#format" onclick="toggleMobileMenu()" class="block py-2 text-gray-300 hover:text-brand-emerald border-b border-gray-800">Format & Peraturan</a>
      <a href="#cara-daftar" onclick="toggleMobileMenu()" class="block py-2 text-gray-300 hover:text-brand-emerald border-b border-gray-800">Cara Pendaftaran</a>
      <a href="#faq" onclick="toggleMobileMenu()" class="block py-2 text-gray-300 hover:text-brand-emerald border-b border-gray-800">Soalan Lazim (FAQ)</a>
      <a href="#hubungi" onclick="toggleMobileMenu()" class="block py-2 text-gray-300 hover:text-brand-emerald">Hubungi Admin</a>
    </div>
  </header>

  <main class="flex-grow">
    <!-- HERO SECTION -->
    <section class="relative min-h-[90vh] flex items-center justify-center py-16 px-4 overflow-hidden bg-grid-pattern">
      <!-- Ambient Glow Effects -->
      <div class="absolute top-1/4 left-1/2 -translate-x-1/2 -translate-y-1/2 w-96 h-96 bg-brand-emerald/15 rounded-full blur-3xl pointer-events-none"></div>
      <div class="absolute bottom-10 right-10 w-80 h-80 bg-brand-gold/10 rounded-full blur-3xl pointer-events-none"></div>

      <div class="max-w-5xl mx-auto text-center relative z-10 space-y-8">
        
        <!-- Organizer Badges -->
        <div class="inline-flex flex-wrap items-center justify-center gap-2 px-4 py-2 rounded-full glass-panel border border-brand-emerald/30 text-xs sm:text-sm font-semibold">
          <span class="text-brand-gold flex items-center gap-1.5">
            <i class="fa-solid fa-trophy"></i> Sempena Hari Sukan Negara 2026
          </span>
          <span class="text-gray-500">•</span>
          <span class="text-gray-300">Anjuran: Majlis Belia Negeri Perak & MBD Perak Tengah</span>
        </div>

        <!-- Main Heading -->
        <div class="space-y-3">
          <h1 class="font-heading text-3xl sm:text-5xl lg:text-6xl font-black tracking-tight text-white uppercase leading-tight">
            ESPORT TOUR <span class="bg-gradient-to-r from-brand-emerald via-teal-300 to-brand-gold bg-clip-text text-transparent">SMART UMMAH</span><br>
            DAERAH PERAK TENGAH 2026
          </h1>
          <p class="font-heading text-lg sm:text-2xl text-brand-gold tracking-widest font-bold uppercase italic">
            "Battle. Compete. Champion."
          </p>
        </div>

        <!-- Key Details Grid -->
        <div class="grid grid-cols-1 sm:grid-cols-3 gap-4 max-w-3xl mx-auto">
          <div class="glass-panel p-4 rounded-xl border border-gray-800 text-center hover:border-brand-emerald/50 transition">
            <i class="fa-solid fa-calendar-days text-brand-emerald text-2xl mb-2"></i>
            <div class="text-xs text-gray-400 font-semibold uppercase">Tarikh Pertandingan</div>
            <div class="font-bold text-white text-base">10 OKTOBER 2026</div>
            <div class="text-[11px] text-brand-emerald font-medium">(Sabtu)</div>
          </div>
          <div class="glass-panel p-4 rounded-xl border border-gray-800 text-center hover:border-brand-emerald/50 transition">
            <i class="fa-solid fa-location-dot text-brand-gold text-2xl mb-2"></i>
            <div class="text-xs text-gray-400 font-semibold uppercase">Lokasi Kejohanan</div>
            <div class="font-bold text-white text-base">Masjid Sultan Yussuf Izzuddin Shah</div>
            <div class="text-[11px] text-gray-400 font-medium">Seri Iskandar, Perak</div>
          </div>
          <div class="glass-panel p-4 rounded-xl border border-gray-800 text-center hover:border-brand-emerald/50 transition">
            <i class="fa-solid fa-users text-brand-cyan text-2xl mb-2"></i>
            <div class="text-xs text-gray-400 font-semibold uppercase">Status Kehadiran</div>
            <div class="font-bold text-white text-base">Wajib Fizikal</div>
            <div class="text-[11px] text-brand-gold font-medium">Tapak Pertandingan</div>
          </div>
        </div>

        <!-- Countdown Timer -->
        <div class="glass-panel p-6 rounded-2xl max-w-2xl mx-auto border border-brand-emerald/30">
          <div class="text-xs uppercase font-heading tracking-widest text-gray-400 mb-3 flex items-center justify-center gap-2">
            <span class="w-2 h-2 rounded-full bg-red-500 animate-ping"></span>
            Masa Berbaki Sebelum Pendaftaran Ditutup
          </div>
          <div class="grid grid-cols-4 gap-2 sm:gap-4 text-center font-heading">
            <div class="bg-brand-dark/80 p-3 rounded-xl border border-gray-800">
              <span id="cd-days" class="text-2xl sm:text-4xl font-black text-brand-emerald">00</span>
              <span class="block text-[10px] sm:text-xs text-gray-400 uppercase mt-1">Hari</span>
            </div>
            <div class="bg-brand-dark/80 p-3 rounded-xl border border-gray-800">
              <span id="cd-hours" class="text-2xl sm:text-4xl font-black text-brand-emerald">00</span>
              <span class="block text-[10px] sm:text-xs text-gray-400 uppercase mt-1">Jam</span>
            </div>
            <div class="bg-brand-dark/80 p-3 rounded-xl border border-gray-800">
              <span id="cd-mins" class="text-2xl sm:text-4xl font-black text-brand-emerald">00</span>
              <span class="block text-[10px] sm:text-xs text-gray-400 uppercase mt-1">Minit</span>
            </div>
            <div class="bg-brand-dark/80 p-3 rounded-xl border border-gray-800">
              <span id="cd-secs" class="text-2xl sm:text-4xl font-black text-brand-gold">00</span>
              <span class="block text-[10px] sm:text-xs text-gray-400 uppercase mt-1">Saat</span>
            </div>
          </div>
        </div>

        <!-- CTA Buttons -->
        <div class="flex flex-col sm:flex-row items-center justify-center gap-4 pt-4">
          <a href="#pendaftaran" class="w-full sm:w-auto px-8 py-4 rounded-xl bg-gradient-to-r from-brand-emerald via-teal-400 to-brand-gold text-black font-heading font-black text-lg shadow-xl glow-emerald hover:scale-105 active:scale-95 transition-all flex items-center justify-center gap-3">
            <i class="fa-solid fa-gamepad text-xl"></i>
            DAFTAR SEKARANG
          </a>
          <a href="#format" class="w-full sm:w-auto px-8 py-4 rounded-xl glass-panel border border-gray-700 hover:border-brand-emerald text-white font-heading font-bold text-base hover:bg-brand-emerald/10 transition flex items-center justify-center gap-2">
            <i class="fa-solid fa-circle-info"></i>
            FORMAT PERTANDINGAN
          </a>
        </div>

      </div>
    </section>

    <!-- TENTANG & KATEGORI SECTION -->
    <section id="kategori" class="py-16 px-4 bg-brand-dark/90 border-t border-gray-800/80">
      <div class="max-w-7xl mx-auto space-y-12">
        
        <!-- Section Header -->
        <div class="text-center space-y-3 max-w-3xl mx-auto">
          <span class="text-brand-emerald text-xs font-bold uppercase tracking-widest bg-brand-emerald/10 px-3 py-1 rounded-full border border-brand-emerald/20">
            Pertandingan Utama
          </span>
          <h2 class="font-heading text-3xl sm:text-4xl font-extrabold text-white">
            KATEGORI & YURAN PENYERTAAN
          </h2>
          <p class="text-gray-400 text-sm sm:text-base">
            Pilih acara eSports kegemaran anda. Tempat adalah TERHAD untuk menjamin kualiti dan kelancaran kejohanan.
          </p>
        </div>

        <!-- Category Cards Grid -->
        <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
          
          <!-- eFootball Card -->
          <div class="glass-panel rounded-2xl border border-gray-800 p-6 sm:p-8 relative overflow-hidden group hover:border-brand-emerald transition-all duration-300">
            <div class="absolute top-0 right-0 bg-brand-emerald text-black font-heading font-black text-xs px-4 py-1.5 rounded-bl-xl uppercase tracking-wider">
              32 Peserta Sahaja
            </div>
            
            <div class="flex items-center gap-4 mb-6">
              <div class="w-16 h-16 rounded-2xl bg-gradient-to-br from-green-500 to-emerald-800 flex items-center justify-center text-3xl text-white shadow-lg">
                <i class="fa-solid fa-futbol"></i>
              </div>
              <div>
                <h3 class="font-heading text-2xl font-black text-white">eFOOTBALL</h3>
                <p class="text-xs text-brand-emerald font-semibold uppercase tracking-wider">Acara Solo (1 vs 1)</p>
              </div>
            </div>

            <div class="space-y-4 text-sm text-gray-300 border-t border-b border-gray-800 py-4 mb-6">
              <div class="flex justify-between items-center">
                <span class="text-gray-400">Yuran Penyertaan</span>
                <span class="font-heading font-extrabold text-2xl text-brand-gold">RM 5 <span class="text-xs font-normal text-gray-400">/ pemain</span></span>
              </div>
              <div class="flex justify-between items-center">
                <span class="text-gray-400">Format Kejohanan</span>
                <span class="font-semibold text-white">Group Stage + Knockout</span>
              </div>
              <div class="flex justify-between items-center">
                <span class="text-gray-400">Masa Perlawanan</span>
                <span class="font-semibold text-white">6 Minit (Single Match)</span>
              </div>
              <div class="flex justify-between items-center">
                <span class="text-gray-400">Kehadiran</span>
                <span class="font-semibold text-brand-emerald">Wajib di Tapak Kejohanan</span>
              </div>
            </div>

            <a href="#pendaftaran" onclick="selectCategoryInForm('eFootball')" class="block w-full py-3 text-center rounded-xl font-heading font-bold bg-brand-emerald/20 hover:bg-brand-emerald text-brand-emerald hover:text-black border border-brand-emerald/40 transition">
              DAFTAR eFOOTBALL (RM5)
            </a>
          </div>

          <!-- MLBB Card -->
          <div class="glass-panel rounded-2xl border border-gray-800 p-6 sm:p-8 relative overflow-hidden group hover:border-brand-gold transition-all duration-300">
            <div class="absolute top-0 right-0 bg-brand-gold text-black font-heading font-black text-xs px-4 py-1.5 rounded-bl-xl uppercase tracking-wider">
              Acara Berpasukan
            </div>
            
            <div class="flex items-center gap-4 mb-6">
              <div class="w-16 h-16 rounded-2xl bg-gradient-to-br from-amber-500 to-yellow-700 flex items-center justify-center text-3xl text-white shadow-lg">
                <i class="fa-solid fa-shield-halved"></i>
              </div>
              <div>
                <h3 class="font-heading text-2xl font-black text-white">MOBILE LEGENDS</h3>
                <p class="text-xs text-brand-gold font-semibold uppercase tracking-wider">Bang Bang (5 vs 5)</p>
              </div>
            </div>

            <div class="space-y-4 text-sm text-gray-300 border-t border-b border-gray-800 py-4 mb-6">
              <div class="flex justify-between items-center">
                <span class="text-gray-400">Yuran Penyertaan</span>
                <span class="font-heading font-extrabold text-2xl text-brand-gold">RM 10 <span class="text-xs font-normal text-gray-400">/ pasukan</span></span>
              </div>
              <div class="flex justify-between items-center">
                <span class="text-gray-400">Keahlian Pasukan</span>
                <span class="font-semibold text-white">5 Pemain Utama</span>
              </div>
              <div class="flex justify-between items-center">
                <span class="text-gray-400">Check-In Pagi</span>
                <span class="font-semibold text-brand-gold">7:30 Pagi – 8:15 Pagi</span>
              </div>
              <div class="flex justify-between items-center">
                <span class="text-gray-400">Format Kejohanan</span>
                <span class="font-semibold text-white">Kumpulan + System Kalah Mati</span>
              </div>
            </div>

            <a href="#pendaftaran" onclick="selectCategoryInForm('Mobile Legends')" class="block w-full py-3 text-center rounded-xl font-heading font-bold bg-brand-gold/20 hover:bg-brand-gold text-brand-gold hover:text-black border border-brand-gold/40 transition">
              DAFTAR MOBILE LEGENDS (RM10)
            </a>
          </div>

        </div>

      </div>
    </section>

    <!-- FORMAT & PERATURAN SECTION -->
    <section id="format" class="py-16 px-4 bg-brand-dark relative">
      <div class="max-w-7xl mx-auto space-y-10">
        
        <div class="text-center space-y-3 max-w-3xl mx-auto">
          <span class="text-brand-gold text-xs font-bold uppercase tracking-widest bg-brand-gold/10 px-3 py-1 rounded-full border border-brand-gold/20">
            Syarat & Format Syarat
          </span>
          <h2 class="font-heading text-3xl sm:text-4xl font-extrabold text-white">
            FORMAT PERTANDINGAN & PERATURAN
          </h2>
          <p class="text-gray-400 text-sm">
            Sila baca dan fahami peraturan rasmi sebelum menghantar pendaftaran anda.
          </p>
        </div>

        <!-- Format Tabs Nav -->
        <div class="flex justify-center border-b border-gray-800">
          <div class="flex gap-4">
            <button id="tab-ef-btn" onclick="switchFormatTab('efootball')" class="py-3 px-6 font-heading font-bold text-sm border-b-2 border-brand-emerald text-brand-emerald transition flex items-center gap-2">
              <i class="fa-solid fa-futbol"></i> eFootball Rules
            </button>
            <button id="tab-ml-btn" onclick="switchFormatTab('mlbb')" class="py-3 px-6 font-heading font-bold text-sm border-b-2 border-transparent text-gray-400 hover:text-white transition flex items-center gap-2">
              <i class="fa-solid fa-shield-halved"></i> MLBB Rules
            </button>
          </div>
        </div>

        <!-- Tab Content: eFootball -->
        <div id="tab-efootball" class="grid grid-cols-1 md:grid-cols-2 gap-8">
          <div class="glass-panel p-6 rounded-2xl border border-gray-800 space-y-4">
            <h3 class="font-heading text-lg font-bold text-brand-emerald flex items-center gap-2">
              <i class="fa-solid fa-sitemap"></i> Format Kejohanan eFootball
            </h3>
            <ul class="space-y-3 text-sm text-gray-300">
              <li class="flex items-start gap-2">
                <i class="fa-solid fa-check-circle text-brand-emerald mt-1"></i>
                <span><strong>Jumlah Peserta:</strong> Terhad kepada 32 pemain sahaja.</span>
              </li>
              <li class="flex items-start gap-2">
                <i class="fa-solid fa-check-circle text-brand-emerald mt-1"></i>
                <span><strong>Peringkat Kumpulan:</strong> 4 pemain setiap kumpulan (Round Robin secara random tanpa jadual tetap).</span>
              </li>
              <li class="flex items-start gap-2">
                <i class="fa-solid fa-check-circle text-brand-emerald mt-1"></i>
                <span><strong>Kelayakan:</strong> Top 2 setiap kumpulan layak ke peringkat kalah mati.</span>
              </li>
              <li class="flex items-start gap-2">
                <i class="fa-solid fa-check-circle text-brand-emerald mt-1"></i>
                <span><strong>Tetapan Perlawanan:</strong> Single Match | Masa: 6 Minit | Extra Time: OFF | Penalty: OFF.</span>
              </li>
              <li class="flex items-start gap-2">
                <i class="fa-solid fa-check-circle text-brand-emerald mt-1"></i>
                <span><strong>Sistem Mata:</strong> Menang = 3 Mata | Seri = 1 Mata | Kalah = 0 Mata.</span>
              </li>
            </ul>
          </div>

          <div class="glass-panel p-6 rounded-2xl border border-gray-800 space-y-4">
            <h3 class="font-heading text-lg font-bold text-brand-gold flex items-center gap-2">
              <i class="fa-solid fa-triangle-exclamation"></i> Peraturan Khas & Speedtest
            </h3>
            <ul class="space-y-3 text-sm text-gray-300">
              <li class="flex items-start gap-2">
                <i class="fa-solid fa-ban text-red-400 mt-1"></i>
                <span><strong>No Celebration & No Backpass:</strong> Dilarang sama sekali membuat keraian gol berlebihan & hantaran ke belakang secara sengaja untuk buang masa.</span>
              </li>
              <li class="flex items-start gap-2">
                <i class="fa-solid fa-wifi text-brand-gold mt-1"></i>
                <span><strong>Ujian Speedtest Ookla:</strong> Peserta Wajib membuat ujian Speedtest bersama pihak lawan menggunakan aplikasi Ookla sebelum perlawanan.</span>
              </li>
              <li class="flex items-start gap-2">
                <i class="fa-solid fa-camera text-brand-gold mt-1"></i>
                <span><strong>Bukti Keputusan:</strong> Screenshot keputusan penuh wajib dihantar ke WhatsApp Group Kumpulan & Tag Admin bertugas.</span>
              </li>
              <li class="flex items-start gap-2">
                <i class="fa-solid fa-headset text-brand-gold mt-1"></i>
                <span><strong>Isu Sambungan:</strong> Sebarang masalah rangkaian hendaklah dilaporkan kepada admin dengan serta-merta.</span>
              </li>
            </ul>
          </div>
        </div>

        <!-- Tab Content: MLBB (Hidden by default) -->
        <div id="tab-mlbb" class="hidden grid grid-cols-1 md:grid-cols-2 gap-8">
          <div class="glass-panel p-6 rounded-2xl border border-gray-800 space-y-4">
            <h3 class="font-heading text-lg font-bold text-brand-gold flex items-center gap-2">
              <i class="fa-solid fa-clock"></i> Kehadiran & Semakan (Check-in)
            </h3>
            <div class="p-4 rounded-xl bg-brand-gold/10 border border-brand-gold/30 text-sm space-y-2">
              <div class="font-bold text-brand-gold uppercase text-xs">Masa Check-in Rasmi</div>
              <div class="text-xl font-heading font-black text-white">07:30 AM – 08:15 AM</div>
              <p class="text-xs text-gray-300">
                Semua pasukan wajib melaporkan kehadiran di meja urusetia sebelum jam 8:15 pagi. Kelewatan boleh mengakibatkan pembatalan penyertaan (Disqualified - DQ).
              </p>
            </div>
            <ul class="space-y-3 text-sm text-gray-300">
              <li class="flex items-start gap-2">
                <i class="fa-solid fa-check-circle text-brand-gold mt-1"></i>
                <span><strong>Format Pasukan:</strong> 5 Pemain Utama (Semua wajib berada di tapak pertandingan).</span>
              </li>
              <li class="flex items-start gap-2">
                <i class="fa-solid fa-check-circle text-brand-gold mt-1"></i>
                <span><strong>Peringkat Awal & Kalah Mati:</strong> Top 2 setiap kumpulan mara ke sistem kalah mati (Knockout stage).</span>
              </li>
            </ul>
          </div>

          <div class="glass-panel p-6 rounded-2xl border border-gray-800 space-y-4">
            <h3 class="font-heading text-lg font-bold text-brand-cyan flex items-center gap-2">
              <i class="fa-solid fa-shuffle"></i> Peraturan Lobby & Shuffle Pasukan
            </h3>
            <ul class="space-y-3 text-sm text-gray-300">
              <li class="flex items-start gap-2">
                <i class="fa-solid fa-random text-brand-cyan mt-1"></i>
                <span><strong>Proses Shuffle:</strong> Selepas semakan check-in selesai, cabutan/shuffle kumpulan akan dibuat secara automatik dan dipaparkan di skrin utama & link rasmi.</span>
              </li>
              <li class="flex items-start gap-2">
                <i class="fa-solid fa-gamepad text-brand-cyan mt-1"></i>
                <span><strong>Lobby Perlawanan:</strong> Kapten pasukan bertanggungjawab untuk Add Kapten lawan & create lobby (Classic / Draft Pick) mengikut arahan admin.</span>
              </li>
              <li class="flex items-start gap-2">
                <i class="fa-solid fa-plug-circle-exclamation text-brand-cyan mt-1"></i>
                <span><strong>Disconnection:</strong> Jika berlaku Connection Lost, pemain mesti masuk semula secepat mungkin. Tiada Recreate Lobby kecuali dengan kebenaran Admin.</span>
              </li>
              <li class="flex items-start gap-2">
                <i class="fa-solid fa-battery-full text-brand-cyan mt-1"></i>
                <span><strong>Kelengkapan Sendiri:</strong> Peserta bertanggungjawab menyediakan Powerbank & internet data persendirian.</span>
              </li>
            </ul>
          </div>
        </div>

      </div>
    </section>

    <!-- CARA PENDAFTARAN -->
    <section id="cara-daftar" class="py-16 px-4 bg-brand-dark/90 border-t border-gray-800">
      <div class="max-w-6xl mx-auto space-y-12">
        
        <div class="text-center space-y-3">
          <h2 class="font-heading text-3xl sm:text-4xl font-extrabold text-white">
            4 LANGKAH MUDAH PENDAFTARAN
          </h2>
          <p class="text-gray-400 text-sm">Ikuti langkah di bawah untuk mendaftar slot kejohanan anda.</p>
        </div>

        <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-6">
          <div class="glass-panel p-6 rounded-2xl border border-gray-800 text-center space-y-3 relative">
            <div class="w-12 h-12 rounded-full bg-brand-emerald text-black font-heading font-black text-xl flex items-center justify-center mx-auto shadow-lg">1</div>
            <h3 class="font-heading font-bold text-white text-base">Pilih Kategori</h3>
            <p class="text-xs text-gray-400">Pilih eFootball (Solo) atau Mobile Legends (Pasukan) dalam borang pendaftaran.</p>
          </div>

          <div class="glass-panel p-6 rounded-2xl border border-gray-800 text-center space-y-3 relative">
            <div class="w-12 h-12 rounded-full bg-brand-emerald text-black font-heading font-black text-xl flex items-center justify-center mx-auto shadow-lg">2</div>
            <h3 class="font-heading font-bold text-white text-base">Isi Maklumat</h3>
            <p class="text-xs text-gray-400">Masukkan butiran diri atau maklumat lengkap 5 pemain pasukan anda.</p>
          </div>

          <div class="glass-panel p-6 rounded-2xl border border-gray-800 text-center space-y-3 relative">
            <div class="w-12 h-12 rounded-full bg-brand-emerald text-black font-heading font-black text-xl flex items-center justify-center mx-auto shadow-lg">3</div>
            <h3 class="font-heading font-bold text-white text-base">Muat Naik Bayaran</h3>
            <p class="text-xs text-gray-400">Buat pembayaran ke akaun rasmi dan muat naik bukti resit transaksi.</p>
          </div>

          <div class="glass-panel p-6 rounded-2xl border border-gray-800 text-center space-y-3 relative">
            <div class="w-12 h-12 rounded-full bg-brand-gold text-black font-heading font-black text-xl flex items-center justify-center mx-auto shadow-lg">4</div>
            <h3 class="font-heading font-bold text-white text-base">Terima Slip & WA</h3>
            <p class="text-xs text-gray-400">Dapatkan No. Pendaftaran automatik dan sahkan penyertaan melalui WhatsApp Admin.</p>
          </div>
        </div>

      </div>
    </section>

    <!-- BORANG PENDAFTARAN SECTION -->
    <section id="pendaftaran" class="py-16 px-4 bg-grid-pattern relative">
      <div class="max-w-4xl mx-auto">
        
        <div class="glass-panel rounded-3xl border border-brand-emerald/40 p-6 sm:p-10 shadow-2xl relative overflow-hidden">
          
          <div class="text-center space-y-2 mb-8">
            <span class="px-3 py-1 bg-brand-emerald/10 text-brand-emerald border border-brand-emerald/30 text-xs font-bold rounded-full uppercase">
              Borang Rasmi Online
            </span>
            <h2 class="font-heading text-2xl sm:text-4xl font-black text-white">
              BORANG PENDAFTARAN kejohanan
            </h2>
            <p class="text-xs sm:text-sm text-gray-400">
              Sila pastikan semua maklumat tepat dan bukti pembayaran disertakan.
            </p>
          </div>

          <!-- Registration Form -->
          <form id="regForm" onsubmit="handleRegistrationSubmit(event)" class="space-y-8">
            
            <!-- Category Selector Buttons -->
            <div class="space-y-3">
              <label class="block text-xs font-heading uppercase text-gray-300 font-bold tracking-wider">
                1. Pilih Kategori Pertandingan <span class="text-red-500">*</span>
              </label>
              <div class="grid grid-cols-2 gap-4">
                <button type="button" id="btn-cat-ef" onclick="selectCategoryInForm('eFootball')" class="py-4 px-4 rounded-xl border-2 border-brand-emerald bg-brand-emerald/10 text-white font-heading font-bold text-sm sm:text-base flex flex-col items-center gap-1 transition shadow-lg">
                  <i class="fa-solid fa-futbol text-2xl text-brand-emerald"></i>
                  <span>eFOOTBALL</span>
                  <span class="text-[11px] font-normal text-brand-emerald">RM 5.00 / pemain</span>
                </button>

                <button type="button" id="btn-cat-ml" onclick="selectCategoryInForm('Mobile Legends')" class="py-4 px-4 rounded-xl border-2 border-gray-800 bg-brand-dark/50 text-gray-400 font-heading font-bold text-sm sm:text-base flex flex-col items-center gap-1 transition hover:border-brand-gold">
                  <i class="fa-solid fa-shield-halved text-2xl text-brand-gold"></i>
                  <span>MOBILE LEGENDS</span>
                  <span class="text-[11px] font-normal text-brand-gold">RM 10.00 / Pasukan</span>
                </button>
              </div>
              <input type="hidden" id="inputCategory" name="category" value="eFootball" required>
            </div>

            <!-- Dynamic Form Fields: eFootball -->
            <div id="fields-eFootball" class="space-y-5">
              <div class="border-b border-gray-800 pb-2">
                <h3 class="font-heading text-sm font-bold text-brand-emerald uppercase tracking-wider flex items-center gap-2">
                  <i class="fa-solid fa-user"></i> Maklumat Pemain eFootball
                </h3>
              </div>

              <div class="grid grid-cols-1 sm:grid-cols-2 gap-4">
                <div>
                  <label class="block text-xs font-semibold text-gray-300 mb-1">Nama Penuh Peserta <span class="text-red-500">*</span></label>
                  <input type="text" id="ef_nama" class="w-full bg-brand-dark/90 border border-gray-800 rounded-xl px-4 py-3 text-sm text-white focus:border-brand-emerald focus:outline-none transition" placeholder="Contoh: Ahmad bin Razak" required>
                </div>
                <div>
                  <label class="block text-xs font-semibold text-gray-300 mb-1">No. Telefon WhatsApp <span class="text-red-500">*</span></label>
                  <input type="tel" id="ef_phone" class="w-full bg-brand-dark/90 border border-gray-800 rounded-xl px-4 py-3 text-sm text-white focus:border-brand-emerald focus:outline-none transition" placeholder="Contoh: 0123456789" required>
                </div>
              </div>

              <div class="grid grid-cols-1 sm:grid-cols-2 gap-4">
                <div>
                  <label class="block text-xs font-semibold text-gray-300 mb-1">E-mel <span class="text-red-500">*</span></label>
                  <input type="email" id="ef_email" class="w-full bg-brand-dark/90 border border-gray-800 rounded-xl px-4 py-3 text-sm text-white focus:border-brand-emerald focus:outline-none transition" placeholder="ahmad@gmail.com" required>
                </div>
                <div>
                  <label class="block text-xs font-semibold text-gray-300 mb-1">Nama Dalam Game (IGN) <span class="text-red-500">*</span></label>
                  <input type="text" id="ef_ign" class="w-full bg-brand-dark/90 border border-gray-800 rounded-xl px-4 py-3 text-sm text-white focus:border-brand-emerald focus:outline-none transition" placeholder="Contoh: FC_Ahmad99" required>
                </div>
              </div>

              <div>
                <label class="block text-xs font-semibold text-gray-300 mb-1">User ID / Game ID eFootball <span class="text-red-500">*</span></label>
                <input type="text" id="ef_gameid" class="w-full bg-brand-dark/90 border border-gray-800 rounded-xl px-4 py-3 text-sm text-white focus:border-brand-emerald focus:outline-none transition" placeholder="Contoh: 849-204-102" required>
              </div>
            </div>

            <!-- Dynamic Form Fields: Mobile Legends (Hidden initially) -->
            <div id="fields-MLBB" class="space-y-6 hidden">
              <div class="border-b border-gray-800 pb-2">
                <h3 class="font-heading text-sm font-bold text-brand-gold uppercase tracking-wider flex items-center gap-2">
                  <i class="fa-solid fa-users"></i> Maklumat Pasukan & Kapten MLBB
                </h3>
              </div>

              <div class="grid grid-cols-1 sm:grid-cols-2 gap-4">
                <div>
                  <label class="block text-xs font-semibold text-gray-300 mb-1">Nama Pasukan (Team Name) <span class="text-red-500">*</span></label>
                  <input type="text" id="ml_team" class="w-full bg-brand-dark/90 border border-gray-800 rounded-xl px-4 py-3 text-sm text-white focus:border-brand-gold focus:outline-none transition" placeholder="Contoh: Perak Esports Squad">
                </div>
                <div>
                  <label class="block text-xs font-semibold text-gray-300 mb-1">Nama Penuh Kapten <span class="text-red-500">*</span></label>
                  <input type="text" id="ml_kapten" class="w-full bg-brand-dark/90 border border-gray-800 rounded-xl px-4 py-3 text-sm text-white focus:border-brand-gold focus:outline-none transition" placeholder="Nama Kapten Pasukan">
                </div>
              </div>

              <div class="grid grid-cols-1 sm:grid-cols-2 gap-4">
                <div>
                  <label class="block text-xs font-semibold text-gray-300 mb-1">No. Telefon Kapten (WhatsApp) <span class="text-red-500">*</span></label>
                  <input type="tel" id="ml_phone" class="w-full bg-brand-dark/90 border border-gray-800 rounded-xl px-4 py-3 text-sm text-white focus:border-brand-gold focus:outline-none transition" placeholder="01X-XXXXXXX">
                </div>
                <div>
                  <label class="block text-xs font-semibold text-gray-300 mb-1">E-mel Kapten <span class="text-red-500">*</span></label>
                  <input type="email" id="ml_email" class="w-full bg-brand-dark/90 border border-gray-800 rounded-xl px-4 py-3 text-sm text-white focus:border-brand-gold focus:outline-none transition" placeholder="kapten@gmail.com">
                </div>
              </div>

              <!-- 5 Players Inputs Grid -->
              <div class="space-y-4 pt-2">
                <label class="block text-xs font-heading uppercase text-brand-gold font-bold tracking-wider">
                  Senarai 5 Pemain Wajib (Nama + Game ID & Server)
                </label>

                <!-- Player 1 -->
                <div class="p-3 rounded-xl bg-brand-dark/60 border border-gray-800 space-y-2">
                  <div class="text-xs font-bold text-gray-400">Pemain 1 (Kapten)</div>
                  <div class="grid grid-cols-1 sm:grid-cols-2 gap-2">
                    <input type="text" id="ml_p1_nama" placeholder="Nama Penuh Player 1" class="bg-brand-dark border border-gray-700 rounded-lg p-2 text-xs text-white">
                    <input type="text" id="ml_p1_id" placeholder="ID & Server (Contoh: 12345678 (1234))" class="bg-brand-dark border border-gray-700 rounded-lg p-2 text-xs text-white">
                  </div>
                </div>

                <!-- Player 2 -->
                <div class="p-3 rounded-xl bg-brand-dark/60 border border-gray-800 space-y-2">
                  <div class="text-xs font-bold text-gray-400">Pemain 2</div>
                  <div class="grid grid-cols-1 sm:grid-cols-2 gap-2">
                    <input type="text" id="ml_p2_nama" placeholder="Nama Penuh Player 2" class="bg-brand-dark border border-gray-700 rounded-lg p-2 text-xs text-white">
                    <input type="text" id="ml_p2_id" placeholder="ID & Server Player 2" class="bg-brand-dark border border-gray-700 rounded-lg p-2 text-xs text-white">
                  </div>
                </div>

                <!-- Player 3 -->
                <div class="p-3 rounded-xl bg-brand-dark/60 border border-gray-800 space-y-2">
                  <div class="text-xs font-bold text-gray-400">Pemain 3</div>
                  <div class="grid grid-cols-1 sm:grid-cols-2 gap-2">
                    <input type="text" id="ml_p3_nama" placeholder="Nama Penuh Player 3" class="bg-brand-dark border border-gray-700 rounded-lg p-2 text-xs text-white">
                    <input type="text" id="ml_p3_id" placeholder="ID & Server Player 3" class="bg-brand-dark border border-gray-700 rounded-lg p-2 text-xs text-white">
                  </div>
                </div>

                <!-- Player 4 -->
                <div class="p-3 rounded-xl bg-brand-dark/60 border border-gray-800 space-y-2">
                  <div class="text-xs font-bold text-gray-400">Pemain 4</div>
                  <div class="grid grid-cols-1 sm:grid-cols-2 gap-2">
                    <input type="text" id="ml_p4_nama" placeholder="Nama Penuh Player 4" class="bg-brand-dark border border-gray-700 rounded-lg p-2 text-xs text-white">
                    <input type="text" id="ml_p4_id" placeholder="ID & Server Player 4" class="bg-brand-dark border border-gray-700 rounded-lg p-2 text-xs text-white">
                  </div>
                </div>

                <!-- Player 5 -->
                <div class="p-3 rounded-xl bg-brand-dark/60 border border-gray-800 space-y-2">
                  <div class="text-xs font-bold text-gray-400">Pemain 5</div>
                  <div class="grid grid-cols-1 sm:grid-cols-2 gap-2">
                    <input type="text" id="ml_p5_nama" placeholder="Nama Penuh Player 5" class="bg-brand-dark border border-gray-700 rounded-lg p-2 text-xs text-white">
                    <input type="text" id="ml_p5_id" placeholder="ID & Server Player 5" class="bg-brand-dark border border-gray-700 rounded-lg p-2 text-xs text-white">
                  </div>
                </div>

              </div>
            </div>

            <!-- PAYMENT & PROOF SECTION -->
            <div class="space-y-4 pt-4 border-t border-gray-800">
              <div class="flex items-center justify-between bg-brand-dark/80 p-4 rounded-xl border border-gray-800">
                <div>
                  <div class="text-xs text-gray-400 uppercase font-semibold">Jumlah Perlu Dibayar</div>
                  <div id="feeDisplay" class="text-2xl font-heading font-black text-brand-gold">RM 5.00</div>
                </div>
                <div class="text-right">
                  <span class="text-[10px] text-gray-400 block">Akaun Bank Penganjur:</span>
                  <span class="text-xs font-bold text-white block">AFFIN BANK</span>
                  <span class="text-xs font-mono text-brand-emerald">105550000264</span>
                  <span class="text-[10px] text-gray-400 block">Majlis Belia Daerah Perak Tengah</span>
                </div>
              </div>

              <!-- Upload File -->
              <div>
                <label class="block text-xs font-semibold text-gray-300 mb-2">
                  Muat Naik Bukti Pembayaran (Resit / QR Transfer) <span class="text-red-500">*</span>
                </label>
                <div class="flex items-center justify-center w-full">
                  <label for="proofUpload" class="flex flex-col items-center justify-center w-full h-32 border-2 border-dashed border-gray-700 hover:border-brand-emerald rounded-2xl cursor-pointer bg-brand-dark/50 hover:bg-brand-dark transition">
                    <div class="flex flex-col items-center justify-center pt-5 pb-6 text-center px-4">
                      <i class="fa-solid fa-cloud-arrow-up text-2xl text-brand-emerald mb-2"></i>
                      <p id="uploadText" class="text-xs text-gray-300">
                        <span class="font-bold text-brand-emerald">Klik untuk muat naik</span> resit bayaran
                      </p>
                      <p class="text-[10px] text-gray-500 mt-1">PNG, JPG, JPEG atau PDF (Maksimum 5MB)</p>
                    </div>
                    <input id="proofUpload" type="file" accept="image/*,.pdf" onchange="handleFilePreview(this)" class="hidden" required>
                  </label>
                </div>
                <div id="filePreviewContainer" class="hidden mt-2 flex items-center justify-between p-2 rounded-lg bg-brand-emerald/10 border border-brand-emerald/30 text-xs text-brand-emerald">
                  <span id="fileName" class="truncate font-semibold">filename.png</span>
                  <button type="button" onclick="resetFileUpload()" class="text-red-400 hover:text-red-300 ml-2 font-bold">X</button>
                </div>
              </div>

              <!-- Consent Checkbox -->
              <div class="flex items-start gap-3 pt-2">
                <input type="checkbox" id="consent" class="mt-1 w-4 h-4 rounded accent-brand-emerald" required>
                <label for="consent" class="text-xs text-gray-300 leading-relaxed">
                  Saya mengesahkan bahawa maklumat yang diberikan adalah tepat dan saya bersetuju mematuhi semua <strong class="text-white">Peraturan & Syarat Kejohanan Esport Tour Smart Ummah Perak Tengah 2026</strong>.
                </label>
              </div>
            </div>

            <!-- Submit Button -->
            <button type="submit" id="btnSubmit" class="w-full py-4 rounded-xl bg-gradient-to-r from-brand-emerald via-teal-400 to-brand-gold text-black font-heading font-black text-lg shadow-xl hover:brightness-110 active:scale-95 transition-all flex items-center justify-center gap-2">
              <i class="fa-solid fa-paper-plane"></i>
              HANTAR PENDAFTARAN
            </button>

          </form>

        </div>

      </div>
    </section>

    <!-- FAQ SECTION -->
    <section id="faq" class="py-16 px-4 bg-brand-dark border-t border-gray-800">
      <div class="max-w-4xl mx-auto space-y-8">
        
        <div class="text-center space-y-2">
          <span class="text-brand-emerald text-xs font-bold uppercase tracking-widest bg-brand-emerald/10 px-3 py-1 rounded-full">Bantuan & FAQ</span>
          <h2 class="font-heading text-3xl font-extrabold text-white">SOALAN LAZIM (FAQ)</h2>
        </div>

        <div class="space-y-4">
          <details class="glass-panel rounded-xl p-4 border border-gray-800 group cursor-pointer">
            <summary class="font-heading font-bold text-white text-sm sm:text-base flex justify-between items-center">
              <span>Adakah pertandingan ini dijalankan secara dalam talian (Online) atau Fizikal?</span>
              <i class="fa-solid fa-chevron-down text-brand-emerald transition-transform group-open:rotate-180"></i>
            </summary>
            <p class="mt-3 text-xs sm:text-sm text-gray-400 leading-relaxed">
              Semua peserta WAJIB hadir secara fizikal di lokasi kejohanan (Masjid Sultan Yussuf Izzuddin Shah, Seri Iskandar) pada 10 Oktober 2026.
            </p>
          </details>

          <details class="glass-panel rounded-xl p-4 border border-gray-800 group cursor-pointer">
            <summary class="font-heading font-bold text-white text-sm sm:text-base flex justify-between items-center">
              <span>Bagaimanakah proses pengesahan bayaran dilakukan?</span>
              <i class="fa-solid fa-chevron-down text-brand-emerald transition-transform group-open:rotate-180"></i>
            </summary>
            <p class="mt-3 text-xs sm:text-sm text-gray-400 leading-relaxed">
              Selepas mendaftar, urusetia akan menyemak bukti resit pembayaran anda. Anda boleh menekan butang WhatsApp Admin selepas pendaftaran untuk mempercepatkan proses pengesahan (VERIFIED).
            </p>
          </details>

          <details class="glass-panel rounded-xl p-4 border border-gray-800 group cursor-pointer">
            <summary class="font-heading font-bold text-white text-sm sm:text-base flex justify-between items-center">
              <span>Bolehkah saya mendaftar untuk kedua-dua kategori eFootball dan MLBB?</span>
              <i class="fa-solid fa-chevron-down text-brand-emerald transition-transform group-open:rotate-180"></i>
            </summary>
            <p class="mt-3 text-xs sm:text-sm text-gray-400 leading-relaxed">
              Boleh, dengan syarat jadual perlawanan tidak bertembung dan anda mendaftar borang berasingan bagi setiap kategori.
            </p>
          </details>
        </div>

      </div>
    </section>

    <!-- HUBUNGI ADMIN SECTION -->
    <section id="hubungi" class="py-16 px-4 bg-brand-dark/95 border-t border-gray-800 text-center">
      <div class="max-w-3xl mx-auto space-y-6">
        <h2 class="font-heading text-3xl font-extrabold text-white">MEMPUNYAI SEBARANG SOALAN?</h2>
        <p class="text-sm text-gray-400">
          Urusetia kejohanan Majlis Belia Daerah Perak Tengah sedia membantu anda.
        </p>
        <div class="flex flex-wrap items-center justify-center gap-4">
          <a href="https://wa.me/60123456789?text=Salam%20Admin%20Esport%20Smart%20Ummah" target="_blank" class="px-6 py-3 rounded-xl bg-green-600 hover:bg-green-500 text-white font-bold text-sm flex items-center gap-2 transition shadow-lg">
            <i class="fa-brands fa-whatsapp text-lg"></i> WhatsApp Admin 1 (012-3456789)
          </a>
          <a href="https://wa.me/60198765432?text=Salam%20Admin%20Esport%20Smart%20Ummah" target="_blank" class="px-6 py-3 rounded-xl bg-green-600 hover:bg-green-500 text-white font-bold text-sm flex items-center gap-2 transition shadow-lg">
            <i class="fa-brands fa-whatsapp text-lg"></i> WhatsApp Admin 2 (019-8765432)
          </a>
        </div>
      </div>
    </section>
  </main>

  <!-- FOOTER -->
  <footer class="bg-black/90 border-t border-gray-800/80 py-8 text-center text-xs text-gray-500">
    <div class="max-w-7xl mx-auto px-4 space-y-3">
      <div class="font-heading font-bold text-gray-300">
        ESPORT TOUR SMART UMMAH DAERAH PERAK TENGAH 2026
      </div>
      <p>Anjuran Majlis Belia Negeri Perak & Majlis Belia Daerah Perak Tengah • Sempena Hari Sukan Negara</p>
      <p class="text-[10px] text-gray-600">&copy; 2026 Hak Cipta Terpelihara.</p>
    </div>
  </footer>

  <!-- MODAL: SUCCESS CONFIRMATION SLIP -->
  <div id="successModal" class="fixed inset-0 z-50 hidden bg-black/80 backdrop-blur-md flex items-center justify-center p-4 overflow-y-auto">
    <div class="glass-panel w-full max-w-lg rounded-3xl border border-brand-emerald p-6 sm:p-8 space-y-6 my-8 relative animate-bounce-short">
      
      <div class="text-center space-y-2">
        <div class="w-16 h-16 bg-brand-emerald/20 text-brand-emerald border border-brand-emerald rounded-full flex items-center justify-center text-3xl mx-auto shadow-lg">
          <i class="fa-solid fa-circle-check"></i>
        </div>
        <h3 class="font-heading text-2xl font-black text-white">TAHNIAH! PENDAFTARAN BERJAYA</h3>
        <p class="text-xs text-gray-300">Pendaftaran anda telah direkodkan dalam sistem rasmi kejohanan.</p>
      </div>

      <!-- Receipt Slip Box -->
      <div class="bg-brand-dark p-5 rounded-2xl border border-gray-800 space-y-3 text-sm">
        <div class="flex justify-between items-center border-b border-gray-800 pb-2">
          <span class="text-gray-400 text-xs">No. Pendaftaran</span>
          <span id="slipRegNo" class="font-mono font-bold text-brand-emerald">EST2026-EF-1029</span>
        </div>
        <div class="flex justify-between items-center border-b border-gray-800 pb-2">
          <span class="text-gray-400 text-xs">Kategori</span>
          <span id="slipCategory" class="font-semibold text-white">eFootball</span>
        </div>
        <div class="flex justify-between items-center border-b border-gray-800 pb-2">
          <span class="text-gray-400 text-xs">Nama / Pasukan</span>
          <span id="slipName" class="font-semibold text-white">Ahmad bin Razak</span>
        </div>
        <div class="flex justify-between items-center border-b border-gray-800 pb-2">
          <span class="text-gray-400 text-xs">Jumlah Bayaran</span>
          <span id="slipFee" class="font-bold text-brand-gold">RM 5.00</span>
        </div>
        <div class="flex justify-between items-center">
          <span class="text-gray-400 text-xs">Status Pembayaran</span>
          <span id="slipStatus" class="px-2 py-0.5 rounded text-xs font-bold bg-amber-500/20 text-amber-400 border border-amber-500/30">
            PENDING VERIFICATION
          </span>
        </div>
      </div>

      <div class="bg-brand-emerald/10 p-3 rounded-xl border border-brand-emerald/30 text-xs text-gray-300 space-y-1">
        <div class="font-bold text-brand-emerald">Arahan Seterusnya:</div>
        <p>Sila klik butang di bawah untuk menghantar No. Pendaftaran anda ke WhatsApp Admin bagi menyertai Group WhatsApp Rasmi Peserta.</p>
      </div>

      <div class="space-y-3">
        <a id="btnWhatsappSlip" href="#" target="_blank" class="w-full py-3.5 rounded-xl bg-green-600 hover:bg-green-500 text-white font-bold text-sm flex items-center justify-center gap-2 transition shadow-lg">
          <i class="fa-brands fa-whatsapp text-lg"></i> Hantar Ke WhatsApp Admin
        </a>
        <button onclick="closeSuccessModal()" class="w-full py-3 rounded-xl glass-panel border border-gray-700 text-gray-300 hover:text-white text-xs font-bold">
          Kembali Ke Halaman Utama
        </button>
      </div>

    </div>
  </div>

  <!-- MODAL: ADMIN LOGIN & DASHBOARD -->
  <div id="adminModal" class="fixed inset-0 z-50 hidden bg-black/90 backdrop-blur-md flex items-center justify-center p-4 overflow-y-auto">
    <div class="glass-panel w-full max-w-5xl rounded-3xl border border-gray-800 p-6 sm:p-8 space-y-6 my-8 max-h-[90vh] overflow-y-auto relative">
      
      <!-- Close Button -->
      <button onclick="toggleAdminModal()" class="absolute top-6 right-6 text-gray-400 hover:text-white text-xl">
        <i class="fa-solid fa-xmark"></i>
      </button>

      <!-- Admin Passcode Screen -->
      <div id="adminAuthScreen" class="text-center py-8 space-y-4 max-w-md mx-auto">
        <div class="w-16 h-16 rounded-full bg-brand-emerald/20 border border-brand-emerald text-brand-emerald flex items-center justify-center text-2xl mx-auto">
          <i class="fa-solid fa-lock"></i>
        </div>
        <h3 class="font-heading text-2xl font-black text-white">LOG MASUK ADMIN</h3>
        <p class="text-xs text-gray-400">Sistem Pengurusan Urusetia Esport Tour Smart Ummah 2026</p>
        <div class="space-y-3">
          <input type="password" id="adminPin" placeholder="Masukkan PIN Admin (Lalai: admin2026)" class="w-full bg-brand-dark border border-gray-700 rounded-xl px-4 py-3 text-sm text-center text-white focus:border-brand-emerald focus:outline-none">
          <button onclick="verifyAdminPin()" class="w-full py-3 bg-brand-emerald hover:bg-brand-emeraldHover text-black font-bold text-sm rounded-xl transition">
            LULUSKAN CAPAIAN
          </button>
        </div>
      </div>

      <!-- Admin Dashboard Content (Hidden until authenticated) -->
      <div id="adminDashboardContent" class="hidden space-y-6">
        
        <div class="flex flex-col sm:flex-row justify-between items-start sm:items-center gap-4 border-b border-gray-800 pb-4">
          <div>
            <h3 class="font-heading text-2xl font-black text-white flex items-center gap-2">
              <i class="fa-solid fa-gauge-high text-brand-emerald"></i> DASHBOARD ADMIN
            </h3>
            <p class="text-xs text-gray-400">Pengurusan Peserta & Pengesahan Yuran Pembayaran</p>
          </div>
          <div class="flex items-center gap-2">
            <button onclick="exportDataCSV()" class="px-3 py-2 bg-brand-dark border border-gray-700 hover:border-brand-emerald rounded-lg text-xs text-gray-300 font-bold flex items-center gap-2">
              <i class="fa-solid fa-file-csv text-brand-emerald"></i> Export CSV
            </button>
            <button onclick="logoutAdmin()" class="px-3 py-2 bg-red-500/20 text-red-400 border border-red-500/30 rounded-lg text-xs font-bold">
              Log Keluar
            </button>
          </div>
        </div>

        <!-- Summary Statistics Cards -->
        <div class="grid grid-cols-1 sm:grid-cols-4 gap-4">
          <div class="bg-brand-dark p-4 rounded-xl border border-gray-800">
            <div class="text-xs text-gray-400">Jumlah Pendaftaran</div>
            <div id="statTotalCount" class="text-2xl font-heading font-black text-white">0</div>
          </div>
          <div class="bg-brand-dark p-4 rounded-xl border border-gray-800">
            <div class="text-xs text-gray-400">eFootball (Solo)</div>
            <div id="statEFCount" class="text-2xl font-heading font-black text-brand-emerald">0</div>
          </div>
          <div class="bg-brand-dark p-4 rounded-xl border border-gray-800">
            <div class="text-xs text-gray-400">MLBB (Pasukan)</div>
            <div id="statMLCount" class="text-2xl font-heading font-black text-brand-gold">0</div>
          </div>
          <div class="bg-brand-dark p-4 rounded-xl border border-gray-800">
            <div class="text-xs text-gray-400">Jumlah Kutipan Yuran</div>
            <div id="statTotalFees" class="text-2xl font-heading font-black text-brand-cyan">RM 0.00</div>
          </div>
        </div>

        <!-- Filter & Search Controls -->
        <div class="flex flex-col sm:flex-row gap-3">
          <input type="text" id="adminSearchInput" oninput="renderAdminTable()" placeholder="Cari Nama / Pasukan / No Tel / ID..." class="flex-grow bg-brand-dark border border-gray-800 rounded-xl px-4 py-2 text-xs text-white focus:outline-none focus:border-brand-emerald">
          <select id="adminCategoryFilter" onchange="renderAdminTable()" class="bg-brand-dark border border-gray-800 rounded-xl px-4 py-2 text-xs text-white">
            <option value="ALL">Semua Kategori</option>
            <option value="eFootball">eFootball</option>
            <option value="Mobile Legends">Mobile Legends</option>
          </select>
          <select id="adminStatusFilter" onchange="renderAdminTable()" class="bg-brand-dark border border-gray-800 rounded-xl px-4 py-2 text-xs text-white">
            <option value="ALL">Semua Status</option>
            <option value="PENDING">PENDING</option>
            <option value="VERIFIED">VERIFIED</option>
            <option value="REJECTED">REJECTED</option>
          </select>
        </div>

        <!-- Data Table -->
        <div class="overflow-x-auto border border-gray-800 rounded-2xl">
          <table class="w-full text-left text-xs text-gray-300">
            <thead class="bg-brand-dark text-gray-400 font-heading text-[11px] uppercase tracking-wider border-b border-gray-800">
              <tr>
                <th class="p-3">No. Reg</th>
                <th class="p-3">Kategori</th>
                <th class="p-3">Nama / Pasukan</th>
                <th class="p-3">Telefon</th>
                <th class="p-3">Jumlah</th>
                <th class="p-3">Status</th>
                <th class="p-3 text-center">Tindakan Admin</th>
              </tr>
            </thead>
            <tbody id="adminTableBody" class="divide-y divide-gray-800">
              <!-- Rendered via JS -->
            </tbody>
          </table>
        </div>

      </div>

    </div>
  </div>

  <!-- JAVASCRIPT LOGIC -->
  <script>
    /* =========================================================
       STATE MANAGEMENT & MOCK DATA
       ========================================================= */
    const ADMIN_PIN = "admin2026";
    let selectedCategory = "eFootball";
    let selectedFileBase64 = null;

    // Initial Mock Registrations
    const initialRegistrations = [
      {
        id: "EST2026-EF-1001",
        category: "eFootball",
        name: "Muhammad Danish",
        phone: "0178829102",
        email: "danish@gmail.com",
        ign: "Danish_Pro",
        gameId: "902-182-391",
        fee: 5,
        status: "VERIFIED",
        date: "2026-10-01"
      },
      {
        id: "EST2026-EF-1002",
        category: "eFootball",
        name: "Amirul Haziq",
        phone: "0192384711",
        email: "amirul@gmail.com",
        ign: "Haz_Striker",
        gameId: "123-948-201",
        fee: 5,
        status: "PENDING",
        date: "2026-10-01"
      },
      {
        id: "EST2026-ML-2001",
        category: "Mobile Legends",
        name: "Perak Apex Gaming",
        captain: "Khairul Nizam",
        phone: "0139928172",
        email: "apex@gmail.com",
        players: "1. Khairul Nizam\n2. Hafizudin\n3. Luqman Hakim\n4. Azman Syafiq\n5. Zikri Ahmad",
        fee: 10,
        status: "VERIFIED",
        date: "2026-10-01"
      }
    ];

    // Load from localStorage or set defaults
    function getStoredRegistrations() {
      const stored = localStorage.getItem("smart_ummah_registrations");
      if (stored) {
        try { return JSON.parse(stored); } catch(e) {}
      }
      localStorage.setItem("smart_ummah_registrations", JSON.stringify(initialRegistrations));
      return initialRegistrations;
    }

    function saveRegistrations(data) {
      localStorage.setItem("smart_ummah_registrations", JSON.stringify(data));
    }

    /* =========================================================
       COUNTDOWN TIMER LOGIC
       ========================================================= */
    function initCountdown() {
      // Event Date: October 10, 2026 08:00:00
      const targetDate = new Date("October 10, 2026 08:00:00").getTime();

      function update() {
        const now = new Date().getTime();
        const diff = targetDate - now;

        if (diff <= 0) {
          document.getElementById("cd-days").innerText = "00";
          document.getElementById("cd-hours").innerText = "00";
          document.getElementById("cd-mins").innerText = "00";
          document.getElementById("cd-secs").innerText = "00";
          return;
        }

        const days = Math.floor(diff / (1000 * 60 * 60 * 24));
        const hours = Math.floor((diff % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
        const mins = Math.floor((diff % (1000 * 60 * 60)) / (1000 * 60));
        const secs = Math.floor((diff % (1000 * 60)) / 1000);

        document.getElementById("cd-days").innerText = String(days).padStart(2, "0");
        document.getElementById("cd-hours").innerText = String(hours).padStart(2, "0");
        document.getElementById("cd-mins").innerText = String(mins).padStart(2, "0");
        document.getElementById("cd-secs").innerText = String(secs).padStart(2, "0");
      }

      update();
      setInterval(update, 1000);
    }

    /* =========================================================
       CATEGORY & FORM SWITCHING
       ========================================================= */
    function selectCategoryInForm(category) {
      selectedCategory = category;
      document.getElementById("inputCategory").value = category;

      const btnEF = document.getElementById("btn-cat-ef");
      const btnML = document.getElementById("btn-cat-ml");
      const fieldsEF = document.getElementById("fields-eFootball");
      const fieldsML = document.getElementById("fields-MLBB");
      const feeDisplay = document.getElementById("feeDisplay");

      if (category === 'eFootball') {
        btnEF.className = "py-4 px-4 rounded-xl border-2 border-brand-emerald bg-brand-emerald/10 text-white font-heading font-bold text-sm sm:text-base flex flex-col items-center gap-1 transition shadow-lg";
        btnML.className = "py-4 px-4 rounded-xl border-2 border-gray-800 bg-brand-dark/50 text-gray-400 font-heading font-bold text-sm sm:text-base flex flex-col items-center gap-1 transition hover:border-brand-gold";
        
        fieldsEF.classList.remove("hidden");
        fieldsML.classList.add("hidden");
        feeDisplay.innerText = "RM 5.00";

        // Required inputs toggle
        document.getElementById("ef_nama").required = true;
        document.getElementById("ef_phone").required = true;
        document.getElementById("ef_email").required = true;
        document.getElementById("ef_ign").required = true;
        document.getElementById("ef_gameid").required = true;

        document.getElementById("ml_team").required = false;
        document.getElementById("ml_kapten").required = false;
        document.getElementById("ml_phone").required = false;
        document.getElementById("ml_email").required = false;
      } else {
        btnML.className = "py-4 px-4 rounded-xl border-2 border-brand-gold bg-brand-gold/10 text-white font-heading font-bold text-sm sm:text-base flex flex-col items-center gap-1 transition shadow-lg";
        btnEF.className = "py-4 px-4 rounded-xl border-2 border-gray-800 bg-brand-dark/50 text-gray-400 font-heading font-bold text-sm sm:text-base flex flex-col items-center gap-1 transition hover:border-brand-emerald";

        fieldsML.classList.remove("hidden");
        fieldsEF.classList.add("hidden");
        feeDisplay.innerText = "RM 10.00";

        // Required inputs toggle
        document.getElementById("ef_nama").required = false;
        document.getElementById("ef_phone").required = false;
        document.getElementById("ef_email").required = false;
        document.getElementById("ef_ign").required = false;
        document.getElementById("ef_gameid").required = false;

        document.getElementById("ml_team").required = true;
        document.getElementById("ml_kapten").required = true;
        document.getElementById("ml_phone").required = true;
        document.getElementById("ml_email").required = true;
      }
    }

    /* =========================================================
       FILE UPLOAD PREVIEW
       ========================================================= */
    function handleFilePreview(input) {
      if (input.files && input.files[0]) {
        const file = input.files[0];
        
        // Validation for size (max 5MB)
        if (file.size > 5 * 1024 * 1024) {
          alert("Saiz fail melebihi 5MB. Sila muat naik resit yang lebih kecil.");
          input.value = "";
          return;
        }

        document.getElementById("fileName").innerText = file.name;
        document.getElementById("filePreviewContainer").classList.remove("hidden");
        
        const reader = new FileReader();
        reader.onload = function(e) {
          selectedFileBase64 = e.target.result;
        };
        reader.readAsDataURL(file);
      }
    }

    function resetFileUpload() {
      document.getElementById("proofUpload").value = "";
      document.getElementById("filePreviewContainer").classList.add("hidden");
      selectedFileBase64 = null;
    }

    /* =========================================================
       FORMAT TAB SWITCHING
       ========================================================= */
    function switchFormatTab(tab) {
      const tabEF = document.getElementById("tab-efootball");
      const tabML = document.getElementById("tab-mlbb");
      const btnEF = document.getElementById("tab-ef-btn");
      const btnML = document.getElementById("tab-ml-btn");

      if (tab === 'efootball') {
        tabEF.classList.remove("hidden");
        tabML.classList.add("hidden");
        btnEF.className = "py-3 px-6 font-heading font-bold text-sm border-b-2 border-brand-emerald text-brand-emerald transition flex items-center gap-2";
        btnML.className = "py-3 px-6 font-heading font-bold text-sm border-b-2 border-transparent text-gray-400 hover:text-white transition flex items-center gap-2";
      } else {
        tabML.classList.remove("hidden");
        tabEF.classList.add("hidden");
        btnML.className = "py-3 px-6 font-heading font-bold text-sm border-b-2 border-brand-gold text-brand-gold transition flex items-center gap-2";
        btnEF.className = "py-3 px-6 font-heading font-bold text-sm border-b-2 border-transparent text-gray-400 hover:text-white transition flex items-center gap-2";
      }
    }

    /* =========================================================
       SUBMIT REGISTRATION FORM
       ========================================================= */
    function handleRegistrationSubmit(event) {
      event.preventDefault();

      const list = getStoredRegistrations();
      const randomDigits = Math.floor(1000 + Math.random() * 9000);
      let regRecord = {};

      if (selectedCategory === "eFootball") {
        const phone = document.getElementById("ef_phone").value.trim();
        const gameId = document.getElementById("ef_gameid").value.trim();

        // Check duplicates
        const duplicate = list.find(item => item.phone === phone || item.gameId === gameId);
        if (duplicate) {
          alert("Peringatan: Nombor telefon atau Game ID ini telah didaftarkan sebelum ini.");
          return;
        }

        regRecord = {
          id: `EST2026-EF-${randomDigits}`,
          category: "eFootball",
          name: document.getElementById("ef_nama").value.trim(),
          phone: phone,
          email: document.getElementById("ef_email").value.trim(),
          ign: document.getElementById("ef_ign").value.trim(),
          gameId: gameId,
          fee: 5,
          status: "PENDING",
          date: new Date().toISOString().split('T')[0],
          proof: selectedFileBase64
        };
      } else {
        const team = document.getElementById("ml_team").value.trim();
        const captain = document.getElementById("ml_kapten").value.trim();
        const phone = document.getElementById("ml_phone").value.trim();

        // Check duplicate team/phone
        const duplicate = list.find(item => item.phone === phone || (item.name && item.name.toLowerCase() === team.toLowerCase()));
        if (duplicate) {
          alert("Peringatan: Nama pasukan atau nombor telefon ini telah didaftarkan.");
          return;
        }

        const p1 = document.getElementById("ml_p1_nama").value || captain;
        const p1_id = document.getElementById("ml_p1_id").value || "-";
        const p2 = document.getElementById("ml_p2_nama").value || "Pemain 2";
        const p2_id = document.getElementById("ml_p2_id").value || "-";
        const p3 = document.getElementById("ml_p3_nama").value || "Pemain 3";
        const p3_id = document.getElementById("ml_p3_id").value || "-";
        const p4 = document.getElementById("ml_p4_nama").value || "Pemain 4";
        const p4_id = document.getElementById("ml_p4_id").value || "-";
        const p5 = document.getElementById("ml_p5_nama").value || "Pemain 5";
        const p5_id = document.getElementById("ml_p5_id").value || "-";

        regRecord = {
          id: `EST2026-ML-${randomDigits}`,
          category: "Mobile Legends",
          name: team,
          captain: captain,
          phone: phone,
          email: document.getElementById("ml_email").value.trim(),
          players: `1. ${p1} (${p1_id})\n2. ${p2} (${p2_id})\n3. ${p3} (${p3_id})\n4. ${p4} (${p4_id})\n5. ${p5} (${p5_id})`,
          fee: 10,
          status: "PENDING",
          date: new Date().toISOString().split('T')[0],
          proof: selectedFileBase64
        };
      }

      // Save record
      list.push(regRecord);
      saveRegistrations(list);

      // Populate Success Slip Modal
      document.getElementById("slipRegNo").innerText = regRecord.id;
      document.getElementById("slipCategory").innerText = regRecord.category;
      document.getElementById("slipName").innerText = regRecord.name;
      document.getElementById("slipFee").innerText = `RM ${regRecord.fee}.00`;
      
      // WhatsApp Link Formatting
      const waMsg = encodeURIComponent(
        `Salam Admin, Saya telah mendaftar Esport Tour Smart Ummah 2026.\n\n` +
        `*No. Pendaftaran:* ${regRecord.id}\n` +
        `*Kategori:* ${regRecord.category}\n` +
        `*Nama/Team:* ${regRecord.name}\n` +
        `*No Tel:* ${regRecord.phone}\n\n` +
        `Sila sahkan penyertaan dan resit pembayaran saya. Terima kasih!`
      );
      document.getElementById("btnWhatsappSlip").href = `https://wa.me/60123456789?text=${waMsg}`;

      // Show Modal & Reset Form
      document.getElementById("successModal").classList.remove("hidden");
      document.getElementById("regForm").reset();
      resetFileUpload();
      selectCategoryInForm('eFootball');
    }

    function closeSuccessModal() {
      document.getElementById("successModal").classList.add("hidden");
    }

    /* =========================================================
       ADMIN DASHBOARD LOGIC
       ========================================================= */
    function toggleAdminModal() {
      const modal = document.getElementById("adminModal");
      modal.classList.toggle("hidden");
    }

    function verifyAdminPin() {
      const pin = document.getElementById("adminPin").value;
      if (pin === ADMIN_PIN) {
        document.getElementById("adminAuthScreen").classList.add("hidden");
        document.getElementById("adminDashboardContent").classList.remove("hidden");
        renderAdminTable();
      } else {
        alert("PIN Admin Tidak Sah. Sila cuba lagi.");
      }
    }

    function logoutAdmin() {
      document.getElementById("adminPin").value = "";
      document.getElementById("adminAuthScreen").classList.remove("hidden");
      document.getElementById("adminDashboardContent").classList.add("hidden");
      toggleAdminModal();
    }

    function renderAdminTable() {
      const list = getStoredRegistrations();
      const search = document.getElementById("adminSearchInput").value.toLowerCase();
      const catFilter = document.getElementById("adminCategoryFilter").value;
      const statusFilter = document.getElementById("adminStatusFilter").value;

      // Statistics
      const totalCount = list.length;
      const efCount = list.filter(i => i.category === 'eFootball').length;
      const mlCount = list.filter(i => i.category === 'Mobile Legends').length;
      const totalFees = list.reduce((sum, item) => sum + (item.status === 'VERIFIED' ? item.fee : 0), 0);

      document.getElementById("statTotalCount").innerText = totalCount;
      document.getElementById("statEFCount").innerText = efCount;
      document.getElementById("statMLCount").innerText = mlCount;
      document.getElementById("statTotalFees").innerText = `RM ${totalFees}.00`;

      // Filter Data
      const filtered = list.filter(item => {
        const matchesSearch = item.name.toLowerCase().includes(search) || 
                              item.phone.includes(search) || 
                              item.id.toLowerCase().includes(search);
        const matchesCat = catFilter === "ALL" || item.category === catFilter;
        const matchesStatus = statusFilter === "ALL" || item.status === statusFilter;
        return matchesSearch && matchesCat && matchesStatus;
      });

      const tbody = document.getElementById("adminTableBody");
      tbody.innerHTML = "";

      if (filtered.length === 0) {
        tbody.innerHTML = `<tr><td colspan="7" class="p-6 text-center text-gray-500">Tiada rekod pendaftaran ditemui.</td></tr>`;
        return;
      }

      filtered.forEach((item) => {
        const tr = document.createElement("tr");
        tr.className = "hover:bg-brand-dark/50 transition border-b border-gray-800";

        let badgeColor = "bg-amber-500/20 text-amber-400 border-amber-500/30";
        if (item.status === "VERIFIED") badgeColor = "bg-green-500/20 text-green-400 border-green-500/30";
        if (item.status === "REJECTED") badgeColor = "bg-red-500/20 text-red-400 border-red-500/30";

        tr.innerHTML = `
          <td class="p-3 font-mono font-bold text-gray-200">${item.id}</td>
          <td class="p-3 font-semibold ${item.category === 'eFootball' ? 'text-brand-emerald' : 'text-brand-gold'}">${item.category}</td>
          <td class="p-3 font-medium text-white">${item.name} ${item.captain ? `<br><span class="text-[10px] text-gray-400">Kapten: ${item.captain}</span>` : ''}</td>
          <td class="p-3 text-gray-300">${item.phone}</td>
          <td class="p-3 font-bold text-brand-gold">RM ${item.fee}.00</td>
          <td class="p-3">
            <span class="px-2 py-0.5 rounded text-[10px] font-bold border ${badgeColor}">
              ${item.status}
            </span>
          </td>
          <td class="p-3 text-center space-x-1">
            <button onclick="updateStatus('${item.id}', 'VERIFIED')" class="px-2 py-1 bg-green-600 hover:bg-green-500 text-white rounded text-[10px] font-bold" title="Sahkan">
              <i class="fa-solid fa-check"></i>
            </button>
            <button onclick="updateStatus('${item.id}', 'REJECTED')" class="px-2 py-1 bg-red-600 hover:bg-red-500 text-white rounded text-[10px] font-bold" title="Tolak">
              <i class="fa-solid fa-xmark"></i>
            </button>
            <button onclick="deleteRecord('${item.id}')" class="px-2 py-1 bg-gray-700 hover:bg-gray-600 text-gray-300 rounded text-[10px] font-bold" title="Padam">
              <i class="fa-solid fa-trash"></i>
            </button>
          </td>
        `;
        tbody.appendChild(tr);
      });
    }

    function updateStatus(id, newStatus) {
      let list = getStoredRegistrations();
      const index = list.findIndex(i => i.id === id);
      if (index !== -1) {
        list[index].status = newStatus;
        saveRegistrations(list);
        renderAdminTable();
      }
    }

    function deleteRecord(id) {
      if (window.confirm("Adakah anda pasti mahu memadam rekod pendaftaran ini?")) {
        let list = getStoredRegistrations();
        list = list.filter(i => i.id !== id);
        saveRegistrations(list);
        renderAdminTable();
      }
    }

    function exportDataCSV() {
      const list = getStoredRegistrations();
      if (list.length === 0) {
        alert("Tiada data untuk dieksport.");
        return;
      }

      let csvContent = "data:text/csv;charset=utf-8,ID,Kategori,Nama/Pasukan,Telefon,Email,Status,Yuran(RM),Tarikh\n";
      list.forEach(r => {
        csvContent += `"${r.id}","${r.category}","${r.name}","${r.phone}","${r.email}","${r.status}","${r.fee}","${r.date}"\n`;
      });

      const encodedUri = encodeURI(csvContent);
      const link = document.createElement("a");
      link.setAttribute("href", encodedUri);
      link.setAttribute("download", `Pendaftaran_Esport_Smart_Ummah_2026.csv`);
      document.body.appendChild(link);
      link.click();
      document.body.removeChild(link);
    }

    /* =========================================================
       MOBILE MENU TOGGLE
       ========================================================= */
    function toggleMobileMenu() {
      const menu = document.getElementById("mobileMenu");
      menu.classList.toggle("hidden");
    }

    /* =========================================================
       PAGE INITIALIZATION
       ========================================================= */
    window.onload = function() {
      initCountdown();
      getStoredRegistrations();
    };
  </script>

</body>
</html>