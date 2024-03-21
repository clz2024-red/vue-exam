<template>
    <h1>{{ title }}</h1>
    <h2>{{ subTitle }}</h2>

    <p>{{ counter }}</p>

    <button v-on:click="minus" type="button">빼기(-)</button>
    <button v-on:click="plus" type="button">더하기(+)</button> 
    

    <br>
    <br>

    <p>{{ message }}</p>
    <button v-on:click="setMessage" type="button">메세지출력</button>

</template>
<script>

export default {
    name: "Ex03View",
    components: {},
    data() {
        return {
            title:"Vue공부",
            subTitle: "클릭이벤트+메소드",
            counter: 0,
            message: ""
        };
    },
    methods: {
        //plus: function plus(){};
        plus(){
            this.counter++;
        },
        minus(){
            this.counter--
        },
        setMessage(){
            console.log("클릭");
            this.message = "늦으면 연락하겠.....아니 늦지 않겠습니다.";
        }
    }
};
</script>
<style></style>