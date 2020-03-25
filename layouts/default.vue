<template>
  <div>
    <Navbar />
    <nuxt />
    <Footer />
  </div>
</template>

<script>
import Navbar from "~/components/Navbar";
import Footer from "~/components/Footer";

export default {
  components: {
    Navbar,
    Footer
  }
};
</script>

<style>
body {
  font-family: "Baloo Chettan 2", cursive;
  margin-top: 95px;
}
h1 {
  font-family: "Parisienne", cursive;
}
.btn {
  background-color: #ff8da1;
  border: #ff8da1;
  color: white;
}

.btn:hover {
  background-color: #ff6681;
  border: #ff6681;
  color: white;
}

.badge {
  position: absolute;
}
</style>
