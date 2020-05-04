<template>
    <div>
        <Masthead/>
        <h1>
            Hello World - Bird is on the fly!
        </h1>
        <h2>My projects</h2>
        <div v-for="project in githubProjects" :key="project.id">
            <h3> {{ project.name }}</h3>
            <a :href="project.html_url">{{ project.name }}</a>
            <p>{{ project.stargazers_count }}</p>
        </div>
    </div>
</template>

<script>

import { mapState } from 'vuex'
import Masthead from '~/components/Masthead.vue'

export default {
    computed: {
        ...mapState(["githubProjects"])
    },
    components: {
        Masthead
    }
    /*,
    mounted() {
        this.$store.dispatch("getGithubProjects");
    }*/   
}




</script>

<style lang="scss" scoped>

</style>