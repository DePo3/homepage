<template>
  <section>
    <div class="wrapperCover">

      <div>
        <div class="coverHeadDesktop" :style="{ backgroundImage: 'url(' + require(`@/assets/pictures/delia_cover.jpg`) + ')' }">
          <!--<img class="djListe" src="~/assets/soliparty-logo1.png>-->
          <div class="titleTextDesktop">
            <h1 class="pageTitleDesktop" style="font-weight:400;">Hey, I am Delia Hallberg</h1>
            <h2 class="pageSubTitleDesktop">Consultant // Researcher // Social Scientist // Tech Enthusiast</h2>
            <p class="titleQuoteDesktop">Technology design is a reflection of social values and norms. We need multidisciplinary collaboration to create human-centric technologies fit for tomorrow's society based on human rights, solidarity and sustainability.</p>
          </div>
        </div>

        <div class="coverHeadTablet" :style="{ backgroundImage: 'url(' + require(`@/assets/pictures/DeliHeaderpicTabletWide.jpg`) + ')' }">
          <!--<img class="djListe" src="~/assets/soliparty-logo1.png>-->
        </div>

        <div class="coverHeadQuote">
          <div class="titleTextTablet">
            <h1 class="pageTitleTablet" style="font-weight:400;">Hey, I am Delia Hallberg</h1>
            <h2 class="pageSubTitleTablet">Consultant // Researcher // Social Scientist // Tech Enthusiast</h2>
          </div>
        </div>

      </div>

    </div>
  </section>
</template>

<script>

export default {
  data() {
    return {

    }
  }
}

</script>

<style>
@import url('https://fonts.googleapis.com/css?family=Kalam&display=swap');


.coverHeadDesktop {
  max-width: 100%;
  min-height: 100vh;
  -webkit-background-size: cover;
  -moz-background-size: cover;
  -o-background-size: cover;
  background-size: cover;
  background-position: right top;
}
.coverHeadTablet {
  display: none;
}
.coverHeadQuote {
  display: none;
}

.titleTextDesktop {
  width: 50%;
  text-align: center;
  margin-left: 5%;
  margin-right: 5%;
  padding-top: 17.5%;
}
.pageTitleDesktop {
  font-size: 40px;
}
.pageSubTitleDesktop {
  font-size: 15px;
}
.titleQuoteDesktop {
  font-size: 20px;
  padding-left: 15%;
  padding-right: 15%;
  padding-top: 2em;
  font-family: 'Kalam';
}

@media screen and (min-width: 1600px) {

}
@media screen and (max-width: 950px) {
  .coverHeadDesktop {
    display: none;
  }
  .coverHeadTablet {
    display: block;
    max-width: 100%;
    min-height: 75vh;
    -webkit-background-size: cover;
    -moz-background-size: cover;
    -o-background-size: cover;
    background-size: auto 120%;
    background-repeat: no-repeat;
    background-position: center center;
  }
  .coverHeadQuote {
    display: block;
    min-height: 25vh;
  }

  .titleTextTablet {
    width: 100%;
    text-align: center;
    padding-top: 4em;
  }
  .pageTitleTablet {
    font-size: 50px;
  }
  .pageSubTitleTablet {
    padding-top: 0em;
    font-size: 25px;
    margin: 0;
  }
}

@media screen and (max-width: 750px) {
  .coverHeadDesktop {
    display: none;
  }
  .titleTextTablet {
    width: 100%;
    text-align: center;
    padding-top: 4em;
  }
  .pageTitleTablet {
    font-size: 40px;
  }
  .pageSubTitleTablet {
    padding-top: 0em;
    font-size: 20px;
    margin: 0;
  }

}

@media screen and (max-width: 600px) {
  .coverHeadDesktop {
    display: none;
  }
  .titleTextTablet {
    width: 100%;
    text-align: center;
    padding-top: 4em;
  }
  .pageTitleTablet {
    font-size: 35px;
  }
  .pageSubTitleTablet {
    padding-top: 0em;
    font-size: 15px;
    margin: 0;
  }
}

@media screen and (max-width: 450px) {
  .coverHeadDesktop {
    display: none;
  }
  .titleTextTablet {
    width: 100%;
    text-align: center;
    padding-top: 4em;
  }
  .pageTitleTablet {
    font-size: 25px;
  }
  .pageSubTitleTablet {
    padding-top: 0em;
    font-size: 12px;
    margin: 0;
  }
}



/* If height very low */
@media screen and (max-height: 600px) {
  .coverHeadTablet {
    display: block;
    max-width: 100%;
    min-height: 75vh;
    -webkit-background-size: cover;
    -moz-background-size: cover;
    -o-background-size: cover;
    background-size: auto 120%;
    background-repeat: no-repeat;
    background-position: center center;
  }
}
</style>
