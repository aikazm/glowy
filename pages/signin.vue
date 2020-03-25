<template>
  <div class="signin d-flex align-items-center flex-column mb-5">
    <b-row>
      <b-col class="signin-form">
        <h1 class="text-center">Sign in</h1>
        <div class="mt-4">
          <b-form @submit="onSubmit" @reset="onReset" v-if="show">
            <b-form-group
              id="input-group-1"
              label="Email address"
              label-for="input-1"
              description="We'll never share your email with anyone else."
            >
              <b-form-input
                id="input-1"
                v-model="form.email"
                type="email"
                required
                placeholder="Enter email"
              ></b-form-input>
            </b-form-group>

            <b-form-group id="input-group-2" label="Password" label-for="input-2">
              <b-form-input
                id="input-2"
                v-model="form.password"
                type="password"
                required
                placeholder="Enter password"
              ></b-form-input>
            </b-form-group>

            <a href>
              <p>Forget Password?</p>
            </a>

            <b-button class="btn-signin" type="submit">Sign in</b-button>

            <p class="text-center mt-2">
              Don't have an account?
              <nuxt-link to="/register">Sign up</nuxt-link>
            </p>
          </b-form>
        </div>
      </b-col>
    </b-row>
  </div>
</template>

<script>
export default {
  data() {
    return {
      form: {
        email: "",
        password: ""
      },
      show: true
    };
  },
  methods: {
    onSubmit(evt) {
      evt.preventDefault();
      alert(JSON.stringify(this.form));
    }
  }
};
</script>

<style>
.btn-signin {
  width: -moz-available;
}
.signin {
  margin-top: 120px;
}
.signin-form {
  background-color: #fff1f4;
  padding: 30px;
  box-shadow: 15px 15px 5px #eaeaea;
}
</style>