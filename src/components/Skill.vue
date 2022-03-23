<template>
    <div :class="[
    'skill',
    technical ? 'skill-technical' : 'skill-creative']">
        <img class="skillImage" :src="skillImage" alt="skill image">
        <hr :class="[
        'skillSeperator',
        technical ? 'skillSeperator-technical' : 'skillSeperator-creative']">
        <p class="skillName">{{ skillName }}</p>
    </div>
</template>

<style scoped>
@import '../assets/style/skill.css';
</style>

<script>
export default {
    methods: {
        
    },
    props: {
        skillType: String,
        skillImage: String,
        skillName: String,
        technical: Boolean,
    },
}
</script>