<template>
  <MobileNavigationComponent class="xl:hidden" /><DesktopNavigationComponent
    class="hidden xl:flex"
  />
</template>
<script>
import MobileNavigationComponent from './MobileNavigationComponent.vue';
import DesktopNavigationComponent from './DesktopNavigationComponent.vue';
export default {
  name: 'NavigationComponent',
  components: { MobileNavigationComponent, DesktopNavigationComponent },
};
</script>
