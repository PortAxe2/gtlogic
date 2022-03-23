<template>
    <header>
        <div class="headerDiv">
            <img class="headerDiv-icon" src="../assets/6082ab3d5ebc506ef5c93c03_logo-gtlogic-min.png" alt="gtlogic logo">
            <div class="headerDiv-links">
                <p @click="scrollToElement('skillsDivId')" class="headerDiv-link" >Skills</p>
                <p @click="scrollToElement('portfolioDivId')" class="headerDiv-link" >Portfolio</p>
                <p @click="scrollToElement('incentiveListId')" class="headerDiv-link" >Incentive</p>
            </div>
        </div>
    </header>
</template>

<style scoped>
@import '../assets/style/header.css';
</style>

<script>
export default {
    methods: {
        scrollToElement(targetDivID) {
            window.scrollTo({
                top:
                document.getElementById(targetDivID).getBoundingClientRect().top
                - document.body.getBoundingClientRect().top - 100,
                behavior: 'smooth'
            })
            
        }
    }
}
</script>