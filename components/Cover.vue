<template>
  <section>
    <div class="wrapperCover">

      <div>
        <div class="cover" :style="{ backgroundImage: 'url(' + require(`@/assets/pictures/delia_cover.jpg`) + ')' }">
          <!--<img class="djListe" src="~/assets/soliparty-logo1.png>-->
          <div class="titleText">
            <h1 class="pageTitle" style="font-weight:400;">Hey, I am Delia Hallberg</h1>
            <h2 class="pageSubTitle">Consultant // Researcher // Social Scientist // Tech Enthusiast</h2>
            <p class="titleQuote">Technology design is a reflection of social values and norms. We need multidisciplinary collaboration to create human-centric technologies fit for tomorrow's society based on human rights, solidarity and sustainability.</p>
          </div>
        </div>
      </div>

    </div>
  </section>
</template>

<script>

export default {

}

</script>

<style>
@import url('https://fonts.googleapis.com/css?family=Kalam&display=swap');

.titleText {
  width: 50%;
  text-align: center;
  margin-left: 5%;
  padding-top: 17.5%;
}
.pageTitle {
  font-size: 45px;
}
.pageSubTitle {

}
.titleQuote {
  padding-left: 15%;
  padding-right: 15%;
  padding-top: 2em;
  font-family: 'Kalam';
}
.cover {
  max-width: 100%;
  min-height: 100vh;
  width: 100vw;
  -webkit-background-size: cover;
  -moz-background-size: cover;
  -o-background-size: cover;
  background-size: cover;
  background-position: center top;
}
</style>
