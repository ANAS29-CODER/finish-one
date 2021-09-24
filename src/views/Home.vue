<template>
  <div class="mainho">
    <div class="home">
      <div class="main">
        <div class="container ssa">
          <div class="row">
            <div class="m1 col-md-6">
              <h6>{{ $t("header.head") }}</h6>
              <h1>
                {{ $t("header.h1") }}
              </h1>

              <p class="text-muted">
                {{ $t("header.p") }}
              </p>
            </div>

            <div class="m2 col-md-6">
              <img src="@/views/download.jpg" class="img-fluied" />
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="serch container w-75">
      <div class="fas row" id="sad">
        <div class="s1 dd col-md-3">
          <h6>
            <fa icon="user" class="mr-3" style="color: red" />
            {{ $t("header.s1h") }}
          </h6>
          <p class="text-muted">{{ $t("header.s1p") }}</p>
        </div>

        <div class="s2 dd col-md-3">
          <h6>
            <fa icon="map-marker-alt" class="mr-3" style="color: red" />{{
              $t("header.s2h")
            }}
          </h6>
          <p class="text-muted">{{ $t("header.s2p") }}</p>
        </div>

        <div class="s3 dd col-md-3">
          <h6>
            <fa icon="clock" class="mr-3" style="color: red" />{{
              $t("header.s3h")
            }}
          </h6>
          <p class="text-muted">{{ $t("header.s3p") }}</p>
        </div>
        <div class="s4 dd col-md-3">
          <i
            class="material-icons"
            style="font-size: 48px; color: red; cursor: pointer"
            >find_replace</i
          >
        </div>
      </div>
    </div>
    <!-- *********************************************-->

    <div class="sec2 container">
      <h1 style="text-align: center; font-weight: bold; color: black">
        {{ $t("header.sec2h") }}
      </h1>
      <div class="row">
        <div class="rr col-md-4">
          <fa icon="medal" style="color: red; font-size: 80px" />
          <h4>{{ $t("header.rrh") }}</h4>
          <p class="text-muted">
            {{ $t("header.rrp") }}
          </p>
        </div>

        <div class="rr rs col-md-4">
          <fa icon="tree" style="color: red; font-size: 80px" />
          <h4>{{ $t("header.rsh") }}</h4>
          <p class="text-muted">
            {{ $t("header.rsp") }}
          </p>
        </div>

        <div class="rr rt col-md-4">
          <fa icon="medal" style="color: red; font-size: 80px" />
          <h4>{{ $t("header.rth") }}</h4>
          <p class="text-muted">
            {{ $t("header.rth") }}
          </p>
        </div>
      </div>
    </div>
    <!-- *********************************************-->
    <div class="sec3 container">
      <h1>{{ $t("header.sec3h") }}</h1>
      <div class="nmmn row">
        <api
          v-for="per in pers"
          v-bind:key="per.id"
          :url="per.url"
          :name="per.name"
          :stars="per.stars"
          :media="per.media"
          :icon="per.icon"
        />
      </div>
    </div>
    <!-- *********************************************-->
    <div class="sec4 container">
      <h2 style="text-align: center; color: black; font-weight: bold">
        {{ $t("header.sec4h") }}
      </h2>

      <div class="sec41">
        <div class="row">
          <div class="fg col-sm-6">
            <h5>{{ $t("header.sec41h") }}</h5>
            <p>{{ $t("header.sec41p") }}</p>
            <input
              class="lk"
              type="text"
              :placeholder="$t('header.sec4i')"
              @click="bor()"
            />
            <p>{{ $t("header.sec4p2") }}</p>
            <input
              class="lk"
              type="text"
              placeholder="059-297-0150"
              @click="bor()"
            />
            <br />
            <button class="btn">{{ $t("header.sec4i2") }}</button>
            <p class="cv">{{ $t("header.sec41p2") }}</p>
          </div>

          <div class="col-sm-6">
            <img
              src="https://angular-project-ssr.herokuapp.com/assets/images/map.png"
              class="img-fluied"
            />
          </div>
        </div>
      </div>
    </div>
    <hr class="jh" />
  </div>
</template>

<script>
import api from "@/components/api.vue";
import im from "@/components/im.json";

export default {
  name: "Home",
  data() {
    return {
      pers: im,
    };
  },

  components: {
    api,
  },
};
</script>

<style scoped src="@/assets/css/ho.css"></style>
