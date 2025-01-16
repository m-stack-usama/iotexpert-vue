<script setup>
// import { RouterLink, RouterView } from 'vue-router'
import { ref } from "vue";
import InputText from "primevue/inputtext";
const value = ref(null);
</script>

<template>
  <div
    class="card w-full h-screen flex flex-col items-center justify-center space-y-5"
  >
    <h1 class="text-2xl tracking-wider underline mt-10">
      Say Hello to PrimeVue & TailwindCss!
    </h1>
    <InputText type="text" v-model="value" placeholder="Say something!" />
    {{ value }}
  </div>
  <!--<RouterView /> -->
</template>

<style scoped></style>
