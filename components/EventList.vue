<template>
    <section class="py-12">
      <div class="container mx-auto text-center">
        <h2 class="text-3xl font-bold text-gray-800 mb-8">Acara Populer</h2>
        <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
          <div v-for="(event, index) in events" :key="index" class="bg-white rounded-lg shadow-md overflow-hidden">
            <img :src="event.image" alt="Event Image" class="w-full h-48 object-cover" />
            <div class="p-4">
              <h3 class="text-xl font-semibold text-gray-800">{{ event.title }}</h3>
              <p class="text-gray-600 mt-2">{{ event.date }}</p>
              <button @click="buyTicket(event)"
                class="mt-4 bg-blue-500 text-white px-4 py-2 rounded hover:bg-blue-600 transition duration-300">
                Beli Tiket
              </button>
            </div>
          </div>
        </div>
      </div>
    </section>
  </template>
  
  <script>
  export default {
    data() {
      return {
        events: [
          { title: 'Konser Musik', date: '15 Desember 2023', image: 'https://via.placeholder.com/300x200' },
          { title: 'Pameran Seni', date: '20 Desember 2023', image: 'https://via.placeholder.com/300x200' },
          { title: 'Workshop Fotografi', date: '25 Desember 2023', image: 'https://via.placeholder.com/300x200' },
        ],
      };
    },
    methods: {
      buyTicket(event) {
        alert(`Anda memesan tiket untuk ${event.title}`);
      },
    },
  };
  </script>