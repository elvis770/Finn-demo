<template>
  <div class="home">
   
    <router-link to="/work">
      <div class="text">
        <p>
          FINNSTATIC
        </p>
      </div>
    </router-link>
      
   
    
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';


export default {
  name: 'HomeView',
  
};
</script>

<style lang="scss">
*{
  margin: 0;
  padding: 0px;
  text-decoration: none;
  background-color: #000;
  color: #d3d3d3;

  
  
  .text{
    padding-top: 250px;
    
    text-align: center;
    font-size: 50px;

  }
}



</style>
