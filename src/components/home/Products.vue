<template>
  <section>
    <div class="content">
      <div class="search-part">
        <div class="searchBar">
          <input id="searchQueryInput" type="text" name="searchQueryInput" value=""/>
          <button id="searchQuerySubmit" type="submit" name="searchQuerySubmit">
            <i class="fa-solid fa-magnifying-glass search-icon"></i>
          </button>
        </div>
        <div class="save-icon">
          <i class="fa-solid fa-bookmark saved-icon"></i>
        </div>
        <div class="icon">
          <i class="fa-solid fa-arrow-up-wide-short filter-icon"></i>
        </div>
      </div>
      <div class="container">
        <div class="row">
          <div class="col-xl-3 col-lg-3 col-md-4 col-sm-6 col-12" v-for="product in products" :key="product.id">
            <div class="card" >
              <div class="img-part">
                  <img src="https://www.desser.co.uk/wp-content/uploads/2022/02/mango-wood-furniture--1024x683.jpg"/>
              </div>
              <div class="text-part">
                <h3>
                  {{product.name}} 
                </h3>
                <br>
                <span>
                  {{product.desc}} 
                </span>
                <br> <br>
                <span class="price">
                  ${{product.price}}
                </span>
              </div>
              <div class="reacts">
                <div class="like-icon">
                  <i class="fa-solid fa-thumbs-up"></i>
                </div>
                <div class="dislike-icon">
                  <i class="fa-solid fa-thumbs-down"></i>
                </div>
                <div class="save-icon">
                  <i class="fa-solid fa-bookmark saved-icon"></i>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name:"Products",
  data() {
    return {
      products: [
        {
          id: 1,
          name: "Lorem ipsum dolor",
          desc:"ipsum dolor sit amet consectetur adipisicing elit. Obcaecati unde cum distinctio",
          price: 405,
        },
        {
          id: 2,
          name: "Lorem ipsum dolor",
          desc:"ipsum dolor sit amet consectetur adipisicing elit. Obcaecati unde cum distinctio",
          price: 246,
        },
        {
          id: 3,
          name: "Lorem ipsum dolor",
          desc:"ipsum dolor sit amet consectetur adipisicing elit. Obcaecati unde cum distinctio",
          price: 454,
        },
        {
          id: 4,
          name: "Lorem ipsum dolor",
          desc:"ipsum dolor sit amet consectetur adipisicing elit. Obcaecati unde cum distinctio",
          price: 543,
        },
        {
          id: 5,
          name: "Lorem ipsum dolor",
          desc:"ipsum dolor sit amet consectetur adipisicing elit. Obcaecati unde cum distinctio",
          price: 165,
        },
        
      ]
    }
  }
};
</script>

<style scoped>
@import "../../assets/CSS/Products.css";
</style>