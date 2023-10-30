<template>
    <div class="second">
        <div class="second-wrap">
            <p>
                Exercise
            </p>
            <img 
                src="https://cdn0.iconfinder.com/data/icons/flat-design-database-set-6/24/button-circle-add-512.png" alt="">
        </div>
        <div class="sub-second">
            <img 
                src="https://cdn3.iconfinder.com/data/icons/nature-emoji/50/Fire-512.png" alt="">
            <p>
                1 cal
            </p>
        </div>
        <div class="sub-second">
            <img 
                src="https://cdn4.iconfinder.com/data/icons/buno-info-signs/32/__clock_time_watch-512.png" alt="">
            <p>
                00:00 hr
            </p>
        </div>
    </div>
    </template>
    
    <script>
    export default {
        name:'SecondView'
    }
    
    </script>
    
    <style scoped lang="scss">
    *{
        margin: 0;
        padding: 0;
        background-color: #151515;
        border-radius: 5px;

        .second img{
            height: 20px;
        }

        .second-wrap{
            display: flex;
            align-items: center;
            justify-content: space-between;

            padding: 15px;
        }

        .sub-second{
            display: flex;
            align-items: center;

            padding-left: 15px;
            padding-bottom:8px ;
            gap:var(--gap, 0.5rem);
        }
    }
    </style>
    