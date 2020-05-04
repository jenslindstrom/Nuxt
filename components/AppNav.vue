<template>
    <div>
        <ul>
            <li>
                <nuxt-link exact to="/">Home</nuxt-link>
            </li>
            <li>
                <nuxt-link exact to="projects">Projects link</nuxt-link>
            </li>
        </ul>
    </div>
</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>
    div {
        display: flex;
        justify-content: center;
        width: 100vw;
        height: 100%;
        ul {
            padding-left: 0;
            li {
                display: inline-block;
            }
        }

    }
</style>