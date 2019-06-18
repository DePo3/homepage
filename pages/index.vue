<template>
  <section class="container-wrapper">
    <Cover/>
    <Cv/>
    <Info/>
    <Footer/>
  </section>
</template>

<script>
import Cover from '../components/Cover'
import Cv from '../components/Cv'
import Info from '../components/Info'
import Footer from '../components/Footer'

export default {
  components: {
    Cover,
    Cv,
    Info,
    Footer
  }
}
</script>

<style>

body {
  color: #1a234d;
}
h1 {
  color: #1a234d;
}
h2 {
  color: #1a234d;
}
h3 {
  color: #1a234d;
}
h4 {
  color: #1a234d;
}
h5 {
  color: #1a234d;
}

</style>
