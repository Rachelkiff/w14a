<template>
    <div>
     <h3>{{ joke }}</h3>
    </div>
</template>

<script>
    export default {
        name: "normal-joke",
        computed: {
            joke() {
                return this.$store.state.joke;
            }
        },
    }
</script>

<style lang="scss" scoped>

</style>