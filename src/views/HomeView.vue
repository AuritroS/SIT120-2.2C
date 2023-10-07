<template>
  <HeaderImage />
  <PopularPicks />
</template>

<script>
// @ is an alias to /src
import HeaderImage from "@/components/HeaderImage.vue";
import PopularPicks from "@/components/PopularPicks.vue";

export default {
  name: "HomeView",
  components: {
    HeaderImage,
    PopularPicks,
  },
};
</script>
