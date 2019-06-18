<template>
  <section class="pageWrapper">

    <h1 style="font-weight:400;font-size:3em;text-align:center;padding-top:1em;">Research</h1>
    <section class="info">

      <div class="research-element">
        <h3 style="text-align:center;">Bachelor Thesis 2013</h3>
        <p style="text-align:center;">find publication here</p>
        <img id="previewResearchPaper"
        src="~/assets/pictures/PreviewGB.png"
        @click="openWebsiteNewTab('https://books.google.de/books?id=ZMtpDAAAQBAJ&lpg=PA85&dq=delia%20hallberg%20bulgarian&hl=de&pg=PA85#v=onepage&q&f=false')">
      </div>

      <div class="research-element">
        <h3 style="text-align:center;">Whitepaper 2018</h3>
        <p style="text-align:center;">Proof of Stake Blockchain Pool</p>
        <img id="previewResearchPaper"
        src="~/assets/pictures/PreviewPSKwhitepaper.png"
        @click="openWebsiteNewTab('https://www.poolofstake.io/wp-content/uploads/2018/09/Pool_of_Stake_whitepaper.pdf')">
      </div>

      <div class="research-element">
        <h3 style="text-align:center;">Master Thesis 2019</h3>
        <p style="text-align:center;">A technoliberal myth</p>
        <img id="previewResearchPaper"
        src="~/assets/pictures/PreviewMA.png"
        @click="openWebsiteNewTab('http://researchpaper.delia-hallberg.de')">
      </div>

    </section>

  </section>
</template>

<script>
export default {
  methods: {
    openWebsiteNewTab(link) {
      window.open(link, "_blank");
    }
  }
}


</script>

<style>
#previewResearchPaper {
  border-radius: 15px;
  height: 25em;
  margin: 1em;
  cursor: pointer;
}
p {
  white-space: pre-line;
}
.pageWrapper {
  padding-bottom: 2em;
  margin: 0;
}
.info {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  display: flex;
  justify-content: space-around; /* align horizontal */
  align-items: center; /* align vertical */
  padding-top: 2em;
}
.research-element {
  background-color: #f5f0ec;
  border-top-left-radius: 50px;
  border-top-right-radius: 50px;
  border-bottom-left-radius: 25px;
  border-bottom-right-radius: 25px;
  border-top: solid #e5de5b 7.5px;
  border-bottom: solid #e5de5b 7.5px;
  padding: 2em;
  margin: 0.5em;
  min-width: 20em;
  -webkit-box-shadow: 3px -1px 10px 0px rgba(0,0,0,0.18);
  -moz-box-shadow: 3px -1px 10px 0px rgba(0,0,0,0.18);
  box-shadow: 3px -1px 10px 0px rgba(0,0,0,0.18);
}
</style>
