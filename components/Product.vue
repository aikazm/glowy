<template>
  <div>
    <figure class="figure">
      <img :src="product.img" class="figure-img img-fluid rounded" />
      <b-badge pill variant="danger">- {{ product.disc }} %</b-badge>
      <h6>{{ product.brand }}</h6>
      <figcaption class="figure-caption">{{ product.name }}</figcaption>
      <figcaption class="figure-caption">
        <strike>Rp 60.500</strike>
      </figcaption>
      <h6>{{ product.price }}</h6>
    </figure>
  </div>
</template>

<script>
export default {
  name: "Product",
  data() {
    return {
      products: [
        {
          id: 1,
          brand: "Nivea",
          img: "@/assets/nivea-1.jpg",
          name: "Double Eye Make Up Remover",
          price: 60500,
          disc: 20,
          qty: 1
        },
        {
          id: 2,
          brand: "Nivea",
          img: "@/assets/nivea-2.jpg",
          name: "Face Care Make Up Starter Serum SPF 33",
          price: 48750,
          disc: 15,
          qty: 1
        },
        {
          id: 3,
          brand: "Nivea",
          img: "@/assets/nivea-3.jpg",
          name: "Hydrating Cleansing Oil",
          price: 92000,
          disc: 15,
          qty: 1
        },
        {
          id: 4,
          brand: "Nivea",
          img: "@/assets/nivea-4.jpg",
          name: "Hydration Micellair Skin Breathe",
          price: 45000,
          disc: 20,
          qty: 1
        }
      ]
    };
  }
};
</script>