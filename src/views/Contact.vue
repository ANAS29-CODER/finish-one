<template>
  <div class="mains">
    <div class="container">
      <div class="row">
        <div class="col-sm-6">
          <form>
            <input type="text" :placeholder="$t('cont.b1')" required /><br />
            <input type="email" :placeholder="$t('cont.b2')" required /><br />
            <textarea
              id="w3review"
              name="Message"
              rows="6"
              cols="6"
              :placeholder="$t('cont.bm')"
              style="width: 200px"
              required
            ></textarea
            ><br />
            <button class="btn" type="submite">{{ $t("cont.b3") }}</button>
          </form>
        </div>
        <div class="col-sm-6">
          <img
            src="https://angular-project-ssr.herokuapp.com/assets/images/contact.png"
            class="img-fluid"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Contact",
};
</script>
<style scopde>
.mains {
  padding: 50px 0px;
  background-color: #8275f0;
  width: 100%;
}
.mains .img-fluid {
  max-width: 100%;
  height: auto;
}

.mains button {
  width: 273px;
  color: white;
  background-color: #483ac0;
  border-radius: 20px;
}
.mains input {
  padding: 10px;
  border-radius: 20px;
  width: 273px;
  border: none;
  margin-bottom: 10px;
  background-color: #d6cfcf;
}
.mains textarea {
  width: 273px !important;
  border-radius: 20px;
  border: none;
  padding: 5px;
  background-color: #d6cfcf;
}
.mains input:focus,
.mains textarea:focus {
  outline: none;
}
.mains button {
  width: 273px;
  color: white;
  background-color: #483ac0;
  border-radius: 20px;
}
.mains .row {
  margin: 40px 0px;
  background-color: white;
  border-radius: 40px;
}
.mains .row div {
  padding: 50px;
}
.mains .row div:last-child {
  text-align: start;
}
.mains .row div:first-child {
  text-align: end;
}
@media screen and (min-width: 768px) and (max-width: 991px) {
  .mains .row img {
    height: 283px;
  }
}
@media screen and (min-width: 576px) and (max-width: 767px) {
  .mains .row img {
    height: 270px;
  }
  .mains form {
    margin-left: -35px;
  }
  .mains input,
  .mains textarea,
  .mains button {
    width: 222px !important;
  }
}
@media only screen and (max-width: 575px) {
  .mains form {
    text-align: center;
  }
}
@media only screen and (max-width: 380px) {
  .mains input,
  .mains textarea,
  .mains button {
    width: 210px !important;
  }
}
@media only screen and (max-width: 315px) {
  .mains input,
  .mains textarea,
  .mains button {
    width: 160px !important;
  }
  .mains .row img {
    height: 216px;
  }
}
@media only screen and (max-width: 260px) {
  .mains input,
  .mains textarea,
  .mains button {
    width: 120px !important;
  }
  .mains .row img {
    height: 190px;
  }
}
</style>
