<template>
  <div class="register d-flex align-items-center flex-column mb-5">
    <b-row>
      <b-col class="register-form">
        <h1 class="text-center">Create an Account</h1>
        <div class="mt-4">
          <b-form @submit="onSubmit" v-if="show">
            <b-form-group id="firstName" label="First Name*" label-for="first-name">
              <b-form-input
                id="firstName"
                v-model="form.firstName"
                type="text"
                placeholder="Enter Your Firt Name"
                required
              ></b-form-input>
            </b-form-group>

            <b-form-group id="lastName" label="Last Name*" label-for="last-name">
              <b-form-input
                id="lastName"
                v-model="form.lastName"
                type="text"
                placeholder="Enter Your Last Name"
                required
              ></b-form-input>
            </b-form-group>

            <b-form-group id="email" label="Email Address*" label-for="email">
              <b-form-input
                id="email"
                v-model="form.email"
                type="email"
                required
                placeholder="Enter email"
              ></b-form-input>
            </b-form-group>

            <b-form-group id="password" label="Password*" label-for="password">
              <b-form-input
                id="password"
                v-model="form.password"
                type="password"
                required
                placeholder="Enter password"
              ></b-form-input>
            </b-form-group>

            <b-button class="btn-register" type="submit">Register</b-button>

            <p class="text-center mt-2">
              Already have an account?
              <nuxt-link to="/register">Sign in</nuxt-link>
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
.btn-register {
  width: -moz-available;
}
.register {
  margin-top: 120px;
}
.register-form {
  background-color: #fff1f4;
  padding: 30px;
  box-shadow: 15px 15px 5px #eaeaea;
}
</style>