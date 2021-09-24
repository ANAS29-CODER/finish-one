<template>
  <div class="main">
    <div class="mainin container">
      <h3>{{ $t("serv.h") }}</h3>
      <p v-html="$t('serv.hp')"></p>

      <div class="row">
        <div class="col-sm-6 col-md-4">
          <fa icon="user-tie" />
          <h6>{{ $t("serv.h1") }}</h6>
          <p>{{ $t("serv.p1") }}</p>
        </div>
        <div class="col-sm-6 col-md-4">
          <fa icon="user-tie" />
          <h6>{{ $t("serv.h2") }}</h6>
          <p>{{ $t("serv.p1") }}</p>
        </div>
        <div class="col-sm-6 col-md-4">
          <fa icon="user-tie" />
          <h6>{{ $t("serv.h3") }}</h6>
          <p>{{ $t("serv.p1") }}</p>
        </div>
        <div class="col-sm-6 col-md-4">
          <fa icon="user-tie" />
          <h6>{{ $t("serv.h4") }}</h6>
          <p>{{ $t("serv.p1") }}</p>
        </div>
        <div class="col-sm-6 col-md-4">
          <fa icon="user-tie" />
          <h6>{{ $t("serv.h5") }}</h6>
          <p>{{ $t("serv.p1") }}</p>
        </div>
        <div class="col-sm-6 col-md-4">
          <fa icon="user-tie" />
          <h6>{{ $t("serv.h6") }}</h6>
          <p>{{ $t("serv.p1") }}</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Services",
};
</script>

<style scoped>
.main {
  padding: 60px 0;
  background-color: #fde1e5;
}
.mainin {
  background-color: white;
  border-radius: 38px;
}
.mainin h3 {
  padding-top: 20px;
  color: black;
  font-weight: bold;
}

.mainin p {
  color: #9e9e9e;
  font-weight: bolder;
  font-size: 13px;
  padding-top: 7px;
}

.mainin p span {
  color: #f44d61;
}
.mainin h6 {
  font-size: 1.25rem;
  font-weight: bold;
  color: black;
  padding-top: 11px;
}
.mainin svg:not(:root).svg-inline--fa {
  font-size: 39px;
  background-color: #ff335a;
  padding: 5px;
  color: white;
  border-radius: 5px;
}
.mainin .row div {
  text-align: center;
  padding: 20px 0px;
  background-color: #f7f5f5;
  margin: 5px auto;
  border-radius: 30px;
  border-right: solid white 2px;
  border-left: solid white 2px;
}
</style>
