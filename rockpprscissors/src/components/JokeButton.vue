<template>
    <div>
    <button @click="newJoke">Click for a new Joke!</button>
    </div>
</template>

<script>
    export default {
        name: "joke-button",
        methods: {
            newJoke() {
                this.$store.dispatch("newJoke")
            }
        },
    }
</script>

<style lang="scss" scoped>

</style>