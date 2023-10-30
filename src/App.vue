<template>
  <nav>
    
  </nav>
  <router-view/>
</template>

<script lang="ts">
import axios from 'axios';

export default{
  data(){
    return{
      apiKey:''
    }
  }
}

</script>

<style lang="scss">
*{
  margin: 0;
  padding: 0;

  background-color: #28282B;
  font-family: "Inter","Helvetica Neue",Helvetica,Arial,sans-serif;

  &::selection{
    background: transparentize($color: #d3d3d3, $amount: 0);
  }
}
</style>
