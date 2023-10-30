<template>
    <div class="more">
        <div class="more-contents">
            <H3>
                More
            </H3>

            <router-link to="/account">
                <div class="icon-show">
                    <img class="icon"
                    src="https://cdn3.iconfinder.com/data/icons/leto-user-group/64/__user_person_profile-512.png" alt="">
                    <p>
                        Finn
                    </p>
                </div>
            </router-link>
            

        </div>
        
        <Footer/>
    </div>
    </template>
    
<script lang="ts">

import Footer from '@/components/Footer.vue'

    export default {
        name:'MoreView',
        components:{
           
            Footer
        }
    }
    
</script>
    
    <style scoped lang="scss">
    *{
        color: #d3d3d3;

        .more-contents{
            text-align: center;
            padding: 15px;
        }

        .more-contents .icon{
            height: 40px;
            padding-bottom: 0;
            margin-bottom: 0;
        }
        .more-contents p{
            padding-top: 0;
        }
    }
    </style>