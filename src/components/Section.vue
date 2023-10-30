<template>
<div class="section">
    <div class="section-container">
        <div class="section-one">
            <p class="wrap">Steps</p>
            <div class="section-wrap">
                <img 
                src="https://cdn2.iconfinder.com/data/icons/thesquid-ink-40-free-flat-icon-pack/64/nike-dunk-512.png" alt="">
                <p class="figure">
                    500
                </p>
            </div>
            <P class="fig">
                Goal: <p> 10,000 steps</p>
            </P>
        </div>

        
    </div>

    
</div>
</template>

<script lang="ts">
export default {
    name:'SectionView'
}

</script>

<style scoped lang="scss">
*{
    margin: 0;
    padding: 0;
    background-color: #151515;
    border-radius: 5px;

    .section-container{

        padding: 20px;
        margin: 10px;
        display: flex;
        align-items:start;
        justify-content: space-between
    }
    .section-container .wrap{
        
        padding-bottom: 10px;
    }
    .section-container .section-wrap{
        display: flex;
        align-items: center;
        gap:var(--gap, 0.5rem);
    }

    .section-container img{
        height: 20px;
    }

    .section-container .fig{
        display: flex;
        align-items: center;
    }
    
}
</style>