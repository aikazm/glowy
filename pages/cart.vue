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
          <tr>
            <td>
              <figure class="figure">
                <b-img src="@/assets/nivea-1.jpg" class="thumbnail-product mr-3" />
                <h6>NIVEA</h6>
                <figcaption class="figure-caption">Double Eye Make Up Remover</figcaption>
              </figure>
            </td>
            <td>Rp 20.000</td>
            <td>
              <div>
                <b-input-group size="sm">
                  <b-input-group-prepend>
                    <b-button>
                      <font-awesome-icon :icon="['fas', 'minus']" />
                    </b-button>
                  </b-input-group-prepend>

                  <b-form-input class="qty"></b-form-input>

                  <b-input-group-append>
                    <b-button>
                      <font-awesome-icon :icon="['fas', 'plus']" />
                    </b-button>
                  </b-input-group-append>
                </b-input-group>
              </div>
            </td>
            <td>Rp 20.000</td>
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


<style>
.cart {
  margin-top: 120px;
}
.thumbnail-product {
  height: 60px;
  float: left;
}
.qty {
  width: 5px;
}
</style>