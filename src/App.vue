<script lang="ts" setup>
import CardFeature from './components/CardFeature.vue';

</script>

<template>
  <header>
    <nav>
      <ul class="flex justify-end">
        <li class="px-2 text-xl lg:text-2xl">Contacto</li>
      </ul>
    </nav>
  </header>
  <main class="w-full h-screen p-10 lg:p-20">
    <div class="flex flex-col items-center ">
      <div class="font-bold text-6xl mt-7 mb-2 lg:text-8xl">
        DINASTY
      </div>
      <div class="text-xl font-medium lg:text-3xl">
        Un comodo generador de horarios
      </div>
    </div>

    <div class="flex justify-center m-5">
      <button
        class="text-2xl font-bold bg-gv-yellow p-3 rounded-2xl hover:bg-amber-200 hover:scale-105 fg-gv-black">GENERAR</button>
    </div>

    <div class="grid lg:grid-cols-3 gap-5">
      <CardFeature bg="bg-gv-green">
        <template #icon-img>
          <img src="@/assets/icons/calendar.svg" alt="">
        </template>

        <template #title>
          Horario personalizado
        </template>
        <template #description>
          Diseña tu horario como lo desees: agrega, edita o elimina actividades fácilmente.
        </template>
      </CardFeature>

      <CardFeature bg="bg-gv-blue">
        <template #icon-img>
          <img src="@/assets/icons/pen-tool.svg" alt="">
        </template>
        <template #title>
          Paleta de colores
        </template>
        <template #description>
          Selecciona los colores que mejor se adapten a tu estilo y haz tu horario único.
        </template>
      </CardFeature>

      <CardFeature bg="bg-gv-red">
        <template #icon-img>
          <img src="@/assets/icons/file-text.svg" alt="">
        </template>
        <template #title>
          Exportación
        </template>
        <template #description>
          Guarda o comparte tu horario con solo un clic en formato PDF o PNG.
        </template>
      </CardFeature>
    </div>
  </main>
</template>

<style scoped></style>
