<template>
  <div>
    <b-navbar toggleable="lg" type="light" variant="light" fixed="top">
      <b-container>
        <b-navbar-brand href="/">
          <b-img src="@/assets/logo.png" />
        </b-navbar-brand>

        <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

        <b-collapse id="nav-collapse" is-nav>
          <b-navbar-nav>
            <b-nav-item-dropdown text="Categories" left>
              <b-dropdown-item href="#">Cleanser</b-dropdown-item>
              <b-dropdown-item href="#">Moisturizer</b-dropdown-item>
              <b-dropdown-item href="#">Treatment</b-dropdown-item>
              <b-dropdown-item href="#">Protection</b-dropdown-item>
            </b-nav-item-dropdown>
            <b-nav-item-dropdown text="Brands" left>
              <b-dropdown-item href="#">EN</b-dropdown-item>
              <b-dropdown-item href="#">ES</b-dropdown-item>
              <b-dropdown-item href="#">RU</b-dropdown-item>
              <b-dropdown-item href="#">FA</b-dropdown-item>
            </b-nav-item-dropdown>
            <b-nav-item href="#">Sale</b-nav-item>
          </b-navbar-nav>

          <!-- Right aligned nav items -->
          <b-navbar-nav class="ml-auto">
            <b-nav-form>
              <b-input-group size="sm">
                <b-form-input placeholder="Search"></b-form-input>
                <b-input-group-append>
                  <b-button type="submit">
                    <font-awesome-icon :icon="['fas', 'search']" />
                  </b-button>
                </b-input-group-append>
              </b-input-group>
            </b-nav-form>

            <b-nav-item>
              <nuxt-link to="/signin">Signin</nuxt-link>
            </b-nav-item>
            <b-nav-item disabled>/</b-nav-item>
            <b-nav-item>
              <nuxt-link to="/register">Register</nuxt-link>
            </b-nav-item>
            <b-nav-item>
              <font-awesome-icon :icon="['fas', 'shopping-cart']" />
              <b-badge pill variant="warning">1</b-badge>
            </b-nav-item>
          </b-navbar-nav>
        </b-collapse>
      </b-container>
    </b-navbar>
  </div>
</template>

<script>
export default {
  name: "Navbar"
};
</script>

<style>
.badge-warning {
  color: white;
}
</style>
