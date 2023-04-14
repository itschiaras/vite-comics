<template>
    <div id="footer-bottom">
        <div class="container h-100 d-flex align-items-center justify-content-between">
            <button class="text-uppercase"> sign-up now!</button>
            <div>
                <ul class="d-flex gap-3">
                    <li class="d-flex align-items-center"><a href="" class="text-uppercase">follow us</a></li>
                    <li><a href=""><img src="../assets/images/footer-facebook.png" alt=""></a></li>
                    <li><a href=""><img src="../assets/images/footer-periscope.png" alt=""></a></li>
                    <li><a href=""><img src="../assets/images/footer-pinterest.png" alt=""></a></li>
                    <li><a href=""><img src="../assets/images/footer-twitter.png" alt=""></a></li>
                    <li><a href=""><img src="../assets/images/footer-youtube.png" alt=""></a></li>
                </ul>
            </div>
        </div>
        
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style lang="scss" scoped>
    #footer-bottom {
        height: 80px;
        background-color: #303030;

        button {
            background-color: transparent;
            color: white;
            border-color: #0282f9;
            padding: .4rem;
            font-weight: 600;
        }

        ul {
            margin-bottom: 0;
        }

        ul a {
            text-decoration: none;
            color: #0282f9;
            font-weight: 700;
        }
    }
</style>