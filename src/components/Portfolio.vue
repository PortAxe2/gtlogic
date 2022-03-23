<template>
    <div class="portfolio" id="portfolioDivId">
        <p class="portfolioHeader">PORTFOLIO</p>
        <div class="portSectionList">
            <a class="portSectionAnchor" href="https://lacelaboratory.com/pages/thelaboratory">
                <div class="portSection portSection-lace">
                    <img class="portSectionLogo" src="https://i.imgur.com/hIlSHfT.png" alt="">
                </div>
            </a>
            <a class="portSectionAnchor" href="https://www.haskapa.com/pages/haskapa-new-campaign">
                <div class="portSection portSection-haskapa">
                    <img class="portSectionLogo" src="https://i.imgur.com/QFfNpT9.png" alt="">
                </div>
            </a>
            <a class="portSectionAnchor" href="http://holexp.com/">
                <div class="portSection portSection-holexp">
                    <img class="portSectionLogo" src="https://i.imgur.com/CdvrdUd.png" alt="">
                </div>
            </a>
        </div>
        <spotify-resume />
    </div>
</template>

<style scoped>
@import '../assets/style/portfolio.css';
</style>

<script>
import SpotifyResume from '../components/SpotifyResume.vue'

export default {
    components: {
        SpotifyResume ,
    },

    methods: {
        goToLink(linkUrl) {
            window.open(linkUrl, '_blank');
        }
    }
}
</script>