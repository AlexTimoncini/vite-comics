<script>
    export default{
        name: 'Mainnavbar',
        data(){
            return{
                navItems: [
                    {
                        name: 'digital comics',
                        icon: '/src/assets/img/buy-comics-digital-comics.png',
                        link: '#'
                    },
                    {
                        name: 'dc merchandise',
                        icon: '/src/assets/img/buy-comics-merchandise.png',
                        link: '#'
                    },
                    {
                        name: 'subscription',
                        icon: '/src/assets/img/buy-comics-subscriptions.png',
                        link: '#'
                    },
                    {
                        name: 'comic shop locator',
                        icon: '/src/assets/img/buy-comics-shop-locator.png',
                        link: '#'
                    },
                    {
                        name: 'dc power visa',
                        icon: '/src/assets/img/buy-dc-power-visa.svg',
                        link: '#'
                    }
                ]
            }
        }
    }
</script>

<template>
    <nav>
        <div class="ivy_container">
            <ul class="ivy_nav_items">
                <li class="ivy_nav_item" v-for="item in navItems">
                    <a :href="item.link">
                        <img :src="item.icon" :alt="item.name">
                        {{ item.name }}
                    </a>
                </li>
            </ul>
        </div>
    </nav>
</template>

<style lang="scss" scoped>
    @use '../styles/partials/mixins' as *;
    @use '../styles/partials/variables' as *;
    nav{
        background-color: $logoColor;
        padding: 3rem 0;
        .ivy_nav_items{
            @include flex();
            column-gap: 1.5rem;
            .ivy_nav_item a{
                text-transform: uppercase;
                color: $priFontColor;
                @include flex();
                
                img{
                    height: 80px;
                    max-width: 80px;
                    display: block;
                    margin: 0 1rem;
                }
            }
        }
    }
</style>
