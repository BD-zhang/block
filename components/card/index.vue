<template>
    <div class="card">
        <div class="card_img">
            <img :src="imgSrc" alt="">
        </div>
        <div class="card_text">
            <span>{{ text }}</span>
        </div>
    </div>
</template>

<script setup>
const props = defineProps({
    imgSrc: String,
    text: String
})

</script>

<style lang="less">
.card {
    width: 260px;
    height: 300px;
    border: solid 1px rgba(214, 214, 214, 0.345);
    border-radius: 10px;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    transition: ease-in-out .2s;
    margin-right: 10px;
    margin-bottom: 20px;

    &:hover {
        box-shadow: 1px 1px 20px rgb(36, 32, 32);
    }

    .card_img {
        height: 70%;
        img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            border-top-left-radius: 10px;
            border-top-right-radius: 10px;
        }
    }

    .card_text {
        padding: 10px;
        height: 30%;
        background-color: #1D1F24;
        color: white;
        border-bottom-left-radius: 10px;
        border-bottom-right-radius: 10px;
    }
}
</style>