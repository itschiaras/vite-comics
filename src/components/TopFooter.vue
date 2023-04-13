<template>
    <div id="footer-top">
        <div class="container">
            <div class="row">
                <div class="col pt-4">
                    <h4>{{ footerLinks[0].title }}</h4>
                    <ul>
                        <li v-for="link in footerLinks[0].links">
                            <a href="">{{ link.text }}</a>
                        </li>
                    </ul>
                    <h4>{{ footerLinks[1].title }}</h4>
                    <ul>
                        <li v-for="link in footerLinks[1].links">
                            <a href="">{{ link.text }}</a>
                        </li>
                    </ul>
                </div>
                <div class="col pt-4">
                    <h4>{{ footerLinks[2].title }}</h4>
                    <ul>
                        <li v-for="link in footerLinks[2].links">
                            <a href="">{{ link.text }}</a>
                        </li>
                    </ul>
                </div>
                <div class="col pt-4">
                    <h4>{{ footerLinks[3].title }}</h4>
                    <ul>
                        <li v-for="link in footerLinks[3].links">
                            <a href="">{{ link.text }}</a>
                        </li>
                    </ul>
                </div>
                <div class="col col-6 img-container">
                    
                </div>

            </div>

        </div>
    </div>
</template>

<script>
import { footerLinks } from '../data/data.js';
export default {
    name: 'FooterTop',
    data() {
        return {
            footerLinks: footerLinks
        }
    }
}
</script>

<style lang="scss" scoped>
#footer-top {
    background-image: url(../assets/images/footer-bg.jpg);
    height: 350px;
    color: white;
    overflow: hidden;
    

    h4 {
        text-transform: uppercase;
        margin-bottom: 0;
    }

    a {
        text-decoration: none;
        color: white;
    }
    .img-container {
        height: 350px;
        background-image: url(../assets/images/dc-logo-bg.png);
        background-size: cover;
        background-position: center;
    }
}
</style>