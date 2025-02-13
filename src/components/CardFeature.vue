<script lang="ts" setup>

defineProps<{ bg?: string }>();
</script>

<template>
  <div class="flex grow flex-col p-5 my-1 lg:p-7 fg-gv-black rounded-md gap-y-4" :class="bg">



    <div class="font-bold text-2xl uppercase text-center ">
      <slot name="title"></slot>
    </div>
    <div class="flex  justify-center ">
      <slot name="icon-img">
      </slot>
    </div>
    <div class="text-xl">
      <slot name="description"></slot>
    </div>
  </div>
</template>

<style scoped></style>
