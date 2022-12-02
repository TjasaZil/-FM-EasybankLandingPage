<template>
  <div>
    <NavigationComponent />
    <main>
      <Hero />
      <EasybankTextComponent />
      <ArticleComponent />
    </main>

    <Footer />
  </div>
</template>
<script>
import Hero from './components/Hero/Hero.vue';
import Footer from './components/Footer/Footer.vue';
import NavigationComponent from './components/Navigation/NavigationComponent.vue';
import EasybankTextComponent from '@/components/Text/EasybankTextComponent.vue';
export default {
  name: 'App',
  components: { Footer, NavigationComponent, EasybankTextComponent },
};
</script>
