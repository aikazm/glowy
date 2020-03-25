<template>
  <div class="home">
    <section class="carousel mb-4">
      <b-carousel
        id="carousel-fade"
        style="text-shadow: 0px 0px 2px #000"
        fade
        indicators
        img-width="1024"
        img-height="480"
      >
        <b-carousel-slide
          caption="Face Masks"
          img-src="@/assets/img-1.png"
          img-alt="People photo created by senivpetro - www.freepik.com"
        ></b-carousel-slide>
        <b-carousel-slide
          caption="Moisturizer"
          img-src="@/assets/img-2.png"
          img-alt="Woman photo created by pressfoto - www.freepik.com"
        ></b-carousel-slide>
        <b-carousel-slide
          caption="Body Care"
          img-src="@/assets/img-3.png"
          img-alt="Hand photo created by freepik - www.freepik.com"
        ></b-carousel-slide>
      </b-carousel>
    </section>

    <section class="sale mb-4">
      <b-container class="text-center">
        <h1>Sale</h1>
        <figure class="figure">
          <img src="@/assets/nivea-1.jpg" class="figure-img img-fluid rounded" />
          <b-badge pill variant="danger">-20%</b-badge>
          <h6>NIVEA</h6>
          <figcaption class="figure-caption">Double Eye Make Up Remover</figcaption>
          <figcaption class="figure-caption">
            <strike>Rp 60.500</strike>
          </figcaption>
          <h6>Rp. 48.400</h6>
        </figure>

        <figure class="figure">
          <img src="@/assets/nivea-2.jpg" class="figure-img img-fluid rounded" />
          <b-badge pill variant="danger">-15%</b-badge>
          <h6>NIVEA</h6>
          <figcaption class="figure-caption">Face Care Make Up Starter Serum SPF 33</figcaption>
          <figcaption class="figure-caption">
            <strike>Rp 48.750</strike>
          </figcaption>
          <h6>Rp 41.438</h6>
        </figure>

        <figure class="figure">
          <img src="@/assets/nivea-3.jpg" class="figure-img img-fluid rounded" />
          <b-badge pill variant="danger">-15%</b-badge>
          <h6>NIVEA</h6>
          <figcaption class="figure-caption">Hydrating Cleansing Oil</figcaption>
          <figcaption class="figure-caption">
            <strike>Rp 92.000</strike>
          </figcaption>
          <h6>Rp 78.200</h6>
        </figure>

        <figure class="figure">
          <img src="@/assets/nivea-4.jpg" class="figure-img img-fluid rounded" />
          <b-badge pill variant="danger">-20%</b-badge>
          <h6>NIVEA</h6>
          <figcaption class="figure-caption">Hydration Micellair Skin Breathe</figcaption>
          <figcaption class="figure-caption">
            <strike>Rp 45.000</strike>
          </figcaption>
          <h6>Rp 36.000</h6>
        </figure>

        <b-button class="d-flex ml-auto">See More</b-button>
      </b-container>
    </section>

    <section class="best-seller mb-5">
      <b-container class="text-center">
        <h1>Best Seller</h1>

        <div>
          <figure class="figure">
            <img src="@/assets/nivea-1.jpg" class="figure-img img-fluid rounded" />
            <h6>NIVEA</h6>
            <figcaption class="figure-caption">Double Eye Make Up Remover</figcaption>
            <figcaption class="figure-caption">
              <strike>Rp 60.500</strike>
            </figcaption>
            <h6>Rp. 48.400</h6>
          </figure>

          <figure class="figure">
            <img src="@/assets/nivea-1.jpg" class="figure-img img-fluid rounded" />
            <h6>NIVEA</h6>
            <figcaption class="figure-caption">Double Eye Make Up Remover</figcaption>
            <figcaption class="figure-caption">
              <strike>Rp 60.500</strike>
            </figcaption>
            <h6>Rp. 48.400</h6>
          </figure>

          <figure class="figure">
            <img src="@/assets/nivea-1.jpg" class="figure-img img-fluid rounded" />
            <h6>NIVEA</h6>
            <figcaption class="figure-caption">Double Eye Make Up Remover</figcaption>
            <figcaption class="figure-caption">
              <strike>Rp 60.500</strike>
            </figcaption>
            <h6>Rp. 48.400</h6>
          </figure>

          <figure class="figure">
            <img src="@/assets/nivea-1.jpg" class="figure-img img-fluid rounded" />
            <h6>NIVEA</h6>
            <figcaption class="figure-caption">Double Eye Make Up Remover</figcaption>
            <figcaption class="figure-caption">
              <strike>Rp 60.500</strike>
            </figcaption>
            <h6>Rp. 48.400</h6>
          </figure>
        </div>

        <div>
          <figure class="figure">
            <img src="@/assets/nivea-1.jpg" class="figure-img img-fluid rounded" />
            <h6>NIVEA</h6>
            <figcaption class="figure-caption">Double Eye Make Up Remover</figcaption>
            <figcaption class="figure-caption">
              <strike>Rp 60.500</strike>
            </figcaption>
            <h6>Rp. 48.400</h6>
          </figure>

          <figure class="figure">
            <img src="@/assets/nivea-1.jpg" class="figure-img img-fluid rounded" />
            <h6>NIVEA</h6>
            <figcaption class="figure-caption">Double Eye Make Up Remover</figcaption>
            <figcaption class="figure-caption">
              <strike>Rp 60.500</strike>
            </figcaption>
            <h6>Rp. 48.400</h6>
          </figure>

          <figure class="figure">
            <img src="@/assets/nivea-1.jpg" class="figure-img img-fluid rounded" />
            <h6>NIVEA</h6>
            <figcaption class="figure-caption">Double Eye Make Up Remover</figcaption>
            <figcaption class="figure-caption">
              <strike>Rp 60.500</strike>
            </figcaption>
            <h6>Rp. 48.400</h6>
          </figure>
        </div>
        <b-button class="button">See More</b-button>
      </b-container>
    </section>

    <section class="our-picks mb-5">
      <b-container class="text-center">
        <h1>Our Pick's</h1>
        <div>
          <b-nav align="center" class="mb-3">
            <b-nav-item active>Oily</b-nav-item>
            <b-nav-item>Combination</b-nav-item>
            <b-nav-item>Normal</b-nav-item>
            <b-nav-item>Dry</b-nav-item>
            <b-nav-item>Sensitive</b-nav-item>
          </b-nav>
        </div>
        <div>
          <figure class="figure">
            <img src="@/assets/nivea-1.jpg" class="figure-img img-fluid rounded" />
            <h6>NIVEA</h6>
            <figcaption class="figure-caption">Double Eye Make Up Remover</figcaption>
            <figcaption class="figure-caption">
              <strike>Rp 60.500</strike>
            </figcaption>
            <h6>Rp. 48.400</h6>
          </figure>

          <figure class="figure">
            <img src="@/assets/nivea-1.jpg" class="figure-img img-fluid rounded" />
            <h6>NIVEA</h6>
            <figcaption class="figure-caption">Double Eye Make Up Remover</figcaption>
            <figcaption class="figure-caption">
              <strike>Rp 60.500</strike>
            </figcaption>
            <h6>Rp. 48.400</h6>
          </figure>

          <figure class="figure">
            <img src="@/assets/nivea-1.jpg" class="figure-img img-fluid rounded" />
            <h6>NIVEA</h6>
            <figcaption class="figure-caption">Double Eye Make Up Remover</figcaption>
            <figcaption class="figure-caption">
              <strike>Rp 60.500</strike>
            </figcaption>
            <h6>Rp. 48.400</h6>
          </figure>

          <figure class="figure">
            <img src="@/assets/nivea-1.jpg" class="figure-img img-fluid rounded" />
            <h6>NIVEA</h6>
            <figcaption class="figure-caption">Double Eye Make Up Remover</figcaption>
            <figcaption class="figure-caption">
              <strike>Rp 60.500</strike>
            </figcaption>
            <h6>Rp. 48.400</h6>
          </figure>

          <figure class="figure">
            <img src="@/assets/nivea-1.jpg" class="figure-img img-fluid rounded" />
            <h6>NIVEA</h6>
            <figcaption class="figure-caption">Double Eye Make Up Remover</figcaption>
            <figcaption class="figure-caption">
              <strike>Rp 60.500</strike>
            </figcaption>
            <h6>Rp. 48.400</h6>
          </figure>
        </div>
      </b-container>
    </section>
  </div>
</template>

<style scoped>
.figure-img {
  height: 200px;
}
h1 {
  font-family: "Parisienne", cursive;
}
.nav-item .active {
  border-bottom: 5px solid #ff8da1;
}
</style>
