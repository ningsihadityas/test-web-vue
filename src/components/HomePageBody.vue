<template>
  <div>

    <div class="image-container">
        <!-- displaying by range -->
      <div v-for="index in 10" :key="index" class="pic">
        <img :src="companyLogo[index].url" />
      </div>
    </div>
   
    <!-- <div class="image-container">
      <div v-for="logo in companyLogo" :key="logo.id" class="pic">
        <img :src="logo.url" :alt="logo.title" />
      </div>
    </div> -->
  </div>
</template>

<script>
import axios from "axios";

export default {
  name: "HomePageBody",
  data() {
    return {
      companyLogo: [],
    };
  },
  mounted() {
    axios
      .get("https://jsonplaceholder.typicode.com/photos")
      .then((response) => {
        console.log("RESPONSE", response);
        if (response.status == 200) {
          this.companyLogo = response.data;
        }
      })
      .catch((error) => console.log(error));
  },
  methods: {
    onclicked() {
      console.log("click");
    },
  },
};
</script>

<style lang="scss">
.image-container {
    display: flex;
    flex-wrap: wrap;
    justify-content: flex-start;
    max-height: ;
  .pic {
    min-height: 75px;
   
    // img {
    //   height: 75px;
    // }
  }
}
</style>
