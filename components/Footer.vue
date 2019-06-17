<template>
  <section>
    <div class="wrapperCover">

      <div class="coverFooter" :style="{ backgroundImage: 'url(' + require(`@/assets/pictures/DeliHireMe.jpg`) + ')' }">
        <!--<img class="djListe" src="~/assets/DJ_Liste_st.png">-->
        <a-button type="primary" size="large" class="hireButton" @click="showDrawer"><span class="hireButtonText">Hire me!</span></a-button>
        <a-drawer
          title="Contact"
          placement="bottom"
          :closable="false"
          @close="onClose"
          :visible="visible"
        >
          <div class="contactDetails">
            <p class="contactFlexElement" style="text-align:center;font-size:30px;">mail@delia-hallberg.de</p>
            <a-icon type="linkedin" class="contactFlexElement" style="font-size:70px;" @click="openWebsiteNewTab('https://www.linkedin.com/in/delia-hallberg/')"/>
          </div>
        </a-drawer>
      </div>

    </div>
  </section>
</template>

<script>

export default {
  data() {
    return {
      visible: false
    }
  },
  methods: {
    showDrawer() {
      this.visible = true
    },
    onClose() {
      this.visible = false
    },
    onChange(e) {
      this.placement = e.target.value
    },
    openWebsiteNewTab(link) {
      window.open(link, "_blank");
    }
  },
}

</script>

<style>
.ant-drawer-header {
  background-color: #f5f0ec;
}
.ant-drawer-content {
  background-color: #f5f0ec;
}
.ant-drawer-title {
  text-align: center;
}
.contactDetails {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  display: flex;
  justify-content: space-around; /* align horizontal */
  align-items: center; /* align vertical */
}
.contactFlexElement {
  width: 100%;
}
.hireButton {
  background-color: #e5de5b;
  float: right;
  padding-top: 1em;
  padding-bottom: 5.5em;
  padding-left: 3em;
  padding-right: 3em;
  margin-top: 20%;
  margin-right: 20%;
  border-radius: 20px;
  border-color: lightgrey;
}
.hireButton:hover {
  background-color: #e5de5b;
  border-color: lightgrey;
}
.hireButton:focus {
  background-color: #e5de5b;
  border-color: lightgrey;
}
.hireButton:hover:focus {
  background-color: #e5de5b;
  border-color: lightgrey;
}
.hireButtonText {
  font-size: 50px;
  color: #1a234d;
}
.coverFooter {
  max-width: 100%;
  min-height: 100vh;
  -webkit-background-size: cover;
  -moz-background-size: cover;
  -o-background-size: cover;
  background-size: cover;
  background-position: center top;
}

@media screen and (min-width: 1600px) {

}
@media screen and (max-width: 950px) {

}
/* If height very low */
@media screen and (max-height: 500px) {
  
}
</style>
