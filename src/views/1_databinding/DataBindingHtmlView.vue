<template>
    <div>{{htmlString}}</div>
    <div v-html="htmlString"></div>
    <div v-show="true">hi</div>
</template>
<script>
export default {
    components: {},
    data() {
        return {
            htmlString: '<p style="color:red;">빨간맛</p>'
        }
    },
    created() {},
    mounted() {},
    unmounted() {},
    methods: {}
}
</script>