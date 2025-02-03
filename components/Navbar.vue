<template>
    <nav class="bg-white shadow-md py-4 px-6">
      <div class="container mx-auto flex justify-between items-center">
        <div class="text-xl font-bold text-gray-800">Ticketing App</div>
        <ul class="flex space-x-6">
          <li><NuxtLink to="/" class="text-gray-700 hover:text-blue-500">Beranda</NuxtLink></li>
          <li><NuxtLink to="/blog" class="text-gray-700 hover:text-blue-500">Acara</NuxtLink></li>
          <li><NuxtLink to="/about" class="text-gray-700 hover:text-blue-500">Tentang Kami</NuxtLink></li>
          <li>
            <button class="bg-blue-500 text-white px-4 py-2 rounded hover:bg-blue-600">Login</button>
          </li>
        </ul>
      </div>
    </nav>
  </template>
  
  <script>
  export default {
    name: 'Navbar',
  };
  </script>