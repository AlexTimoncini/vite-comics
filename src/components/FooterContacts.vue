<script>
    export default{
        name: 'FooterContacts',
        data(){
            return{
                socialMedias: [
                    {
                        name: 'Facebook',
                        icon: '/src/assets/img/footer-facebook.png',
                        link: '#',
                    },
                    {
                        name: 'Twitter',
                        icon: '/src/assets/img/footer-twitter.png',
                        link: '#',
                    },                    {
                        name: 'You Tube',
                        icon: '/src/assets/img/footer-youtube.png',
                        link: '#',
                    },
                    {
                        name: 'Pinteres',
                        icon: '/src/assets/img/footer-pinterest.png',
                        link: '#',
                    },
                    {
                        name: 'Periscope',
                        icon: '/src/assets/img/footer-periscope.png',
                        link: '#',
                    }
                ]
            }
        }
    }
</script>

<template>
    <section id="footerContacts">
        <div class="ivy_container">
            <button class="ivy_signup">Sign-up now!</button>
            <ul class="ivy_social_box">
                <li class="ivy_social_header">Follow Us</li>
                <li class="ivy_social_media" v-for="a in socialMedias">
                    <a :href="a.link">
                        <img :src="a.icon" :alt="a.name + ' logo'">
                    </a>
                </li>
            </ul>
        </div>

    </section>
</template>

<style lang="scss" scoped>
    @use '../styles/partials/mixins' as *;
    @use '../styles/partials/variables' as *;

    #footerContacts{
        background-color: $secBgColor;

        .ivy_container{
            @include flex(row, space-between, center, nowrap);
            padding: 2rem 0;
            .ivy_signup{
                border: 3px solid $logoColor;
                background: none;
                padding: 1rem;
                text-transform: uppercase;
                font-weight: bold;
                color: $priFontColor;
            }

            .ivy_social_box{
                @include flex();
                column-gap: 1rem;
                .ivy_social_header{
                    text-transform: uppercase;
                    color: $logoColor;
                    font-weight: bold;
                    font-size: 1.2rem;
                    margin-right: 0.5rem;
                }
            }
        }
    }
</style>
