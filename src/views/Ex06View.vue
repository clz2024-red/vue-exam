<template>
    <h1>{{title}}</h1>
    <h2>{{subTitle}}</h2>

    <select name="telecom">
        <option value="">이동통신사를 선택해주세요</option>
        <option value="sk" >SK텔레콤</option>
        <option value="kt" selected="selected">KT</option>
        <option value="lg">LG U+</option>
    </select>

    <br><br>
    <select name="telecom" v-model="telecom">
        <option value="">이동통신사를 선택해주세요</option>
        <option value="sk" >SK텔레콤</option>
        <option value="kt" >KT</option>
        <option value="lg">LG U+</option>
    </select>
    <p>선택한 이동통신사는 {{ telecom }}입니다.</p>

</template>
<script>

export default {
    name: "Ex06View",
    components: {},
    data() {
        return {
            title: "vue공부",
            subTitle: "폼-selectbox: (양방향바인딩)->폼에는 v-model그냥쓰자",
            telecom: "sk"
        };
    },
    methods: {},
};
</script>
<style></style>