<template>
  <MobileNavigationComponent
    class="z-50 xl:hidden"
  /><DesktopNavigationComponent class="hidden xl:flex z-50" />
</template>
<script>
import MobileNavigationComponent from './MobileNavigationComponent.vue';
import DesktopNavigationComponent from './DesktopNavigationComponent.vue';
export default {
  name: 'NavigationComponent',
  components: { MobileNavigationComponent, DesktopNavigationComponent },
};
</script>
