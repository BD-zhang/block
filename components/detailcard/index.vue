<template>
    <div class="detail_card">
        <div :class="['card_img', isEven ? 'card_img_right' : 'card_img_left']">
            <img src="/picture.png" alt="">
        </div>
        <div :class="['card_text', isEven ? 'card_text_right' : 'card_text_left']">ni hao ni hao nihao nihaoni hao ni hao nihao nihaoni hao ni hao nihao nihaoni hao ni hao nihao nihao</div>
    </div>
</template>

<script setup>
const prop = defineProps({
    isEven: Boolean
})
</script>

<style lang="less" scoped>
.detail_card {
    width: 800px;
    position: relative;
    margin-bottom: 20px;
    cursor: pointer;

    .card_img {
        width: 200px;
        height: 150px;
        position: absolute;
        border-radius: 10px;
        border: 1px solid rgba(151, 151, 151, 0.404);

        &_left {
            left: 10px;
        }

        &_right {
            right: 10px;
        }

        img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            border-radius: 10px;
            
        }
    }

    .card_text {
        height: 150px;
        width: 100%;
        margin-top: 20px;
        border-radius: 10px;
        border: solid 1px rgb(214 214 214 / 35%);
        background-color: #1D1F24;
        box-sizing: border-box;
        font-size: 13px;
        padding: 20px;
        transition: ease-in-out .2s;

        &_left {
            padding-left: 218px;

        }

        &_right {
            padding-right: 218px;
        }

        &:hover {
            box-shadow: 1px 1px 10px grey;
        }
    }
}
</style>