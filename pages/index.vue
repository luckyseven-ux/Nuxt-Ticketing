<template>
    <div>
      <HeroSection />
      <EventList />
    </div>
  </template>
  
  <script>
  import HeroSection from '~/components/HeroSection.vue';
  import EventList from '~/components/EventList.vue';
  
  export default {
    components: { HeroSection, EventList },
  };
  </script>