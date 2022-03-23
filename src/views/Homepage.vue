<template>
    <header-component />
    <body>
        <intro-div />
        <github-linkedin />
        <skills-list :technical="true" />
        <skills-list :technical="false" />
        <portfolio />
        <incentive />
    </body>
    <footer>
        <footer-component />
    </footer>

</template>

<style scoped>
@import '../assets/style/homepage.css';
</style>

<script>
import HeaderComponent from '../components/HeaderComponent.vue'
import IntroDiv        from '../components/IntroDiv.vue'
import GithubLinkedin  from '../components/GithubLinkedin.vue'
import SkillsList      from '../components/SkillsList.vue'
import Portfolio       from '../components/Portfolio.vue'
import Incentive       from '../components/Incentive.vue'
import FooterComponent from '../components/FooterComponent.vue'

export default {
    components: {
        HeaderComponent,
        IntroDiv ,
        GithubLinkedin ,
        SkillsList ,
        Portfolio ,
        Incentive ,
        FooterComponent ,
    },

    methods: {
        
    },

    data() {
        return {

        }
    },
}
</script>