<template>
  <div class="hea">
    <div class="container cell suo" id="spe">
      <span> <fa icon="phone-alt" />(+972)592970150</span>
      <span class="assa" id="demo"
        ><fa icon="envelope" style="" />anasouda43@gmail.com
      </span>

      <div class="aa">
        <a
          href="https://www.facebook.com/anas.adel.94/?viewas=show_switched_toast=falseshow_switched_tooltip=falseshow_podcast_settings=false"
          ><i class="fa fa-facebook" style="font-size: 20px"></i
        ></a>
        <a href="https://www.instagram.com/accounts/login/"
          ><i class="fa fa-instagram" style="font-size: 20px"></i
        ></a>
        <a
          href="https://twitter.com/Twitter?ref_src=twsrc%5Egoogle%7Ctwcamp%5Eserp%7Ctwgr%5Eauthor"
          ><i class="fa fa-twitter" style="font-size: 20px"></i
        ></a>
      </div>
      <hr />
    </div>

    <nav class="navbar navbar-expand-lg navbar-light">
      <div class="container">
        <a class="navbar-brand" href="/"
          ><fa icon="tty" />{{ $t("footer.d1a") }}</a
        >
        <button
          class="navbar-toggler"
          id="nas"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#navbarTogglerDemo02"
          aria-controls="navbarTogglerDemo02"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse sas" id="navbarTogglerDemo02">
          <ul class="navbar-nav me-auto mb-2 mb-lg-0 mx-auto">
            <router-link
              :to="`/${$i18n.locale}/`"
              tag="li"
              class="nav-item"
              exact
              ><a class="nav-link" @click="link">{{
                $t("footer.d2ua1")
              }}</a></router-link
            >

            <router-link
              :to="`/${$i18n.locale}/about`"
              class="nav-item"
              tag="li"
              exact
              ><a class="nav-link" @click="link">{{
                $t("footer.d2ua2")
              }}</a></router-link
            >

            <router-link
              :to="`/${$i18n.locale}/services`"
              class="nav-item"
              tag="li"
              exact
              ><a class="nav-link" @click="link">{{
                $t("footer.d2ua3")
              }}</a></router-link
            >

            <router-link
              :to="`/${$i18n.locale}/team`"
              class="nav-item"
              tag="li"
              exact
            >
              <a class="nav-link" @click="link">{{
                $t("footer.d2ua4")
              }}</a></router-link
            >

            <router-link
              :to="`/${$i18n.locale}/contact`"
              class="nav-item"
              tag="li"
              exact
              ><a class="nav-link" @click="link">{{
                $t("footer.d2ua5")
              }}</a></router-link
            >
          </ul>
          <div class="bt d-flex">
            <button id="ar1" class="btn mr-4" @click.prevent="setLocale('ar')">
              Ar
            </button>
            <button id="er1" class="btn mr-2" @click.prevent="setLocale('en')">
              En
            </button>
            <ul class="navbar-nav d-flex">
              <router-link to="/" class="nav-item sasa" tag="li"
                ><a class="nav-link" style="color: rgb(255 13 82)">
                  {{ $t("footer.prof") }} <fa icon="user" /></a
              ></router-link>
            </ul>
          </div>
        </div>
      </div>
    </nav>
  </div>
</template>

<script>
export default {
  name: "Header",
  data() {
    return { langs: ["en", "ar"] };
  },
  methods: {
    link() {
      return document.getElementById("nas").click();
    },
    setLocale(locale) {
      this.$i18n.locale = locale;
      this.$router.push("/").catch(() => {});
      if (locale === "en") {
        document.body.style.direction = "ltr";
        return document.getElementById("nas").click();
      } else {
        document.body.style.direction = "rtl";

        document.getElementById("spe").style.direction = "ltr";

        return document.getElementById("nas").click();
      }
    },
  },
};
</script>
<style scoped src="@/assets/css/ma.css"></style>
