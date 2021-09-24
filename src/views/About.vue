<template>
  <div class="abou main">
    <div class="about container">
      <div class="row">
        <div class="sec1 col-sm-6">
          <img
            src="https://angular-project-ssr.herokuapp.com/assets/images/img2.png"
            class="ss img-fluid"
          />
          <img
            src="https://angular-project-ssr.herokuapp.com/assets/images/img3.png"
            class="img-fluid"
          />

          <img
            src="https://angular-project-ssr.herokuapp.com/assets/images/img4.png"
            class="img-fluid"
          />
          <img
            src="https://angular-project-ssr.herokuapp.com/assets/images/img5.png"
            class="ss img-fluid"
          />
        </div>

        <div class="sec2 col-sm-6" style="word-break: break-word">
          <h3>{{ $t("about.head") }}</h3>
          <br />
          <p v-html="$t('about.idea')" />
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.abou .row {
  padding: 30px 0;
  width: inherit;
}
.abou {
  padding: 60px 0;
  background-color: #fde1e5;
}
.about {
  background-color: #fff;
  margin: 50px auto;
  border-radius: 50px;
}
.about .sec2 span {
  color: red !important;
}
.abou img[data-v-039c5b43] {
  border-radius: 10px;
  margin-right: 17px;
  margin-top: 5px;
  max-width: 42%;
}
.abou .ss .img-fluid {
  max-width: 70%;
  max-height: 50%;
}
@media only screen and (max-width: 767px) and (min-width: 576px) {
  .abou img[data-v-039c5b43][data-v-039c5b43] {
    border-radius: 10px;
    margin-right: 9px;
    margin-top: 32px;
    max-width: 45%;
  }
}

@media only screen and (max-width: 430px) {
  .abou .ss .img-fluid {
    width: 50%;
  }
}
@media only screen and (max-width: 402px) {
}
.abou .sec2 {
  margin: auto;
}
.abou .sec2 h3 {
  color: black;
  font-weight: bolder;
  text-align: start;
  padding-top: 10px;
}
.abou .sec2 p {
  color: black;
  font-weight: bold;
  text-align: start;
}
.abou .sec2 p span {
  color: red;
}

@media only screen and(max-width:575px) {
  .abou .sec2 {
    order: 1;
  }
  .abou .sec1 {
    order: 2;
  }
}
@media only screen and (max-width: 257px) {
  .abou .sec2 p[data-v-039c5b43] {
    font-size: small;
  }
  .abou img[data-v-039c5b43][data-v-039c5b43] {
    border-radius: 10px;
    margin-right: 17px;
    margin-top: 5px;
    max-width: 34%;
  }
}
</style>
