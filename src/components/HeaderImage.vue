<template>
  <section class="header-img">
    <img :src="image" alt="graphic" class="graphic" />
    <img :src="imageSmaller" alt="graphic" class="graphic-smaller" />
  </section>
</template>

<script>
import image from "../assets/website-banner-desktop-landscape.webp";
import imageSmaller from "../assets/website-banner-desktop-landscape-smaller.webp";

export default {
  name: "HeaderImage",
  data: function () {
    return {
      image,
      imageSmaller,
    };
  },
};
</script>

<style scoped>
.header-img {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
}
img {
  height: 450px;
  width: 100%;
  object-fit: cover;
}
.graphic-smaller {
  display: none;
}
@media screen and (max-width: 1000px) {
  .graphic {
    display: none;
  }
  .graphic-smaller {
    display: inline;
  }
}
</style>
