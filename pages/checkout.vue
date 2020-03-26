<template>
  <div class="checkout mb-5">
    <b-container>
      <b-row>
        <b-col>
          <div class="shipping-address">
            <b-row>
              <b-col>
                <h4 class="mb-4">Shipping Address</h4>
                <b-form>
                  <b-row>
                    <b-col>
                      <b-form-group id="input-group-2" label="First Name*" label-for="input-2">
                        <b-form-input id="input-2" required></b-form-input>
                      </b-form-group>
                    </b-col>
                    <b-col>
                      <b-form-group id="input-group-2" label="Last Name*" label-for="input-2">
                        <b-form-input id="input-2" required></b-form-input>
                      </b-form-group>
                    </b-col>
                  </b-row>
                  <b-form-group id="input-group-2" label="Full Address*" label-for="input-2">
                    <b-form-input id="input-2" required></b-form-input>
                  </b-form-group>
                  <b-form-group id="input-group-2" label="City*" label-for="input-2">
                    <b-form-input id="input-2" required></b-form-input>
                  </b-form-group>
                  <b-form-group id="input-group-2" label="Phone Number*" label-for="input-2">
                    <b-form-input id="input-2" required></b-form-input>
                  </b-form-group>
                </b-form>
              </b-col>
            </b-row>
          </div>
        </b-col>
        <b-col cols="5">
          <div class="order-summary">
            <h4 class="mb-4">Order Summary</h4>
            <b-row>
              <b-col>
                <figure class="figure">
                  <b-img src="@/assets/nivea-1.jpg" class="thumbnail-product mr-3" />
                  <h6>NIVEA</h6>
                  <figcaption class="figure-caption">Double Eye Make Up Remover</figcaption>
                </figure>
              </b-col>
              <b-col class="text-right">
                <p>Qty: 1</p>
                <p>Rp. 20.000</p>
              </b-col>
            </b-row>
            <b-row>
              <b-col>
                <p>Sub Total</p>
                <p>Discount</p>
                <p>Shipping</p>
                <p>Total</p>
              </b-col>
              <b-col class="text-right">
                <p>Rp 20.000</p>
                <p>-</p>
                <p>-</p>
                <p>Rp 20.000</p>
              </b-col>
            </b-row>
          </div>
          <div class="mt-4 text-right">
            <b-button>Proceed To Payment</b-button>
          </div>
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<style>
.checkout {
  margin-top: 120px;
}
.thumbnail-product {
  height: 60px;
  float: left;
}
.order-summary,
.shipping-address {
  border: 2px solid #f4f4f4;
  padding: 20px;
  border-radius: 10px;
}
</style>