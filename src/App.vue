<template>
  <div id="app">
    <Header />
    <Banner />
    <main>
        <div class="container_70">
          <Comics />
        </div>
    </main>
    <Prefooter />
    <Footer />
    <References />
    
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Prefooter from "./components/Prefooter.vue";
import Footer from "./components/Footer.vue";
import References from "./components/References.vue";
import Banner from "./components/Banner.vue";
import Comics from "./components/Comics.vue";

export default {
  name: "App",
  components: {
    Header,
    Prefooter,
    Footer,
    References,
    Banner,
    Comics
  },
};
</script>

<style lang="scss">
@import './style/variables.scss';
@import './style/reset.scss';
@import './style/general.scss';
@import url('https://fonts.googleapis.com/css2?family=Mukta:wght@400;600;800&family=Roboto:wght@400;500;900&display=swap');
main{
  color: $secondary_color;
  background-color: #1c1c1c;
  padding: 40px 0 20px;
  position: relative;
}
</style>
