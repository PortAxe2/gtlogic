<template>
    <p :class="technical ? 'techSkillsHeader' : 'creativeSkillsHeader'" id="skillsDivId">Techincal Skills</p>
    <div 
    :class="[
    'skills',
    technical ? 'skills-technical' : 'skills-creative']">
        <skill v-for="Skill in getSkillsList"
        :key="Skill.id"
        :skillImage="Skill.skillImage"
        skillType="tech"
        :skillName="Skill.skillName"
        :technical="technical"
        />
    </div>
</template>

<style scoped>
@import '../assets/style/skillslist.css';
</style>

<script>
import Skill from '../components/Skill.vue'

export default {
    components: { 
        Skill ,
    },

    props: {
        technical: Boolean,
    },

    methods: {
        
    },

    data() {
        return {
            techSkills: [
                {
                    'skillId': '1',
                    'skillName': 'JavaScript',
                    'skillImage': 'https://i.imgur.com/CSlHBl7.png'
                },
                {
                    'skillId': '2',
                    'skillName': 'HTML',
                    'skillImage': 'https://i.imgur.com/wkhas5F.png'
                },
                {
                    'skillId': '3',
                    'skillName': 'CSS',
                    'skillImage': 'https://i.imgur.com/ro0uf0k.png'
                },
                {
                    'skillId': '4',
                    'skillName': 'Vue.js',
                    'skillImage': 'https://i.imgur.com/gyw4IMw.png'
                },
                {
                    'skillId': '5',
                    'skillName': 'Firebase',
                    'skillImage': 'https://i.imgur.com/fLdYuGQ.png'
                },
                {
                    'skillId': '6',
                    'skillName': 'Node.js',
                    'skillImage': 'https://i.imgur.com/5t5QgOi.png'
                },
                {
                    'skillId': '7',
                    'skillName': 'MySQL',
                    'skillImage': 'https://i.imgur.com/LYisPCB.png'
                },
                {
                    'skillId': '8',
                    'skillName': 'Python',
                    'skillImage': 'https://i.imgur.com/M7StgOd.png'
                },
            ],

            creativeSkills: [
                {
                    'skillId': '0',
                    'skillName': 'Illustrator',
                    'skillImage': 'https://i.imgur.com/AO5YR7o.png'
                },
                {
                    'skillId': '10',
                    'skillName': 'Premiere',
                    'skillImage': 'https://i.imgur.com/77mwDVP.png'
                },
                {
                    'skillId': '11',
                    'skillName': 'After Effects',
                    'skillImage': 'https://i.imgur.com/pBHtNU6.png'
                },
                {
                    'skillId': '12',
                    'skillName': 'Lightroom',
                    'skillImage': 'https://i.imgur.com/QczDKF8.png'
                }
            ],
        }
    },

    computed: {
        getSkillsList() {
            return (this.technical ? this.techSkills : this.creativeSkills);
        }
    }


}
</script>