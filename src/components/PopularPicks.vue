<template>
  <section class="popular-picks">
    <h2>Popular Picks</h2>
    <section class="shoes">
      <RouterLink to="/shoes/1" class="shoe">
        <img :src="shoe1" alt="shoe1" />
        <h3>Shoe 1</h3>
      </RouterLink>
      <RouterLink to="/shoes/2" class="shoe">
        <img :src="shoe2" alt="shoe2" />
        <h3>Shoe 2</h3>
      </RouterLink>
      <RouterLink to="/shoes/3" class="shoe">
        <img :src="shoe3" alt="shoe3" />
        <h3>Shoe 3</h3>
      </RouterLink>
    </section>
  </section>
</template>

<script>
import shoe1 from "../assets/Duramo_10_Shoes_Black_GW8336_01_standard.avif";
import shoe2 from "../assets/NMD_R1_Shoes_Black_GZ9258_01_standard.avif";
import shoe3 from "../assets/NMD_R1_Shoes_White_GZ9261_01_standard.avif";

export default {
  name: "PopularPicks",
  data() {
    return {
      shoe1,
      shoe2,
      shoe3,
    };
  },
};
</script>

<style scoped>
.popular-picks {
  margin-top: 500px;
  padding: 0 10%;
}
h2 {
  font-weight: 600;
  font-size: 30px;
  margin-bottom: 50px;
}
a {
  text-decoration: none;
  color: black;
}
.shoes {
  display: flex;
  justify-content: space-between;
}

h3 {
  font-weight: 500;
  font-size: 25px;
}
img {
  max-width: 300px;
}

@media screen and (max-width: 1000px) {
  .shoes {
    flex-direction: column;
  }
  .shoe {
    margin-top: 50px;
  }
}
</style>
