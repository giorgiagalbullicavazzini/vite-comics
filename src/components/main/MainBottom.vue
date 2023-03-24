<script>
export default {
    name: 'MainBottom',
    data() {
        return {
            buttons: [
                {
                    image: 'buy-comics-digital-comics.png',
                    text: 'Digital Comics'
                },
                {
                    image: 'buy-comics-merchandise.png',
                    text: 'DC Merchandise'
                },
                {
                    image: 'buy-comics-subscriptions.png',
                    text: 'Subscription'
                },
                {
                    image: 'buy-comics-shop-locator.png',
                    text: 'Comic Shop Locator'
                },
                {
                    image: 'buy-dc-power-visa.svg',
                    text: 'DC Power VISA'
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
    <div id="main-bottom">
        <div class="container">
            <div v-for="button in buttons" class="button">
                <div class="image">
                    <img :src="getImagePath(`../../assets/img/${button.image}`)" :alt="button.text">
                </div>
                <div class="text"><a href="#">{{ button.text }}</a></div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../../assets/styles/partials/variables';

#main-bottom {
    background-color: variables.$brand-color;

    .container {
        align-items: center;
        display: flex;
        justify-content: center;
        padding: 3.125rem 0;

        .button {
            align-items: center;
            display: flex;
            margin: 0 1.5625rem;

            .image {
                margin-right: .625rem;
                width: variables.$shop-icons;

                img {
                    max-height: variables.$shop-icons;
                    object-fit: contain;
                }
            }

            .text {
                text-transform: uppercase;

                a {
                    color: variables.$main-color;
                }
            }
        }
    }
}
</style>