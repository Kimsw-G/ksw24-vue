<template>
<div>
    여기는 서브입니다.
    {{value1}}<br>
    <button @click="sendEmit">에밋 제출</button>
</div>
</template>
<script>
export default {
    components: {},
    props: {
        value1: String
    },
    data() {
        return {
            myvalue: "sfsfs"
        }
    },
    created() {},
    mounted() {},
    unmounted() {},
    methods: {
        sendEmit(){
            let emitValue = "나는 에밋된 값"
            this.$emit("setInput",this.myvalue,emitValue)
        }
    }
}
</script>