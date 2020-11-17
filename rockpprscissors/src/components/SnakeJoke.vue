<template>
    <div>
      <h3>{{ joke }}</h3>
    </div>
</template>

<script>
    export default {
        name: "snake-joke",
        computed: {
            joke() {
                return this.$store.getters.snake;
            }
        }
    }
</script>

<style lang="scss" scoped>

</style>