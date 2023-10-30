<template>
    <div class="window">
        <div class="window-container">
            <div class="parent">
                <img class="image-one"
                src="https://cdn3.iconfinder.com/data/icons/leto-user-group/64/__user_person_profile-512.png" alt="">
                <img class="image-two"
                src="https://cdn0.iconfinder.com/data/icons/zondicons/20/camera-512.png" alt="">
            </div>
            <div class="user-container">
                
                <p class="user">
                    Name: <b>Finn </b>
                </p>
                <p class="user">
                    Age: <b> 21</b>
                </p>
                <p class="user">
                    Weight: <b> 77kg</b>
                </p>
                <p class="user">
                    height: <b> 183cm</b>
                </p>

            </div>

            <div class="edit">
                <router-link to="/">
                    <button class="edit-button">Edit Profile</button>
                </router-link>
                
            </div>

        </div>
        
    </div>

    
        
    </template>
    
    <script>
    export default {
        name:'WindowView'
    } 
    
    </script>
    
    <style scoped lang="scss">
    *{
        margin: 0;
        padding: 0;


        
        background-color: #151515;
        border-radius: 5px;


        .window .window-container{
            text-align: center;
            padding: 10px;
        }
        .window .parent{
            position: relative;
            top: 0;
            bottom: 0;
        }
        .window .image-one{
            position: relative;
            height: 60px;
            top: 0;
            bottom: 0;
            padding-top: 40px;
        }
        .window .image-two {
            position: absolute;
            height: 18px;
            top: 78px;
            left: 195px;
            
        }
        .window .user-container{
            text-align: start;
            color: #d3d3d3;
        }

        .window .user{
            font-size: 10px;
        }
        .window .user b{
            font-size: 20px;
        } 

        .window .edit{
            padding: 20px 20px 20px 10px;
        }
        .window .edit-button{
            background-color: #87c1ff;
            color: #151515;
            border: none;
            border-radius: 20px;
            padding: 10px 20px;
            margin-left: 10px;
            cursor: pointer;
            font-size: 16px;
        }

        .window .edit-button:hover{
            background-color: #000080;
        }
        
    }
    </style>