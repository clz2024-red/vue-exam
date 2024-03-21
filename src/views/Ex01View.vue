<template>
    <h1>{{ title }}</h1>
    <h2>{{ subTitle }}</h2>

    <p>{{ content }}</p>
</template>

<script>
export default {
    name: "Ex01Vuew",
    components: {},
    data() {
        return {
            title: "vue공부",
            subTitle: "페이지만들기 + 라우터 페이지 개념 추가",
            content: "vue 공부시작"
        };
    },
    methods: {},
};
</script>

<style></style>

