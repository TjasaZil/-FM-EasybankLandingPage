<template>
  <div>
    <NavigationComponent />
    <EasybankTextComponent />

    <Footer />
  </div>
</template>
<script>
import Footer from './components/Footer/Footer.vue';
import NavigationComponent from './components/Navigation/NavigationComponent.vue';
import EasybankTextComponent from '@/components/Text/EasybankTextComponent.vue';
export default {
  name: 'App',
  components: { Footer, NavigationComponent, EasybankTextComponent },
};
</script>
