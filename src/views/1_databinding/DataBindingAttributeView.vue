<template>
    <div>
        <input type="text" name="" id="" v-bind:value="userId" readonly>
        <input type="text" name="" id="" :value="userId" readonly>
        <br/>
        <img :src="imgsrc" alt="" :style="mystyle">
        <br/>
        <input type="search" name="" id="" v-model="txt1">
        <button :disabled="txt1 === ''">조회</button>
    </div>
</template>
<script>
export default {
    components: {},
    data() {
        return {
            userId: 'kimsw',
            imgsrc: 'https://upload.wikimedia.org/wikipedia/commons/thumb/c/cd/Stray_kitten_Rambo002.jpg/1200px-Stray_kitten_Rambo002.jpg',
            mystyle: 'width: 100px; height: auto',
            txt1: ''
        }
    },
    created() {},
    mounted() {},
    unmounted() {},
    methods: {}
}
</script>