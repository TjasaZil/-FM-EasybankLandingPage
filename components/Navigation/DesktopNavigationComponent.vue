<template>
  <section class="w-full h-20 absolute top-0 left-0 mx-auto bg-white">
    <div
      class="w-10/12 max-w-7xl mx-auto h-full flex justify-between items-center"
    >
      <img alt="easybank logo" src="@/assets/images/logo.svg" class="h-5" />
      <ul class="flex justify-center items-center space-x-14">
        <li
          v-for="text in texts"
          :key="text"
          class="capitalize hover:border-b-4 text-neutral-grayish-blue hover:border-b-primary-bright-cyan text-lg hover:text-primary-dark-blue py-6"
        >
          {{ text }}
        </li>
      </ul>
      <Button text="Request Invite"></Button>
    </div>
  </section>
</template>
<script>
import Button from '../Button/Button.vue';
export default {
  name: 'DesktopNavigationComponent',
  components: { Button },
  data() {
    return {
      texts: ['home', 'about', 'contact', 'blog', 'careers'],
    };
  },
};
</script>
