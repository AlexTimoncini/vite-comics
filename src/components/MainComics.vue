<script>
    export default{
        name: 'MainComics'
    }
</script>

<template>
    <section id="comics">
        <div class="ivy_container">
            <h1 class="ivy_comics_title">current series</h1>
            <ul class="ivy_comic_list">
    
            </ul>
            <button class="ivy_load_more">load more</button>
        </div>
    </section>
</template>

<style lang="scss" scoped>
    @use '../styles/partials/mixins' as *;
    @use '../styles/partials/variables' as *;

    #comics{
        position: relative;
        padding: 2rem 0;
        background-color: $priBgColor;
        .ivy_comics_title{
            text-transform: uppercase;
            background-color: $logoColor;
            color: $priFontColor;
            padding: 1rem;
            position: absolute;
            top: 0;
            transform: translateY(-50%);
        }
    }
</style>
