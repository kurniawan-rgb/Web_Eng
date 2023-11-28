
<template>
  <header class="header-section" style=" position: fixed; padding: 24px 0 0 0; background-color: #063D63; justify-content: space-between; align-items: center;">
        <div class="container flex justify-between" style="padding: 0 128px;">
            <a href="https://eng.unhas.ac.id/fakultas/" class="site-logo">
                <img src="../assets/unhas_id.png" alt="">
            </a>
              <div class="w-80 h-10 justify-center items-center gap-6 inline-flex icon-find">
                  <div class="w-64 h-10 relative">
                    <div class="w-64 h-10 left-0 top-0 absolute bg-sky-950 rounded-full"></div>
                    <div class="w-24 h-3.5 left-[19.75px] top-[12.59px] absolute text-white text-opacity-60 text-base font-normal font-['Inter']">Mencari...</div>
                  </div>
              </div>
            </div>
    <nav class="navbar" style="margin-top: 20px; padding: 14px 128px; background-color: #EB2629; align-items: center; color: white;"> 
        <div class="navbar-nav flex space-x-10 center">
            <a href="#">PROFIL</a>
            <a href="#">SUMBER DAYA</a>
            <a href="#">KEMAHASISWAAN</a>
            <a href="#">RISET DAN INOVASI</a>
            <a href="#">KEMITRAAN</a>
            <a href="#">GPM-PR</a>
            <a href="#">COT</a>
        </div>
    </nav>
  </header>
  
  <body>
    <section class="Hero">
        <img style="width: 100%;" src="../assets/bg.png" alt="">
    </section>
    
    <section class="Sambutan flex" style="padding: 24px 128px; margin: 80px 0;">
        <img src="../assets/Foto Dekan.png" alt="">
        <div class="px-14">
            <div class="flex gap-4">
                <h1 id="Sambutan" class="text-4xl font-semibold" style="color: #063D63;">SAMBUTAN DEKAN</h1>
                <img src="../assets/Garis1.png" alt="" style="height: 4px; width: 320px; margin-top: 20px;">
            </div>
            <p class="text-white text-justify py-6" style="color: black;">"Assalamu Alaikum Wr. Wb. Puji syukur kehadirat Tuhan Yang Maha Kuasa atas limpahan rahmat dan hidayah-Nya sehingga informasi tentang Fakultas Teknik Unhas melalui situs web ini dapat terwujud. Besar harapan kita semoga ridho-Nya menyertai segala aktifitas dalam upaya pembinaan sumber daya manusia dalam bidang teknologi dan semoga informasi melalui web ini dapat berguna bagi semua pihak. Kami dari semua civitas akademika Fakultas Teknik dengan semua dukungan komponen perguruan tinggi yang ada akan terus meningkatkan pencapaian menuju terwujudnya visi dan misi yang telah dicanangkan dalam rencana strategis fakultas. Semoga informasi yang diberikan lewat layanan website ini dapat memberikan gambaran situasi dan kondisi Fakultas Teknik kepada semua lapisan masyarakat. Selamat Datang di Fakultas Teknik Universitas Hasanuddin.</p>
            <br style="margin-bottom: 20px;">
            <p>Wassalam"</p>
            <h1 class="text-2xl font-semibold" style="color: black;">Prof. Dr. Eng. Ir. Muhammad Isran Ramli, S.T., M.T., IPM., ASEAN Eng.</h1>
        </div>
    </section>

    <!-- Section Galeri -->
    <section>
      <GaleriSlider></GaleriSlider>
    </section>

    <section class="Berita px-16 mt-8" style="padding: 24px 128px;">
      <BeritaEng></BeritaEng>
    </section>

    <section class="Informasi px-16 mt-[10px] top-49" style="padding: 204px 128px;">
        <div class="flex justify-between">
            <div class="flex gap-4">
                <h1 class="text-4xl font-semibold" style="color: #063D63;">INFORMASI</h1>
                <img src="../assets/Garis1.png" alt="" style="height: 4px; width: 320px; margin-top: 20px;">
            </div>
            <div style="margin-top: 10px; text-decoration-line: underline; text-decoration-color: #063D63;">
                <a href="#" class="text-base font-medium" style="color: #063D63;">Lihat semua informasi -></a>
            </div>
        </div>
        <div class="grid gap-x-6 gap-y-8 grid-cols-2">
            <div class="py-4 px-8 my-20 mx-12" style="background-color: #f4f4f4;">
                <h1 class="text-sm max-w-lg font-semibold">THE 3RD EPI INTERNATIONAL CONFERENCE ON SCIENCE AND ENGINEERING 2019</h1>
                <div class="flex pt-5">
                    <img src="../assets/kalender.png" alt="">
                    <p class="text-xs" style="padding: 2px 0 0 8px;">23 September 2019</p>
                </div>
            </div>
            <div class="py-4 px-8 my-20 mx-12" style="background-color: #f4f4f4;">
                <h1 class="text-sm max-w-lg font-semibold">WORKSHOP & SIMPOSIUM NASIONAL GEOMEKANIKA 5 2019</h1>
                <div class="flex pt-5">
                    <img src="../assets/kalender.png" alt="">
                    <p class="text-xs" style="padding: 2px 0 0 8px;">06 Agustus 2019</p>
                </div>
            </div>
            <div class="py-4 px-8 my-20 mx-12" style="background-color: #f4f4f4;"> 
                <h1 class="text-sm max-w-lg font-semibold">Pengembangan Karakter Mahasiswa Baru 2019 Fakultas Teknik Unhas</h1>
                <div class="flex pt-5">
                    <img src="../assets/kalender.png" alt="">
                    <p class="text-xs" style="padding: 2px 0 0 8px;">09 Juli 2019</p>
                </div>
            </div>
            <div class="py-4 px-8 my-20 mx-12" style="background-color: #f4f4f4;">
                <h1 class="text-sm max-w-lg font-semibold">International Guest Lecture on Journal Article</h1>
                <div class="flex pt-5">
                    <img src="../assets/kalender.png" alt="">
                    <p class="text-xs" style="padding: 2px 0 0 8px;">25 Juni 2019</p>
                </div>
            </div>
        </div>
    </section>
  </body>

  <footer>
    <div class="w-1512 h-554 relative">
    <img class="w-1512 h-554  left-0 top-0 absolute" src="https://via.placeholder.com/1512x554" />
    <div class="w-72 h-4 left-[606px] top-[504.04px] absolute text-center text-zinc-400 text-base font-normal font-['Inter'] leading-snug">Copyright © 2022 All rights reserved</div>
    <div class="w-36 h-28 left-[944px] top-[247px] absolute flex-col justify-start items-start gap-6 inline-flex">
        <div class="text-center text-white text-base font-bold font-['Inter']">DIDUKUNG OLEH</div>
        <div class="justify-start items-start gap-4 inline-flex">
            <div class="w-14 h-16 flex-col justify-center items-center inline-flex">
                <img class="w-14 h-16" src="https://via.placeholder.com/60x62" />
            </div>
            <div class="w-16 h-16 justify-center items-center flex">
                <img class="w-16 h-16" src="https://via.placeholder.com/67x62" />
            </div>
        </div>
    </div>
    <div class="w-16 h-5 left-[944px] top-[83px] absolute flex-col justify-start items-start gap-6 inline-flex">
        <div class="text-center text-white text-base font-bold font-['Inter']">ALAMAT</div>
    </div>
    <div class="w-96 h-40 left-[168px] top-[247px] absolute flex-col justify-start items-start gap-6 inline-flex">
        <div class="text-center text-white text-base font-normal font-['Inter']">+62 852-9999-9958</div>
        <div class="w-40 h-7 justify-center items-center inline-flex">
            <div class="w-40 h-7 text-white text-base font-normal font-['Inter']">teknik@unhas.ac.id</div>
        </div>
        <div class="justify-start items-start gap-6 inline-flex">
            <div class="w-6 h-7 relative flex-col justify-start items-start inline-flex"></div>
            <div class="grow shrink basis-0 self-stretch px-px py-px flex-col justify-center items-center inline-flex"></div>
            <div class="w-6 h-7 relative flex-col justify-start items-start inline-flex"></div>
            <div class="grow shrink basis-0 self-stretch flex-col justify-center items-center inline-flex"></div>
            <div class="w-96 h-14 justify-center items-center flex">
                <div class="w-96 h-14 text-white text-base font-normal font-['Inter']">Jl. Malino No.8 F, Romang Lompoa, Kec. Bontomarannu, Kabupaten Gowa, Sulawesi Selatan 92171</div>
            </div>
        </div>
    </div>
    <img class="w-96 h-20 left-[156px] top-[80.02px] absolute" src="https://via.placeholder.com/533x80" />
</div>
  </footer>

</template>
<script>
import GaleriSlider from '../components/GaleriSlider.vue'
import BeritaEng from '../components/BeritaEng.vue';
export default {
  components: { GaleriSlider, BeritaEng },
  name: 'HomeView',
}
</script>

<style scoped>
:root {
    --bg1 : #063D63;
    --bg2 : #EB2629;
}


.header-section {
    justify-content: space-between;
    align-items: center;
    position: fixed;
    top: 0;
    left: 0;
    right: 0;
    background-color: #063D63;
    z-index: 99;
}

.icon-find{
  margin-right: -50em;
}

.header-section img {
    width: 300px;
}

.navbar-nav a:hover {
    color: #063D63;
}
</style>



