<template>
  <section class="container">
    <section class="container-wrapper">
      <Cover/>
      <Info/>
      <CV/>
      <Footer/>
    </section>
  </section>
</template>

<script>
import Cover from '../components/Cover'
import CV from '../components/CV'
import Info from '../components/Info'
import Footer from '../components/Footer'

export default {
  components: {
    Cover,
    CV,
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
.container {
  width: 100vw;
  max-width: 100%;
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  overflow-x: hidden;
}
</style>
