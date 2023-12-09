<template>
      <div class="flex justify-between">
            <div class="flex gap-4">
                <h1 class="text-4xl font-semibold" style="color: #063D63;">BERITA</h1>
                <img src="../assets/Garis1.png" alt="" style="height: 4px; width: 320px; margin-top: 20px;">
            </div>
            <div style="margin-top: 10px; text-decoration-line: underline; text-decoration-color: #063D63;">
                <a href="#" class="text-base font-medium" style="color: #063D63;">Lihat semua berita -></a>
            </div>
        </div>
        <div class="w-100 h-80 relative">
          <div class="w-96 h-80 left-0 top-0 absolute bg-gray-50"></div>
          <div class="left-[510px] top-[20px] absolute text-base  text-center text-neutral-500 text-xl font-semibold font-['Inter']">24 Oktober 2022</div>
    
    <div class="w-200 h-24 left-[511px] top-[134px] absolute justify-center items-center inline-flex">
        <div class="w-100 h-24 text-justify text-neutral-500 text-xl font-normal font-['Inter']">Acara puncak Dies Natalis ke-62 FT Unhas dihadiri oleh Rektor Unhas, Bapak Prof. Dr. Ir. Jamaluddin Jompa, M.Sc. para wakil Rektor, Dekan, Direktur, dan jajaran pimpinan Unhas. Juga hadir beberapa tamu undangan, baik dari...</div>
    </div>
    <div class="w-100 h-9 left-[511px] top-[78px] absolute justify-center items-center inline-flex">
        <div class="text-center text-black text-3xl font-semibold font-['Inter']">Puncak Dies Natalis ke-62, FT-UH</div>
    </div>
    <img class="w-95 h-80 left-0 top-4 absolute" src="../assets/main_berita.png" />
    <div class="w-28 h-5 left-[511px] top-[300px] absolute text-sky-900 text-base font-semibold font-['Inter']">Selengkapnya</div>
</div>

<div class="flex">
  <div class=" w-96 h-96 mt-10 relative">
    <div class="w-96 h-96 left-0 top-0 absolute bg-gray-50"></div>
    <div class="w-80 h-32 left-[19.50px] top-[266px] absolute justify-center items-center inline-flex">
        <div class="w-80 h-32 text-black text-xl font-semibold font-['Inter']">Kunjungan Kerja Fakultas Sipil dan Perencanaan Universitas Balikpapan Dalam Rangka Studi Banding Tinjauan Kurikulum Pendidikan</div>
    </div>
    <img class="w-96 h-64 left-0 top-20px absolute" src="../assets/berita1.png" />
    <div class="w-28 h-5 left-[245.50px] top-[500px] absolute text-sky-900 text-base font-semibold font-['Inter']">Selengkapnya</div>
    <div class="w-32 h-5 left-[19.50px] top-[500px] absolute text-neutral-500 text-base font-semibold font-['Inter']">24 Oktober 2022</div>
</div>
<div class="w-96 h-96 mx-5 mt-10 relative">
    <div class="w-96 h-96 left-[0.14px] top-0 absolute bg-gray-50"></div>
    <div class="w-80 h-32 left-[19.64px] top-[266px] absolute justify-center items-center inline-flex">
        <div class="w-80 h-32  text-black text-xl font-semibold font-['Inter']">Kerjasama Penyelenggaraan PS PPI Antara Fakultas Teknik Universitas Hasanuddin dengan Fakultas Teknik Universitas Halu Oleo</div>
    </div>
    <img class="w-96 h-64 left-0 top-[0.46px] absolute" src="../assets/berita2.png" />
    <div class="w-28 h-5 left-[245.64px] top-[500px] absolute text-sky-900 text-base font-semibold font-['Inter']">Selengkapnya</div>
    <div class="w-32 h-5 left-[19.64px] top-[500px] absolute text-neutral-500 text-base font-semibold font-['Inter']">24 Oktober 2022</div>
</div>
<div class="w-96 h-96 mx-4 mt-10 relative">
    <div class="w-96 h-96 left-0 top-0 absolute bg-gray-50"></div>
    <div class="w-80 h-32 left-[19.50px] top-[266px] absolute justify-center items-center inline-flex">
        <div class="w-80 h-32 text-black text-xl font-semibold font-['Inter']">Kunjungan Kerja Tim         FT - Universitas Tanjungpura<br/></div>
    </div>
    <img class="w-96 h-64 left-0 top-[0.50px] absolute" src="../assets/berita3.png" />
    <div class="w-28 h-5 left-[245.50px] top-[500px] absolute text-sky-900 text-base font-semibold font-['Inter']">Selengkapnya</div>
    <div class="w-32 h-5 left-[19.50px] top-[500px] absolute text-neutral-500 text-base font-semibold font-['Inter']">24 Oktober 2022</div>
</div>
</div>
<div v-for="post in postData">
    <h1>{{ post.Judul }}</h1>
</div>
</template>
<script>
import { onMounted, ref } from 'vue';

export default {
    name: "BeritaSection"
}

const postData=ref([])

const getPost = async()=> {
    return fetch('http://0.0.0.0:8055/admin/content/beritaWeb')
    .then(response=> response.json())
}

onMounted(() => {
    getPost().then(data => {
        postData.value=data
    })
})
</script>