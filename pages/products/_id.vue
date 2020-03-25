<template>
  <div>
    <b-container>
      <b-breadcrumb :items="items"></b-breadcrumb>

      <b-row>
        <b-col cols="4">
          <b-img class="product-img text-center" src="@/assets/nivea-1.jpg"></b-img>
          <ul>
            <li>
              <b-img class="product-thumbnail" rounded src="@/assets/nivea-1.jpg"></b-img>
            </li>
          </ul>
        </b-col>
        <b-col>
          <h6>NIVEA</h6>
          <p class="product-name">Double Eye Make Up Remover</p>
          <ul class="price">
            <li class="after">Rp. 48.400</li>
            <li class="disc">-20%</li>
            <li class="before">
              <strike>Rp 60.500</strike>
            </li>
          </ul>

          <!-- <ul class="mt-3">
            <li>Qty</li>
            <li>
              <b-input-group>
                <b-input-group-prepend>
                  <b-button>-</b-button>
                </b-input-group-prepend>

                <b-form-input></b-form-input>

                <b-input-group-append>
                  <b-button>+</b-button>
                </b-input-group-append>
              </b-input-group>
            </li>
          </ul>-->

          <div class="mt-3">
            <b-tabs content-class="mt-3">
              <b-tab title="Description" active>
                <p>Efektif menghapus make up, bahkan maskara yang sangat waterprrof. Memberikan kelembapan untuk kulit area mata yang lembut, serta melindungi bulu mata. Membersihkan make up dengan sangat lembut, tidak perlu diusap dengan keras.</p>
              </b-tab>
              <b-tab title="Review">
                <p>I'm the second tab</p>
              </b-tab>
            </b-tabs>
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
      items: [
        {
          text: "Home",
          href: "#"
        },
        {
          text: "Brands",
          active: true
        }
      ]
    };
  }
};
</script>

<style>
/* Breadcrumb */
.breadcrumb {
  margin-top: 30px;
  background: transparent;
}
.product-img {
  height: 325px;
}

.product-thumbnail {
  height: 73px;
  border: 2px solid #ffc4ce;
}
.product-name,
.price .before {
  color: #6c757d;
}

li {
  display: inline;
}

ul {
  margin: 0;
  padding: 0;
}

.disc {
  background-color: #ff8da1;
  color: white;
  margin: 20px;
  padding: 5px;
}
</style>