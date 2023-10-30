<template>
    <div class="slides">
         <div class="slide-one">

            <H3 class="text-one">
                Calories
            </H3>

            <h4 class="text-two">
                Remaining = Goal - Food + Exercise
            </h4>

            <div class="wrapper">

                <div class="circle">
                    2.000   
                </div>

                <div class="list">

                    <div class="list-one">
                        <img
                        src="https://cdn4.iconfinder.com/data/icons/fast-food-113/52/20-512.png" alt="">
                        <ul>
                            <li class="one">
                                Water
                            </li>
                            <li>
                                1L
                            </li>
                        </ul>
                    </div>

                    <div class="list-one">
                        <img
                        src="https://cdn3.iconfinder.com/data/icons/webuy-restaurant/48/Fork_Spoon-1024.png" alt="">
                        <ul>
                            <li class="one">
                                Food
                            </li>
                            <li>
                                0
                            </li>
                        </ul>
                    </div>

                    <div class="list-one">

                        <img
                        src="https://cdn4.iconfinder.com/data/icons/energy-3/63/flame-512.png" alt="">
                        <ul>
                            <li class="one">
                            Exercise
                            </li>
                            <li>
                                1
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
         </div>

         
    </div>

   
    
   
</template>

<script lang="ts">

export default {
    name:'SlideView',
    
}


</script>

<style scoped lang="scss">
*{
    margin: 1.5px;
    padding: 0;
    background-color: #151515;
    border-radius: 5px;

    .slides{
        display: inline-block;
        padding: 10px;
        
        
        border-radius: 7px;
        
    }

    .slides .slide-one{
        padding: 10px;
    }

    .slides H3{
        font-size: 30px;
    }

    .slides h4{
        font-size: 10px;
    }

    .slides .wrapper{
        display: flex;
        align-items: center;
        justify-content: space-between;
        padding: 10px;
        gap:var(--gap, 5.5rem);
    }
    .slides .circle{
        border-radius: 50%;
        width: 34px;
        height: 34px;
        padding: 50px;
        
        border: 1px solid #87c1ff;
        color: #87c1ff;
        text-align: center;
    }

    .slides .list-one{
        display: flex;
        align-items: center;
    }

    .slides img{
        height: 20px;
    }

    .slides ul{
        list-style: none;
        font-size: 15px;
    }

    .slides ul .one{
        font-weight: 10;
    }

}
</style>