<script>
    import FooterNavList from './FooterNavList.vue';
    import FooterContacts from './FooterContacts.vue';
    export default{
        name: 'FooterApp',
        components: {
            FooterNavList,
            FooterContacts
        }
    }
</script>

<template>
    <footer>
        <FooterNavList />
        <FooterContacts />
    </footer>
</template>

<style lang="scss" scoped>
</style>
