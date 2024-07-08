<script>
import facebookIcon from '../assets/img/footer-facebook.png'
import twitterIcon from '../assets/img/footer-twitter.png'
import youtubeIcon from '../assets/img/footer-youtube.png'
import pinterestIcon from '../assets/img/footer-pinterest.png'
import findusIcon from '../assets/img/footer-periscope.png'

    export default {
        name :'AppSocial',
        data() {
            return {
                socials:[
                    {
                        name: "facebook",
                        icon: facebookIcon,
                        url: "#",
                    },
                    {
                        name: "twitter",
                        icon: twitterIcon,
                        url: "#",
                    },
                    {
                        name: "youtube",
                        icon: youtubeIcon,
                        url: "#",
                    },
                    {
                        name: "pinterest",
                        icon: pinterestIcon,
                        url: "#",
                    },
                    {
                        name: "find-us",
                        icon: findusIcon,
                        url: "#",
                    },                  
                ],
            }
        }
    }
</script>

<template>
    <div class="component-container">
        <div class="container" >
            <div class="sign-up">
                <a href="#">SIGN-UP NOW!</a>
            </div>
            <div class="social-icons">
                <div class="follow">
                    <a href="#">FOLLOW US</a>
                </div>
                <div class="icons-container" >
                    <div :class="social.name" v-for="(social,index) in socials" :key="index"><a :href="social.url"><img :src="social.icon" alt=""></a></div>
                </div>
            </div>
        </div>
    </div>
</template>


<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;


.component-container {
    background-color: #303030;
    height: $navandborderheight;
}
.container {
    display: flex;
    height: 100%;
    justify-content: space-between
}
.sign-up {
    @include center(horizontal);
    
    a {
        color: white ;
        font-weight: bold;
        font-size: 18px;
        text-decoration: none;
        border: 3px solid $bluedc;
        padding: 10px
    }
}
.social-icons {
    @include center(horizontal);
    width: 31%;
}
.follow  {
    width: 30%;
    a {
        color: $bluedc;
        font-weight: bold;
        font-size: 18px;
        text-decoration: none;
    }
}
.icons-container {
    display: flex;
    gap: 6%;
    width: 70%;
    transform: scale(0.8);
}
</style>