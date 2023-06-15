<script>
    export default{
        name: 'HeaderJumbo',
    }
</script>

<template>
    <section id="jumbotron">
        <div class="ivy_container">
            <h1> -- Content goes here --</h1>
        </div>
    </section>
</template>

<style lang="scss" scoped>
    @use '../styles/partials/variables' as *;
    #jumbotron{
        background-color: $priBgColor;
        color: $priFontColor;
        h1{
            padding: 4rem 0;
            font-size: 2rem;
        }
    }
</style>
