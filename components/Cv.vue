<template>
  <section>

        <div class="cv">
          <img class="cvImage" src="~/assets/pictures/delia_cv.png">
        </div>

        <section class="cv-mobile">
          <div class="timeline">
            <div class="container left">
              <div class="content">
                <h2><b>2009</b></h2>
                <p>
                  <b>German Abitur</b>
                </p>
              </div>
            </div>
            <div class="container right">
              <div class="content">
                <h2><b>2011-12</b></h2>
                <p>
                  <b>D-Team University of Twente</b>
                  strategic marketing for student acquisition
                </p>
              </div>
            </div>

            <div class="container left">
              <div class="content">
                <h2><b>2013</b></h2>
                <p>
                  <b>Bachelor of Science in European Studies</b>
                  <b>University of Twente</b>, multidisciplinary study of economics, political science, law and sociology
                </p>
              </div>
            </div>
            <div class="container right">
              <div class="content">
                <h2><b>2014</b></h2>
                <p>
                  <b>Heinrich-Böll-Foundation Prague</b>
                  policy analysis, conceptualization and organization of workshops and seminars on sustainability, renewable energy, gender democracy
                </p>
              </div>
            </div>

            <div class="container left">
              <div class="content">
                <h2><b>2016-17</b></h2>
                <p>
                  <b>Startup Incubator "Gründerservice" Humboldt University Berlin</b>
                  daily operations of startup houses, startup support, workshop assistance
                </p>
              </div>
            </div>
            <div class="container right">
              <div class="content">
                <h2><b>2017-18</b></h2>
                <p>
                  <b>Pool of Stake AG</b>
                  ICO whitepaper, blockchain governance research, product development, content management
                </p>
              </div>
            </div>

            <div class="container left">
              <div class="content">
                <h2><b>2019</b></h2>
                <p>
                  <b>Master of Arts in Sociology</b>
                  <b>Free University Berlin</b>
                </p>
              </div>
            </div>

          </div>
        </section>

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
  display: block;
  max-width: 100%;
}
.cv-mobile {
  display: none;
}

@media screen and (max-width: 1000px) {
  .cv-mobile {
    display: block;
  }
  .cv {
    display: none;
  }
}


/* The actual timeline (the vertical ruler) */
.timeline {
  background-color: #f5f0ec;
  position: relative;
  max-width: 1200px;
  margin: 0 auto;
}

/* The actual timeline (the vertical ruler) */
.timeline::after {
  content: '';
  position: absolute;
  width: 6px;
  background-color: white;
  top: 0;
  bottom: 0;
  left: 50%;
  margin-left: -3px;
}

/* Container around content */
.container {
  padding: 10px 40px;
  position: relative;
  background-color: inherit;
  width: 50%;
}

/* The circles on the timeline */
.container::after {
  content: '';
  position: absolute;
  width: 25px;
  height: 25px;
  right: -17px;
  background-color: white;
  border: 4px solid #e5de5b;
  top: 15px;
  border-radius: 50%;
  z-index: 1;
}

/* Place the container to the left */
.left {
  left: 0;
}

/* Place the container to the right */
.right {
  left: 50%;
}

/* Add arrows to the left container (pointing right) */
.left::before {
  content: " ";
  height: 0;
  position: absolute;
  top: 22px;
  width: 0;
  z-index: 1;
  right: 30px;
  border: medium solid white;
  border-width: 10px 0 10px 10px;
  border-color: transparent transparent transparent white;
}

/* Add arrows to the right container (pointing left) */
.right::before {
  content: " ";
  height: 0;
  position: absolute;
  top: 22px;
  width: 0;
  z-index: 1;
  left: 30px;
  border: medium solid white;
  border-width: 10px 10px 10px 0;
  border-color: transparent white transparent transparent;
}

/* Fix the circle for containers on the right side */
.right::after {
  left: -16px;
}

/* The actual content */
.content {
  padding: 20px 30px;
  background-color: white;
  position: relative;
  border-radius: 6px;
}

/* Media queries - Responsive timeline on screens less than 600px wide */
@media screen and (max-width: 600px) {
/* Place the timelime to the left */
  .timeline::after {
    left: 31px;
  }

/* Full-width containers */
  .container {
    width: 100%;
    padding-left: 70px;
    padding-right: 25px;
  }

/* Make sure that all arrows are pointing leftwards */
  .container::before {
    left: 60px;
    border: medium solid white;
    border-width: 10px 10px 10px 0;
    border-color: transparent white transparent transparent;
  }

/* Make sure all circles are at the same spot */
  .left::after, .right::after {
    left: 15px;
  }

/* Make all right containers behave like the left ones */
  .right {
    left: 0%;
  }
}

</style>
