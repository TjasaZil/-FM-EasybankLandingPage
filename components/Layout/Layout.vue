<script setup lang="ts">
const props = defineProps<{
  class?: string;
}>();
</script>

<template>
  <div
    class="mx-auto h-full w-full max-w-[1312px] px-4 md:w-[calc(100%-3rem)] lg:w-[calc(100%-100px)] lg:px-0"
    :class="props.class"
  >
    <slot />
  </div>
</template>
