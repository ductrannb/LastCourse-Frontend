<template>
  <div class="container">
    <Alert />
    <loading :is_loading="loading"></loading>
    <v-row class="content">
      <v-col class="banner" cols="7">
        <div class="banner-img">
          <v-img src="/src/assets/banner.svg"></v-img>
        </div>

        <div class="slogan">
          <p class="h1-text">Sản phẩm chất lượng</p>
          <p>
            Tất cả các sản phẩm trên M Clothing đều dược đăng bán bởi các nhà cung cấp, uy
            tín và đảm bảo chât lượng
          </p>
        </div>
      </v-col>

      <v-col cols="5">
        <div class="right-content">
          <div class="logo">
            <v-img src="/src/assets/logo.svg" />
          </div>
          <main>
            <router-view></router-view>
          </main>
        </div>
      </v-col>
    </v-row>
  </div>
</template>

<script>
import Loading from "../components/Loading.vue";

export default {
  name: "AccountLayout",
  components: { Loading },
};
</script>

<style>
.v-form {
  padding: 5px;
}
.container {
  max-width: 1175px;
}

.center-row .content {
  display: flex;
  height: 100vh;
  justify-content: center;
  align-items: center;
}

.h1-text {
  font-weight: 700;
  color: red;
}

.banner {
  width: 100%;
}

.banner-img {
  width: 80%;
  margin: 0 10%;
  height: auto;
}

.slogan {
  padding: 0 6rem;
  text-align: center;
}

.right-content {
  display: flex;
  justify-content: center;
  flex-direction: column;
  align-items: center;
}

.logo {
  width: 40%;
  height: auto;
}

.form-content {
  text-align: center;
}

.form-heading-title {
  font-weight: 600;
  font-size: 1.5rem;
}

.form-heading-subtitle {
  margin: 1rem 0 2rem;
}

.form-check-box {
  font-size: 14px;
}

.another-action {
  font-weight: 600;
  color: #ee273c;
  text-decoration: none;
}

.base-button {
  color: #ffffff !important;
  width: 278px !important;
  height: 44px !important;
  padding: 11px 21px !important;
  border-radius: 100px !important;
  text-transform: none !important;
  margin-top: 3rem;
}

.hide-logo .right-content .logo {
  display: none;
}

.bottom-content {
  margin-top: 1.5rem;
}

/*Custom vuetify*/

.my-input .v-field__field {
  width: 381px;
  height: 44px;
}

.my-input .v-field__input {
  min-height: unset !important;
  height: 100%;
  padding: 10px 24px;
}

.my-input .v-field--appended {
  display: flex;
  align-items: center;
}

.my-input .v-field__append-inner {
  padding: 0;
}

.my-input .v-label.v-field-label {
  font-weight: 400;
  font-size: 14px;
  line-height: 14px;
}

.my-input .v-field__outline__start {
  padding-right: 24px !important;
  border-top-left-radius: 100px !important;
  border-bottom-left-radius: 100px !important;
}

.my-input .v-field__outline__end {
  border-top-right-radius: 100px !important;
  border-bottom-right-radius: 100px !important;
  padding-left: 24px !important;
}

.my-input .v-btn__content {
  text-transform: none;
}

.my-input .v-input__details {
  min-height: unset;
  text-align: left;
  padding: 10px 24px;
}

.countries-select .v-select {
  font-weight: 500;
  width: 120px;
  margin: auto;
}

.countries-select .mdi-menu-down::before {
  color: #0074bd;
}

.my-check-box .v-label {
  font-size: 14px;
  opacity: 1;
  color: #2a2a2a;
}

.my-check-box .v-selection-control {
  min-height: unset !important;
}
.my-check-box .check-box-label {
  cursor: pointer;
}

.my-check-box .v-selection-control__input > .v-icon {
  opacity: 1;
  color: #0074bd;
}

.hide-input-detail .v-input__details {
  display: none;
}
</style>
