<template>
    <div class="layout">
        <div class="nav">
            <div v-for="(item, index) in navArr" :key="index">
                <span class="nav_text">{{ item.text }}</span>
            </div>
        </div>
    </div>
    <slot/>
</template>

<script setup>
const navArr = ref([
    {
        text: 'home',
        link: 'a'
    },
    {
        text: 'map',
        link: 'b'
    }
])
</script>

<style lang="less" scoped>
.layout {
    display: flex;
    justify-content: flex-end;
    margin-bottom: 50px;

    .nav {
        background-color: #0e1630;
        display: flex;
        width: 400px;
        padding: 10px;
        justify-content: space-around;
        border: solid 1px rgba(193, 193, 193, 0.526);

        .nav_text {
            flex: 1;
            padding: 5px;
            cursor: pointer;
            transition: ease-in-out .2s;
            // border-right: solid 1px gray;

            &:hover {
                color: #eb4a4a;
            }
        }
    }
}
</style>