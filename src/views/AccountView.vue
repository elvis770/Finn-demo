<template>
    <div class="account">
        <Top/>
        <Window/>
    </div>
    </template>
    
    <script lang="ts">
    import { defineComponent } from 'vue';
    import Top from '@/components/Top.vue'
    import Window from '@/components/Window.vue'

    export default {
        name:'AccountView',
        components: {
            Top,
            Window
        }
        
    }
    
    </script>
    
    <style scoped lang="scss">
    
    </style>