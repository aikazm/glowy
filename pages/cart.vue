<template>
  <div class="cart mb-5">
    <b-container>
      <h1 class="text-center mb-4">My Shopping Cart</h1>
      <table class="table">
        <thead>
          <tr>
            <th>Product Details</th>
            <th>Price</th>
            <th>Qty</th>
            <th>Total</th>
          </tr>
        </thead>
        <tbody>
          <tr v-for="product in products" :key="product.id">
            <td>
              <figure class="figure">
                <b-img :src="product.img" class="thumbnail-product mr-3" />
                <h6>{{ product.brand }}</h6>
                <figcaption class="figure-caption">{{ product.name }}</figcaption>
              </figure>
            </td>
            <td>Rp {{product.price}}</td>
            <td>
              <div>
                <b-form-spinbutton class="btn-inc-dec" v-model="product.qty" min="1" max="100"></b-form-spinbutton>
              </div>
            </td>
            <td>{{ total }}</td>
          </tr>
        </tbody>
      </table>
      <b-row>
        <b-col>
          <b-button>
            <font-awesome-icon :icon="['fas', 'arrow-left']" class="mr-2" />Continue Shopping
          </b-button>
        </b-col>
        <b-col cols="3">
          <b-row>
            <b-col>
              <p>Sub Total</p>
              <p>Total</p>
            </b-col>
            <b-col class="text-right">
              <p>Rp 20.000</p>
              <p>Rp 20.000</p>
            </b-col>
          </b-row>
          <div class="d-flex justify-content-end">
            <b-button>
              Checkout
              <font-awesome-icon :icon="['fas', 'arrow-right']" class="ml-2" />
            </b-button>
          </div>
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
export default {
  data() {
    return {
      products: [
        {
          id: 1,
          brand: "nivea",
          img: "@/assets/nivea-1.jpg",
          name: "Double Eye Make Up Remover",
          price: 60500,
          qty: 1
        },
        {
          id: 2,
          brand: "nivea",
          img: "@/assets/nivea-2.jpg",
          name: "Face Care Make Up Starter Serum SPF 33",
          price: 48750,
          qty: 1
        }
      ],
      total: 0
    };
  },
  computed: {
    total: function() {
      return this.qty * this.price;
    }
  }
};
</script>

<style>
.cart {
  margin-top: 120px;
}
.thumbnail-product {
  height: 60px;
  float: left;
}
.btn-inc-dec {
  width: 130px;
}
</style>