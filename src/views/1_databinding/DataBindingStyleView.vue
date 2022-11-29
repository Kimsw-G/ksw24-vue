<template>
    <div>
        <div :style="style1">
            스타일 바인딩: 글씨:red, 폰트크기:30px
        </div>
        <button @click="style1.color='blue'">색상바꾸기</button>
    </div>
</template>
<script>
export default {
    components: {},
    data() {
        return {
            style1: {
                color: 'red',
                fonsSize: '30px'
            }
        }
    },
    created() {},
    mounted() {},
    unmounted() {},
    methods: {}
}
</script>
<style>
</style>