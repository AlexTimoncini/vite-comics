<script>
    export default{
        name: 'FooterNavList',
        data(){
            return{
                navbarLists: [
                    {
                        title: 'dc comics',
                        navbarList: [
                            {
                                name: 'Characters',
                                link: '#'
                            },
                            {
                                name: 'Comics',
                                link: '#'
                            },
                            {
                                name: 'Movies',
                                link: '#'
                            },
                            {
                                name: 'TV',
                                link: '#'
                            },
                            {
                                name: 'Games',
                                link: '#'
                            },
                            {
                                name: 'Videos',
                                link: '#'
                            },
                            {
                                name: 'News',
                                link: '#'
                            },
                        ]
                    },
                    {
                        title: 'shop',
                        navbarList: [
                            {
                                name: 'Shop DC',
                                link: '#'
                            },
                            {
                                name: 'Shop DC Collectibles',
                                link: '#'
                            },
                        ]
                    },
                    {
                        title: 'dc',
                        navbarList: [
                            {
                                name: 'Term Of Use',
                                link: '#'
                            },
                            {
                                name: 'Privacy policy (New)',
                                link: '#'
                            },
                            {
                                name: 'Ad Choices',
                                link: '#'
                            },
                            {
                                name: 'Advertising',
                                link: '#'
                            },
                            {
                                name: 'Jobs',
                                link: '#'
                            },
                            {
                                name: 'Subscriptions',
                                link: '#'
                            },
                            {
                                name: 'Talent Workshops',
                                link: '#'
                            },
                            {
                                name: 'CPSC Certificates',
                                link: '#'
                            },
                            {
                                name: 'Ratings',
                                link: '#'
                            },
                            {
                                name: 'Shop Help',
                                link: '#'
                            },
                            {
                                name: 'Contact Us',
                                link: '#'
                            },
                        ]
                    },
                    {
                        title: 'sites',
                        navbarList: [
                            {
                                name: 'DC',
                                link: '#'
                            },
                            {
                                name: 'MAD Magazines',
                                link: '#'
                            },
                            {
                                name: 'DC Kids',
                                link: '#'
                            },
                            {
                                name: 'DC Universe',
                                link: '#'
                            },
                            {
                                name: 'DC Power Visa',
                                link: '#'
                            },
                        ]
                    },
                ]
            }
        }
    }
</script>

<template>
    <nav>
        <div class="ivy_container">
            <div class="ivy_navbar_lists">
                <ul class="ivy_navbar_list" v-for="list in navbarLists">
                    <h1 class="ivy_navbar_title">{{ list.title }}</h1>
                    <li class="ivy_navbar_item" v-for="item in list.navbarList">
                        <a :href="item.link">{{ item.name }}</a>
                    </li>
                </ul>
            </div>
            <div class="ivy_big_logo">
                <img src="../assets/img/dc-logo-bg.png" alt="dc logo">
            </div>
        </div>
    </nav>
</template>

<style lang="scss" scoped>
    @use '../styles/partials/mixins' as *;
    @use '../styles/partials/variables' as *;
    nav{
        background-image: url('../assets/img/footer-bg.jpg');
        overflow: hidden;
        height: 450px;
        .ivy_container{
            @include flex(row, space-between, center, nowrap);
            height: 100%;
            .ivy_navbar_lists{
                @include flex(column, flex-start, flex-start, wrap);
                height: 100%;
                padding-top: 2rem;
                column-gap: 2rem;
                z-index: 2;
                .ivy_navbar_list{
                    margin-bottom: 2rem;
                    .ivy_navbar_title{
                        color: $priFontColor;
                        text-transform: uppercase;
                        font-size: 1.3rem;
                        margin-bottom: 1rem;
                    }
                    .ivy_navbar_item{
                        padding: 0.25rem 0;

                        a{
                            color: $secFontColor
                        }
                    }
                }
            }
        }

    }
</style>