<template>
  <div class="navbar">
    <nav>
      <div class="navbar-item">
        <router-link to="/account">
          <img class="user"
          src="https://cdn3.iconfinder.com/data/icons/leto-user-group/64/__user_person_profile-512.png" alt="">
        </router-link>
      </div>
      
      <div class="navbar-item">
        <router-link to="/work">
          <h3 class="write">
            FINNTASTIC
          </h3>
        </router-link>
      </div>
      
      <div class="navbar-item">
        <img class="user"
        src="https://cdn4.iconfinder.com/data/icons/buno-audio/32/bell_notification_ring-512.png" alt="">
      </div>
      
    </nav>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default {
  name: 'NavbarView'
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
*{
  margin: 0;
  padding: 0;
  .navbar{
    position: fixed;
    top: 0;
    bottom: 0;
    width: 100%;
    height: 0;
  }

  nav{
    padding: 15px;
    
    display: flex;
    align-items: center;
    justify-content: space-between;
  }
  nav .user{
    height: 20px;
  }
  nav .write{
    font-size: 20px;
    color: #fff;
  }
}
</style>
