<script>
    import MainNavbar from './MainNavbar.vue';
    import MainComics from './MainComics.vue';
    export default{
        name: 'MainApp',
        components: {
            MainNavbar,
            MainComics
        }
    }
</script>

<template>
    <main>
        <MainComics />
        <MainNavbar />
    </main>
</template>

<style lang="scss" scoped>
</style>
