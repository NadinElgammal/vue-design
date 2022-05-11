<template>
<section>
    <Header />
    <IntroDiv />
    <Products />
</section>
</template>

<script>
import Header from "../layouts/Header.vue";
import IntroDiv from "../components/home/IntroDiv.vue";
import Products from "../components/home/Products.vue";

export default {
components: {
    Header,
    IntroDiv,
    Products,
},
};
</script>
