<template>
  <section>

        <div class="cv">
          <img class="cvImage" src="~/assets/pictures/delia_cv.png">
        </div>

  </section>
</template>

<script>

export default {

}

</script>

<style>

.cvImage {
  padding-left: 2em;
  padding-right: 2em;
  display: block;
  margin: 0 auto;
  max-height: 100%;
  max-width: 100%;
}

.cv {
  max-width: 100%;
}

@media screen and (min-width: 1600px) {

}
@media screen and (max-width: 880px) {
  
  .cover {
    max-width: 100%;
    min-height: 100vh;
    -webkit-background-size: cover;
    -moz-background-size: cover;
    -o-background-size: cover;
    background-size: cover;
    background-position: center top;
  }
  .solipartyMapucheText {
    position: absolute;
    left: 50%;
    padding-top: 2em;
    padding-bottom: 2em;
    margin-left: -45%;
    margin-top: 2em;
    width: 90%;
  }
}
/* If height very low */
@media screen and (max-height: 500px) {
  .solipartyMapucheText {
    display: block;
    margin-left: auto;
    margin-right: auto;
    padding-top: 2em;
    padding-bottom: 2em;
    width: 90%;
    max-height: 100%;
  }
}

</style>
