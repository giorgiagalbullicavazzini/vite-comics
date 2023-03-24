<script>
export default {
    name: 'Socials',
    data() {
        return {
            socials: [
                {
                    social: 'Facebook',
                    image: 'footer-facebook.png',
                },
                {
                    social: 'Twitter',
                    image: 'footer-twitter.png',
                },
                {
                    social: 'YouTube',
                    image: 'footer-youtube.png',
                },
                {
                    social: 'Pinterest',
                    image: 'footer-pinterest.png',
                },
                {
                    social: 'Periscope',
                    image: 'footer-periscope.png',
                }
            ]
        }
    },
    methods: {
        getImagePath: function (imgPath) {
            return new URL(imgPath, import.meta.url).href;
        }
    }
}
</script>

<template>
    <div id="socials">
        <h3>Follow us</h3>
        <div class="buttons">
            <div v-for="social in socials" class="button">
                <a href="#">
                    <img :src="getImagePath(`../../assets/img/${social.image}`)" :alt="social.social">
                </a>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../../assets/styles/partials/variables';

#socials {
    align-items: center;
    display: flex;

    h3 {
        color: variables.$brand-color;
        margin-right: .3125rem;
        text-transform: uppercase;
    }

    .buttons {
        display: flex;

        .button {
            aspect-ratio: 1;
            margin-left: .9375rem;
            width: 1.875rem;
        }
    }
}
</style>