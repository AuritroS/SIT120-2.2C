<template>
  <div class="container">
    <img :src="shoe1" alt="" />
    <div class="details">
      <h2>Shoes 1</h2>
      <h3>Mens Shoes</h3>
      <h4>$100</h4>
      <h3 class="size-label">Select Size</h3>
      <div class="sizes">
        <button>US 6</button><button>US 6.5</button><button>US 7</button>
        <button>US 6</button><button>US 6.5</button><button>US 7</button>
        <button>US 6</button><button>US 6.5</button><button>US 7</button>
      </div>
      <button class="add">Add to Bag</button>
      <button class="favorite">Favorite</button>
    </div>
  </div>
</template>

<script>
import shoe1 from "../assets/Duramo_10_Shoes_Black_GW8336_01_standard.avif";

export default {
  name: "DetailView",
  data() {
    return {
      shoe1,
    };
  },
};
</script>

<style scoped>
img {
  max-width: 700px;
  margin-top: 100px;
}
.container {
  display: flex;
  justify-content: space-evenly;
  align-items: center;
}
.sizes {
  width: 50%;
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
}
button {
  background: transparent;
  border-style: solid;
  border-color: black;
  border-width: 1px;
  width: 100px;
  height: 50px;
  border-radius: 5px;
  margin: 5px;
}
.add {
  background: black;
  color: white;
  width: 100%;
  border-radius: 50px;
  margin-top: 20px;
}
.favorite {
  width: 100%;
  border-radius: 50px;
}
h4 {
  margin-top: 30px;
}
.size-label {
  margin-top: 40px;
}
</style>
