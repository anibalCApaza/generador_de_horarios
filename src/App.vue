<script lang="ts" setup>
import CardFeature from './components/CardFeature.vue';

</script>

<template>
  <div class="w-full h-screen p-10 lg:p-20">
    <div class="flex flex-col items-center ">
      <div class="font-bold text-7xl mt-7 mb-2">
        DINASTY
      </div>
      <div class="text-2xl font-medium ">
        Un comodo generador de horarios
      </div>
    </div>

    <div class="flex justify-center m-5">
      <button
        class="text-2xl font-bold bg-gv-yellow p-3 rounded-2xl hover:bg-amber-200 hover:scale-105 fg-gv-black">GENERAR</button>
    </div>

    <div class="flex flex-row gap-4  flex-wrap lg:flex-nowrap">
      <CardFeature bg="bg-gv-green">
        <template #icon-img>
          <img src="@/assets/icons/calendar.svg" alt="">
        </template>

        <template #title>
          Horario personalizado
        </template>
        <template #description>
          Diseña tu horario como lo desees: agrega, edita o elimina materias fácilmente.
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
  </div>
</template>

<style scoped></style>
