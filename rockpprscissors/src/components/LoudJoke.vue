<template>
    <div>
       <h3>{{ joke }}</h3>
    </div>
</template>

<script>
    export default {
        name: "loud-joke",
        computed: {
            joke() {
                return this.$store.getters.loud;
            }
        },
    }
</script>

<style lang="scss" scoped>

</style>