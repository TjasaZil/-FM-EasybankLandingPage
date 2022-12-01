<script setup lang="ts">
const props = defineProps<{
  text: string;
  class?: string;
}>();
</script>

<template>
  <button
    class="group relative py-3 px-8 rounded-full text-neutral-white bg-gradient-to-r from-primary-lime-green to-primary-bright-cyan"
    :class="props.class"
  >
    <span
      class="absolute top-0 left-0 w-full h-full bg-neutral-white rounded-full opacity-0 group-hover:opacity-30 duration-200 ease-out"
    ></span>
    {{ props.text }}
  </button>
</template>
