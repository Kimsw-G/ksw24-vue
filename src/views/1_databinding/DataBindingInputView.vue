<template>
    <div>
        <input type="text" v-model="userId">
        <button @click="myFunction()">클릭!</button>
        <button @click="changeData()">변경!</button> <br>

        <input type="text" v-model="num0"> + 
        <input type="text" v-model="num1"> = 
        <span>{{num0 + num1}}</span><br/>

        <input type="text" v-model.number="num2"> + 
        <input type="text" v-model.number="num3"> = 
        <span>{{num2 + num3}}</span><br/>
    </div>
</template>
<script>
export default {
    components: {},
    data() {
        return {
            userId: '',
            num0 : 0,
            num1 : 0,
            num2 : 0,
            num3 : 0,
        }
    },
    created() {},
    mounted() {},
    unmounted() {},
    methods: {
        myFunction(){
            console.log(this.userId);
        },
        changeData(){
            this.userId = "kimsw"
        }
    }
}
</script>