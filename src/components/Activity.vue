<template>
    <div class="activity">
        <div class="activity-container">
            <div class="act-wrap">
                <h2>
                    Weekly Schedule
                </h2>
            </div>
            <div class="wrap-one">
                <p>
                    Today
                </p>
                 <p class="little">
                     Edit
                </p>
            </div>
           <div class="wrap-two">
                <div>
                    
                    <img class="image"
                    src="https://cdn3.iconfinder.com/data/icons/home-house-building/778/apartment_building_home_house_townhome-512.png" alt="+">
                </div>
                <div>
                    <p> ---</p>
                </div>
                <div> 
                   
                    <img class="image"
                    src="https://cdn4.iconfinder.com/data/icons/luna-bicycle/512/City_bike_sepeda_jengki__keranjang-512.png" alt="">
                </div>
                <div>
                    <p> ---</p>
                </div>
                <div>
                    
                    <img class="image"
                    src="https://cdn2.iconfinder.com/data/icons/building-219/66/12-512.png" alt="+">
                </div>
                <div>
                    <p> ---</p>
                </div>
                <div>
                    
                    <img class="image"
                    src="https://cdn4.iconfinder.com/data/icons/luna-bicycle/512/City_bike_sepeda_jengki__keranjang-512.png" alt="+">
                </div>
                <div>
                    <p> ---</p>
                </div>
                <div>
                    
                    <img class="image"
                    src="https://cdn0.iconfinder.com/data/icons/fitness-gym-6/56/08_dumbbell-512.png" alt="+">
                </div>
                <div>
                    <p> ---</p>
                </div>
                <div>
                   
                    <img class="image"
                    src="https://cdn3.iconfinder.com/data/icons/home-house-building/778/apartment_building_home_house_townhome-512.png" alt="">
                </div>
           </div>
           <div class="wrap-three">
            <button class="history-button">History</button>
           </div>
            
        </div>
    </div>
    </template>
    
    <script lang="ts">
    export default {
        name:'ActivityView'
    }
    
    </script>
    
    <style scoped lang="scss">
    *{
        margin: 0;
        padding: 0;
        background-color: #151515;
        border-radius: 5px;

        .activity-container{
            padding: 20px;
            margin: 10px;
        }
        .activity-container h2{
            text-align: center;
        }
        .activity-container .wrap-one{
            display: flex;
            align-items: center;
            justify-content: space-between;

            padding-top: 20px;
        }

        .activity-container .little{
        padding: 5px;
        font-size: 10px;
        color: #87c1ff;

        border: 1px solid ;
        border-radius: 7px;
        background: #0000;
        }
        .activity-container .wrap-two{
            text-align: center;
            display: flex;
            align-items: center;

            padding: 25px;
        }

        .activity-container .image{
            height: 20px;
            padding-left: 10px;
        }
        .activity-container .wrap-three{
            text-align: center;
        }
        .activity-container .history-button{
            background-color: #87c1ff;
            color: #151515;
            border: none;
            border-radius: 20px;
            padding: 10px 20px;
            margin-left: 10px;
            cursor: pointer;
            font-size: 16px;
        }

    }
    </style>