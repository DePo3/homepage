<template>
  <section class="pageWrapper">

    <h1 style="font-weight:400;text-align:center;">Research</h1>
    <div class="info">
      <img id="previewResearchPaper" src="~/assets/pictures/PreviewMA.png" @click="openWebsiteNewTab('http://researchpaper.delia-hallberg.de')">
      <img id="previewResearchPaper" src="~/assets/pictures/PreviewPSKwhitepaper.png" @click="openWebsiteNewTab('https://www.poolofstake.io/wp-content/uploads/2018/09/Pool_of_Stake_whitepaper.pdf')">
      <img id="previewResearchPaper" src="~/assets/pictures/PreviewGB.png" @click="openWebsiteNewTab('https://books.google.de/books?id=ZMtpDAAAQBAJ&lpg=PA85&dq=delia%20hallberg%20bulgarian&hl=de&pg=PA85#v=onepage&q&f=false')">

    </div>

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
  height: 40em;
  margin: 1em;
  cursor: pointer;
}
p {
  white-space: pre-line;
}

.info {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  display: flex;
  justify-content: center; /* align horizontal */
  align-items: center; /* align vertical */
  padding-top: 2em;
}
</style>
