<template>
  <div class="footer">
    <b-container>
      <b-row>
        <b-col cols="2">
          <b-img src="@/assets/logo.png" />
        </b-col>
        <b-col>
          <b-nav vertical>
            <b-nav-item disabled>Bandung, Indonesia</b-nav-item>
            <b-nav-item disabled>Customer Service</b-nav-item>
            <b-nav-item disabled>cs@glowy.com</b-nav-item>
          </b-nav>
        </b-col>
        <b-col>
          <div>
            <b-nav vertical>
              <b-nav-item>FAQ</b-nav-item>
              <b-nav-item>Blog</b-nav-item>
              <b-nav-item>Terms & Condition</b-nav-item>
              <b-nav-item>Privacy Policy</b-nav-item>
            </b-nav>
          </div>
        </b-col>
        <b-col>
          <b-nav vertical>
            <b-nav-item disabled>Newsletter Subscription</b-nav-item>
            <b-nav-item>
              <b-input-group size="sm">
                <b-form-input placeholder="Enter Your Email Here" type="email"></b-form-input>
                <b-input-group-append>
                  <b-button>Subscribe</b-button>
                </b-input-group-append>
              </b-input-group>
            </b-nav-item>
          </b-nav>

          <b-nav>
            <b-nav-item>
              <font-awesome-icon :icon="['fab', 'facebook-f']" />
            </b-nav-item>
            <b-nav-item>
              <font-awesome-icon :icon="['fab', 'twitter']" />
            </b-nav-item>
            <b-nav-item>
              <font-awesome-icon :icon="['fab', 'instagram']" />
            </b-nav-item>
          </b-nav>
        </b-col>
      </b-row>
    </b-container>
    <p class="copyright text-center">2020 © Glowy. All Rights Reserved</p>
  </div>
</template>

<script>
export default {
  name: "Footer"
};
</script>

<style>
.nav-item .nav-link {
  color: #75797d;
}
.footer {
  background-color: #f8f9fa;
  padding-top: 10px;
}
</style>
