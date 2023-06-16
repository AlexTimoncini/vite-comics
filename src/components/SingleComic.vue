<script>
    export default{
        name: 'SingleComic',
        props: {
            comicObj : Object,
        }
    }
</script>

<template>
    <li>
        <div class="ivy_thumb">
            <img :src="comicObj.thumb" :alt="comicObj.series">
        </div>
        <h2 class="ivy_comic_title">{{ comicObj.series }}</h2>
    </li>
</template>

<style lang="scss" scoped>
    @use '../styles/partials/variables' as *;
    .ivy_thumb{
        height: 300px;
        width: 100%;
        margin-bottom: 1rem;

        img{
            width: 100%;
            height: 100%;
            object-fit: cover;
            display: block;
        }
    }

    .ivy_comic_title{
        color: $priFontColor;
    }
</style>
