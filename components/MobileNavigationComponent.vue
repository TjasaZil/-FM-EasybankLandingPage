<template>
  <section class="w-full h-16 absolute top-0 left-0 mx-auto">
    <div class="w-full h-full flex justify-between items-center px-4 bg-white">
      <img alt="easybank logo" src="@/assets/images/logo.svg" class="h-5" />
      <img
        v-if="menuIsOpen"
        alt="mobile hamburger icon"
        src="@/assets/images/icon-hamburger.svg"
        class="w-10 h-5 hover:cursor-pointer"
        @click="openMenu"
      />
      <div v-else>
        <img
          alt="mobile hamburger icon"
          src="@/assets/images/icon-close.svg"
          class="w-5 h-5 hover:cursor-pointer"
          @click="openMenu"
        />
        <ul
          class="bg-gradient-to-b from-blue-900 to-blue-50 w-full absolute top-16 left-0 mx-auto text-center pt-7 h-screen"
        >
          <li
            v-for="text in texts"
            :key="text"
            class="bg-white w-11/12 mx-auto capitalize py-6 text-2xl hover:underline hover:font-semibold"
          >
            {{ text }}
          </li>
        </ul>
      </div>
    </div>
  </section>
</template>
<script>
export default {
  name: 'MobileNavigationComponent',
  data() {
    return {
      menuIsOpen: true,
      texts: ['home', 'about', 'contact', 'blog', 'careers'],
    };
  },

  methods: {
    openMenu() {
      this.menuIsOpen = !this.menuIsOpen;
    },
  },
};
</script>
