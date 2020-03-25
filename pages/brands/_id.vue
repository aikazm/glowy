<template>
  <div>
    <b-container>
      <b-breadcrumb :items="items"></b-breadcrumb>
      <b-row>
        <b-col cols="2">
          <h5>Brands</h5>
          <b-input-group size="sm">
            <b-form-input placeholder="Search"></b-form-input>
            <b-input-group-append>
              <b-button type="submit">
                <font-awesome-icon :icon="['fas', 'search']" />
              </b-button>
            </b-input-group-append>
          </b-input-group>
          <b-nav vertical class="w-25">
            <b-nav-item active>Active</b-nav-item>
            <b-nav-item>Link</b-nav-item>
            <b-nav-item>Another Link</b-nav-item>
            <b-nav-item>Disabled</b-nav-item>
          </b-nav>
        </b-col>
        <b-col>
          <figure class="figure">
            <img src="@/assets/nivea.jpg" class="figure-img img-fluid rounded" />
            <h5>About The Brand</h5>
            <figcaption
              class="figure-caption"
            >Lorem ipsum dolor sit, amet consectetur adipisicing elit. Sequi provident optio eaque quam suscipit harum reprehenderit ab dolorum aspernatur. Excepturi architecto quis laboriosam nulla fugit veritatis, nihil modi exercitationem possimus.</figcaption>
          </figure>

          <b-form inline class="mb-3">
            <label class="mr-sm-2" for="inline-form-custom-select-pref">Sort By :</label>
            <b-form-select
              id="inline-form-custom-select-pref"
              class="mb-2 mr-sm-2 mb-sm-0"
              :options="[{ text: 'Choose...', value: null }, 'One', 'Two', 'Three']"
              :value="null"
            ></b-form-select>
          </b-form>

          <b-row>
            <b-col>
              <figure class="figure">
                <img src="@/assets/nivea-1.jpg" class="figure-img img-fluid rounded" />
                <h6>NIVEA</h6>
                <figcaption class="figure-caption">Double Eye Make Up Remover</figcaption>
                <figcaption class="figure-caption">
                  <strike>Rp 60.500</strike>
                </figcaption>
                <h6>Rp. 48.400</h6>
              </figure>
            </b-col>
            <b-col>
              <figure class="figure">
                <img src="@/assets/nivea-1.jpg" class="figure-img img-fluid rounded" />
                <h6>NIVEA</h6>
                <figcaption class="figure-caption">Double Eye Make Up Remover</figcaption>
                <figcaption class="figure-caption">
                  <strike>Rp 60.500</strike>
                </figcaption>
                <h6>Rp. 48.400</h6>
              </figure>
            </b-col>
            <b-col>
              <figure class="figure">
                <img src="@/assets/nivea-1.jpg" class="figure-img img-fluid rounded" />
                <h6>NIVEA</h6>
                <figcaption class="figure-caption">Double Eye Make Up Remover</figcaption>
                <figcaption class="figure-caption">
                  <strike>Rp 60.500</strike>
                </figcaption>
                <h6>Rp. 48.400</h6>
              </figure>
            </b-col>
            <b-col>
              <figure class="figure">
                <img src="@/assets/nivea-1.jpg" class="figure-img img-fluid rounded" />
                <h6>NIVEA</h6>
                <figcaption class="figure-caption">Double Eye Make Up Remover</figcaption>
                <figcaption class="figure-caption">
                  <strike>Rp 60.500</strike>
                </figcaption>
                <h6>Rp. 48.400</h6>
              </figure>
            </b-col>
            <b-col>
              <figure class="figure">
                <img src="@/assets/nivea-1.jpg" class="figure-img img-fluid rounded" />
                <h6>NIVEA</h6>
                <figcaption class="figure-caption">Double Eye Make Up Remover</figcaption>
                <figcaption class="figure-caption">
                  <strike>Rp 60.500</strike>
                </figcaption>
                <h6>Rp. 48.400</h6>
              </figure>
            </b-col>
          </b-row>
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
.breadcrumb {
  background-color: none;
}
</style>