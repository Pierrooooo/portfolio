<template>
  <div>
  <Header />
  <section class="big_container">
    <Skills />
    <Projects />
    </section>
    <Footer />
  </div>
</template>

<script>
import Footer from '../components/Footer.vue'
export default {
    name: "IndexPage",
    data() {
        return {};
    },
    components: { Footer }
}
</script>
