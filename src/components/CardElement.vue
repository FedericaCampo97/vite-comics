<script>

export default {
    name: 'CardMain',
    props: ['thumb'],
    data() {
        return {
        }
    }
}
</script>

<template>
    <div class="p-3">
        <img :src="thumb" class="img_card" alt="">
        <h5 class="text-white mt-3">Action Comic</h5>
    </div>
</template>

<style></style>