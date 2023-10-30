<template>
    <div class="top">
        <div class="top-container">
            <div>
                <router-link to="/work">
                    <img class="photo"
                    src="https://cdn1.iconfinder.com/data/icons/interface-travel-and-environment/64/arrow-left-interface-1024.png" alt="">
                </router-link>
                    
            </div>
            <div class="top-text">
                <p>
                    Welcome Elvis!
                </p>
            </div>
            <div class="setting">
                <img class="photo"
                src="https://cdn4.iconfinder.com/data/icons/evil-icons-user-interface/64/setting-512.png" alt="">
            </div>
        </div>
    </div>
    </template>
    
    <script>
    export default {
        name:'TopView'
    }
    
    </script>
    
    <style scoped lang="scss">
    *{
        margin: 0;
        padding: 0;

        .top{
            padding: 5px;
            padding-bottom: 10px;
        }
        .top .top-container{
            display: flex;
            align-items: center;
            gap:var(--gap, 7.1rem);
        }
        .top .photo{
            height: 20px;
        }

        .top .top-text{
            text-align: center;
            color: #d3d3d3;
        }
    }
    </style>
    