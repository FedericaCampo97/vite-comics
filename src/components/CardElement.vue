<script>

export default {
    name: 'CardMain',
    props: ['thumb', 'title'],
    data() {
        return {
        }
    }
}
</script>

<template>
    <div class="p-3">
        <img :src="thumb" class="img_card" alt="">
        <h6 class="text-white mt-3 text-uppercase">{{ title }}</h6>
    </div>
</template>

<style></style>