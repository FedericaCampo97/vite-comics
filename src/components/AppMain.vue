<script>
import cards from '../js/arrayCards';
import cardElement from './CardElement.vue';

const arrayMain = [
    {
        name: 'DIGITAL COMICS',
        image: 'src/assets/img/buy-comics-digital-comics.png'
    },
    {
        name: 'DC MERCHANDISE',
        image: 'src/assets/img/buy-comics-merchandise.png'
    },
    {
        name: 'SUBSCRIPTION',
        image: 'src/assets/img/buy-comics-subscriptions.png'
    },
    {
        name: 'COMIC SHOP LOCATOR',
        image: 'src/assets/img/buy-comics-shop-locator.png'
    },
    {
        name: 'DC POWER VISA',
        image: 'src/assets/img/buy-dc-power-visa.svg'
    },
]
export default {
    name: 'AppMain',
    components: {
        cardElement
    },
    data() {
        return {
            arrayMain,
            cards,
        }
    }
}
</script>

<template>
    <div class="block_jumbo bg-black">
        <button class="current_button"><strong>CURRENT SERIES</strong></button>
    </div>

    <div class="card_comics text-center">
        <div class="container d-flex flex-wrap pt-5 pb-3">
            <cardElement v-for="element in cards" class="card_element" :thumb="element.thumb" :title="element.series" />
        </div>
        <button class="btn btn-primary mt-3 mb-3 custom_button"><strong>LOAD MORE</strong></button>
    </div>
    <div class="block_menu">
        <div class="container">
            <ul class="nav justify-content-center p-5">
                <li class="nav-item d-flex align-items-center" style="width:20%" v-for="card in arrayMain">
                    <img :src="card.image" alt="" class="tag-img">
                    <span class="nav-link text-white" href="#">
                        {{ card.name }}
                    </span>
                </li>
            </ul>
        </div>
    </div>
</template>

<style scoped></style>
