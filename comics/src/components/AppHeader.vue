<script setup>
const arrayHeader = ['characters', 'comics', 'movies', 'tv', 'games', 'collectibles', 'videos', 'fans', 'news', 'shop'];
</script>

<template>
    <!-- Image and text -->
    <nav class="navbar navbar-light bg-white">
        <div class="container">
            <a class="navbar-brand p-3" href="#">
                <img src="../assets/img/dc-logo.png" width="80" height="80" class="d-inline-block align-top" alt="">
            </a>
            <ul class="nav justify-content-end">
                <li class="nav-item custom-li" v-for="element in arrayHeader">
                    <span class="nav-link text-black" href="#">
                        <strong>
                            {{ element.toUpperCase() }}

                        </strong>
                    </span>
                </li>
            </ul>
        </div>
    </nav>
</template>

<style scoped></style>
