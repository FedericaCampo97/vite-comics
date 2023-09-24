<script setup>
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
</script>

<template>
    <div class="bg-black">
        <div class="container">
            <nav class="navbar navbar-expand-lg navbar-light bg-black pt-5 pb-5">
                <a class="navbar-brand content" href="#"> --&#62; Content goes here &#60;-- </a>
            </nav>
        </div>
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
