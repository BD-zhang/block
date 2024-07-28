<template>
    <div class="box">
        <div class="box_left">
            <Card img-src="/picture.png" text="Oculus Working on Update to Improve Rift S Audio"/>
            <div class="box_info">
                <div class="info_detail">
                    <i class="iconfont icon-didian1 icon"></i>
                    <span class="detail_text">github.com</span>
                </div>
                <div class="info_detail">
                    <i class="iconfont icon-didian1 icon"></i>
                    <span class="detail_text">xxx-xxx.@email.com</span>
                </div>
            </div>
        </div>
        <div class="box_right">
            <RightPage/>
        </div>
    </div>
</template>

<script setup>
import RightPage from './components/RightPage.vue';
defineComponent({
    RightPage
})

</script>

<style lang="less">
.box {
    // background-color: rgb(18, 9, 64);
    // height: 100vh;
    // width: 100vw;
    display: flex;

    .box_left {
        width: 30%;
    }

    .box_right {
        width: 70%;
    }

    .icon {
        font-size: 16px;
    }

    .info_detail {
        width: 260px;
        margin-top: 15px;
        display: flex;
        align-items: center;
        // justify-content: space-between;
    }

    .detail_text {
        margin-left: 50px;
    }
}
</style>