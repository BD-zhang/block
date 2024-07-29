<template>
    <div class="right">
        <Detailcard :is-even="true"/>
        <Detailcard :is-even="false"/>
        <Detailcard :is-even="true"/>
        <Detailcard :is-even="false"/>
        <Detailcard :is-even="true"/>
    </div>
</template>

<script setup></script>

<style lang="less" scoped>
.right {
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
    flex: 3;
    height: 100%;
}
</style>