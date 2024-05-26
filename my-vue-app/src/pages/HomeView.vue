<script>
export default {
    methods:{
        goToabout() {
            this.$router.push ('/about')
        },
    },
}
</script>

<template>
    <h2> homeView</h2>
    <button @click="goToAbout"> Go to about</button>
</template>