<template>
  <div class="eec">
    <div class="eem row">
      <div class="eein col-md-4">
        <img :src="url" class="img-fluied" />
      </div>

      <div class="eein col-md-4">
        <h6>{{ name }}</h6>
        <ul>
          <li v-for="star in stars" :key="star.id"><fa icon="star" /></li>
        </ul>

        <p style="font-weight: bold">
          <fa :icon="['fab', 'facebook-f']" class="mr-2" style="color: red" />
          {{ media }}
        </p>
      </div>
      <div class="eein dat col-md-4">
        <p class="text-muted">9 March 2020</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: ["url", "name", "stars", "media", "icon"],
  name: "api",
};
</script>

<style scoped>
.eec {
  background-color: #fcfcfc;
  padding: 10px 10px;
  max-width: 47%;
  margin-right: 26px;
  margin-bottom: 20px;
}
.eec:hover {
  border: solid rgb(187, 185, 183) 5px;

  transition: 0.5s border;
}

.mainone {
  width: 100%;
}
.sec3 .eem .eein {
  text-align: start;
}
.sec3 .eem .eein img {
  border-radius: 50% 60%;
  display: inline-block;
  width: fit-content;
  max-width: 80%;
  max-height: 60%;
  border-radius: 50%;
}
.dat {
  text-align: center;
  margin: 0% auto;
}
.sec3 .eem .eein h6 {
  color: rgb(27, 17, 17);
  font-weight: bold;
  width: max-content;
}
.sec3 .eem .eein ul {
  padding-left: unset;
}
.sec3 .eem .eein ul li {
  list-style: none;
  display: inline;
  margin-left: 2px;
  color: rgb(255, 0, 0);
  width: max-content;
}
@media only screen and (max-width: 991px) {
  .nmmn {
    width: 112%;
  }
  .eec {
    margin: 20px 0% !important;
  }
  .eec {
    width: 100%;
  }
  .eein svg.mr-2.svg-inline--fa.fa-facebook-f.fa-w-10 {
    margin: 0% !important;
  }
}

@media only screen and (max-width: 400px) {
  .eein {
    margin-left: 1px !important;
    float: left;
    width: 100%;
  }
  .eec {
    width: 100%;
  }
  .sec3 .eem .eein img[data-v-6ba76b3a] {
    max-width: 100%;
  }
  .sec3 .eem .eein h6 {
    margin: 0% auto;
    font-size: 14px;
    text-align: center !important;
  }
  .eec[data-v-6ba76b3a] {
    max-width: 60%;
  }
  .sec3 .eem .eein {
    text-align: center;
  }
}
</style>
