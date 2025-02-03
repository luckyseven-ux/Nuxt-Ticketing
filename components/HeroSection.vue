<template>
  <section class="bg-cover bg-top bg-no-repeat h-[500px] flex items-center justify-center text-white"
    :style="{ backgroundImage: `url(${backgroundImage})` }">
    <div class="text-center">
      <h1 class="text-4xl font-bold mb-4">Pesan Tiket Acara Favoritmu Sekarang!</h1>
      <p class="text-lg mb-6">Temukan acara terbaik di kota Anda dan pesan tiket dengan mudah.</p>
      <form class="flex justify-center">
        <input type="text" placeholder="Cari acara..."
          class="w-full md:w-96 px-4 py-2 border rounded-l-md focus:outline-none focus:ring-2 focus:ring-blue-500" />
        <button type="submit"
          class="bg-blue-500 text-white px-6 py-2 rounded-r-md hover:bg-blue-600 transition duration-300">
          Cari
        </button>
      </form>
    </div>
  </section>
</template>

<script >
import backgroundImage from '~/assets/img/uq-contact-taylor-swift-background-3-2560x1440.jpg';

export default {
  name: 'HeroSection',
  data() {
    return {
      backgroundImage
    };
  }
};
</script>
