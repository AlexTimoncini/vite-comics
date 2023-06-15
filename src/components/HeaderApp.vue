<script>
    import HeaderNavbar from './HeaderNavbar.vue';
    import HeaderJumbo from './HeaderJumbo.vue';
    export default{
        name: 'HeaderApp',
        components: {
            HeaderNavbar,
            HeaderJumbo,
        }
    }
</script>

<template>
    <header>
        <HeaderNavbar />
        <HeaderJumbo />
    </header>
</template>

<style lang="scss" scoped>
</style>
