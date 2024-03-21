<template>
    <h1>{{ title }}</h1>
    <h2>{{ subTitle }}</h2>

    <table border="1">
        <thead>
            <tr>
                <th>번호</th>
                <th>이름</th>
                <th>핸드폰</th>
                <th>회사</th>
            </tr>
        </thead>
        <tbody>
            <tr v-bind:key="personVo.no"  v-for="(personVo) in pList" >
                <td></td>
                <td>{{ personVo.name }}</td>
                <td></td>
                <td></td>
            </tr>
        </tbody>
    </table >

    <br>
    <button v-on:click="getList" type="button">데이터불러오기</button>
</template>
<script>

export default {
    name: "Ex08View",
    components: {},
    data() {
        return {
            title: "vue공부",
            subTitle: "반복문",
            pList: []
        };
    },
    methods: {
        getList(){
            console.log("데이터 수신중......");
            let personList = [
                {no: 1, name: "정우성", hp: "010-1111-1111", company: "02-1111-1111"},
                {no: 2, name: "이효리", hp: "010-2222-2222", company: "02-2222-2222"},
                {no: 3, name: "유재석", hp: "010-3333-3333", company: "02-3333-3333"}
            ]
            this.pList = personList;
         

        }
    },
};
</script>
<style></style>