<template>
    <div class="footer">
        <nav>
            <div class="footer-wrap">
                <router-link to="/work">
                    <img 
                    src="https://cdn2.iconfinder.com/data/icons/wireframe-1/128/embedded_tiles_design_wireframe_layout_dashboard-512.png" alt="">
                </router-link>
                <p class="text">
                    Dashboard
                </p>
            </div>
            <div class="footer-wrap">
                <router-link to="/">
                    <img 
                    src="https://cdn0.iconfinder.com/data/icons/ui-and-ux-outline-blue/64/newsfeed_ui_ux_basic_website-512.png" alt="">
                </router-link>
                <p class="text">
                    NewsFeed
                </p>
            </div>
            <div class="footer-wrap">
                <router-link to="/more">
                    <img 
                    src="https://cdn1.iconfinder.com/data/icons/essential-ui-v-1/64/1_more_horizontal_user_interface-512.png" alt="">
                </router-link>
                <p class="text">
                    More
                </p>
            </div>

        </nav>
        
    </div>

</template>

<script>
export default{
    name: 'FooterView'
}
</script>

<style scoped lang="scss">
*{
    margin: 0;
    padding: 0;

    .footer {
        position: fixed;
        bottom: 0;
        left: 0;
        width: 100%;
        height: 70px;

    }
    nav{
        padding: 15px;
        display: flex;
        align-items: center;
        justify-content: space-between;
    }
    .footer .footer-wrap{
        display: inline-block;
    }
    .footer img{
        height: 20px;
    }
    .footer p{
        font-size: 10px;
    }

}
</style>