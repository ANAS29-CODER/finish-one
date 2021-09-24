<template>
  <div class="mainm">
    <div class="container">
      <h3 style="color: black; padding-bottom: 20px; font-weight: bold">
        Our specialists
      </h3>
      <div class="row">
        <div class="col-sm-6 col-md-3 card" v-for="pos in poss" :key="pos.id">
          <img
            class="card-img-top"
            :src="pos.url"
            alt="Card image"
            style="width: 100%"
          />
          <div class="card-body">
            <h4 class="card-title">{{ pos.name }}</h4>
            <p class="card-text text-muted">
              {{ pos.job }}
            </p>
            <p class="card-text text-danger .font-weight-light">
              {{ pos.exp }}
            </p>
            <a href="#" class="btn btn-danger stretched-link">See Profile</a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import ims from "@/components/ims.json";

export default {
  name: "Team",
  data() {
    return {
      poss: ims,
    };
  },
};
</script>

<style scoped>
.mainm {
  background-color: #fde1e5;
}
.mainm .row div {
  padding: 20px 0px;
}
.mainm .container {
  margin: 30px auto;
  padding: 50px;
}
.mainm .card-img-top {
  margin: auto;
  max-width: 88px;
  max-height: 80px;
  border: 3px solid var(--openred);
  border-radius: 50%;
}
.mainm .card {
  border: none;
  border-radius: 50px;
  background-color: #fff;
  border-left: solid 3px #fde1e5;
  border-right: solid 3px #fde1e5;
  margin-bottom: 10px;
}
.mainm .card p {
  font-weight: bold;
}
.mainm .card:hover {
  background-color: #e9cbcb;
}
.mainm .row div:last-child {
  text-align: center;
}
</style>
