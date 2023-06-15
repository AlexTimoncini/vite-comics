<script>
    export default{
        name: 'HeaderNavbar',
        data(){
            return{
                navbarItems: [
                    {
                        name: 'Characters',
                        link: '#',
                        active: false
                    },
                    {
                        name: 'Comics',
                        link: '#',
                        active: true
                    },
                    {
                        name: 'Movies',
                        link: '#',
                        active: false
                    },
                    {
                        name: 'Tv',
                        link: '#',
                        active: false
                    },
                    {
                        name: 'Games',
                        link: '#',
                        active: false
                    },
                    {
                        name: 'Collectibles',
                        link: '#',
                        active: false
                    },
                    {
                        name: 'Videos',
                        link: '#',
                        active: false
                    },
                    {
                        name: 'Fnas',
                        link: '#',
                        active: false
                    },
                    {
                        name: 'News',
                        link: '#',
                        active: false
                    },
                    {
                        name: 'Shop',
                        link: '#',
                        active: false
                    },
                ]
            }
        }
    }
</script>

<template>
    <nav>
        <div class="ivy_container">
            <div class="ivy_logo_box">
                <img src="../assets/img/dc-logo.png" alt="dc logo">
            </div>
            <ul class="ivy_nav_items">
                <li class="ivy_item" v-for="item in navbarItems">
                    <a :href="item.link">{{ item.name }}</a>
                </li>
            </ul>
        </div>
    </nav>
</template>

<style lang="scss" scoped>
    @use '../styles/partials/mixins' as *;
    @use '../styles/partials/variables' as *;
    nav{
        background-color: $priFontColor;
        padding: 2rem 0;
        .ivy_container{
            @include flex(row, space-between, center, nowrap);
            .ivy_nav_items{
                @include flex();
                height: 100%;
                .ivy_item a{
                    font-size: 1.1rem;
                    color: $secFontColor;
                    text-transform: uppercase;
                    font-weight: bold;
                    margin: 0 1rem;
                }
            }
        }
    }
</style>
