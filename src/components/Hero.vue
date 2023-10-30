<template>
    <div class="hero">
        <h3 class="head">
            Daily Update
        </h3>
        <p class="little">
            Edit
        </p>
    </div>
</template>

<script>

export default {
    name:'HeroView' 
}
</script>

<style lang="scss">
*{
    margin: 0;
    padding: 0;

    .hero{
        margin: 0;
        padding: 10px;

        display: flex;
        align-items: center;
        justify-content: space-between;
    }
    .hero .head{
        padding: 5px;
    }
    .hero .little{
        padding: 5px;
        font-size: 10px;
        color: #87c1ff;

        border: 1px solid ;
        border-radius: 7px;
        background: #0000;
        
    }
}
</style>