<template>
    <div>
        <select name="" id="" v-model="selectCity">
            <option value=""></option>
            <option value="02">서울</option>
            <option value="051">부산</option>
            <option value="054">제주</option>
        </select>
    </div>
</template>
<script>
export default {
    components: {},
    data() {
        return {
            selectCity: '051'
        }
    },
    created() {},
    mounted() {},
    unmounted() {},
    methods: {}
}
</script>