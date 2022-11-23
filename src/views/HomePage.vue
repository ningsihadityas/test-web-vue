<!-- <template>
  <div id="home">
    <h1>vue test</h1>
    <form >
        <div class="field">
            <label class="label">Email</label> <br>
            
            <input type="text" placeholder="enter email" v-model="email">
            <p> email: {{ kelas }} </p>
        
            <br>
            <label class="label">password</label> <br>
            <input password="password" type="password" placeholder="enter password" v-model="password">
          
        </div>
    </form>
    <br/><br/>
    <button @click="submitForm">submit</button>
  </div>
</template> -->

<template>
  <div>
    <HomePageHeader></HomePageHeader>
<HomePageBody></HomePageBody>
  </div>

</template>

<script>

import HomePageHeader from '@/components/HomePageHeader.vue';
import HomePageBody from '@/components/HomePageBody.vue';
export default {
  name: "HomePage",
  components: {
    HomePageHeader,
    HomePageBody
  },
};
</script>
