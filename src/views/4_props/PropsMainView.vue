<template>
<div>
    <div>나는 메인</div>
    <Sub value1="value1. 바나나 😢" @setInput="setInput">

    </Sub>
    <input v-model="mylet">
</div>
</template>
<script>
import Sub from './PropsSubView.vue' 
export default {
    components: {
        Sub
    },
    data() {
        return {
            myvalue: "",
            mylet: ""
        }
    },
    created() {},
    mounted() {},
    unmounted() {},
    methods: {
        setInput(myvalue, mylet){
            this.myvalue = myvalue
            this.mylet = mylet
            console.log(`값 받기 성공 ${myvalue}, ${mylet}`);
        }
    }
}
</script>