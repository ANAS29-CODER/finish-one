<template>
  <div class="sec5 footer container">
    <div class="cd row">
      <div class="col-6 col-md-3">
        <a class="navbar-brand" :href="`/${$i18n.locale}`"
          ><fa icon="tty" />{{ $t("footer.d1a") }}</a
        >
        <p class="text-muted">(+972)592970150</p>
        <p class="text-muted">anasouda43@gmail.com</p>
        <p class="text-muted">(+972)592970150</p>

        <div class="aa">
          <a
            href="https://www.facebook.com/anas.adel.94/?viewas=&show_switched_toast=false&show_switched_tooltip=false&show_podcast_settings=false"
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
      </div>

      <div class="fs col-6 col-md-3">
        <h6>{{ $t("footer.d2h") }}</h6>
        <ul style="list-style: none">
          <router-link :to="`/${$i18n.locale}`" tag="li" class="nav-item" exact
            ><a class="nav-link">{{ $t("footer.d2ua1") }}</a></router-link
          >

          <router-link
            :to="`/${$i18n.locale}/about`"
            class="nav-item"
            tag="li"
            exact
            ><a class="nav-link">{{ $t("footer.d2ua2") }}</a></router-link
          >

          <router-link
            :to="`/${$i18n.locale}/services`"
            class="nav-item"
            tag="li"
            exact
            ><a class="nav-link">{{ $t("footer.d2ua3") }}</a></router-link
          >

          <router-link
            :to="`/${$i18n.locale}/team`"
            class="nav-item"
            tag="li"
            exact
          >
            <a class="nav-link">{{ $t("footer.d2ua4") }}</a></router-link
          >

          <router-link
            :to="`/${$i18n.locale}/contact`"
            class="nav-item"
            tag="li"
            exact
            ><a class="nav-link">{{ $t("footer.d2ua5") }}</a></router-link
          >
        </ul>
      </div>
      <div class="col-6 col-md-3">
        <h6>{{ $t("footer.d3h") }}</h6>
        <p class="text-muted">{{ $t("footer.d3p1") }}</p>
        <p class="text-muted">{{ $t("footer.d3p2") }}</p>
        <p class="text-muted">{{ $t("footer.d3p3") }}</p>
      </div>
      <div class="col-6 col-md-3">
        <h6 style="color: rgb(255 13 82)">{{ $t("footer.d4h") }}</h6>
        <p class="cer text-muted">
          {{ $t("footer.d4p1") }}
        </p>
        <p class="text-muted">{{ $t("footer.d4p2") }}</p>
        <input type="text" placeholder="a@gmail.com" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "foo",
};
</script>
<style scoped src="@/assets/css/footer.css"></style>
