<template>
    <div>
        <div>{{count}}</div>
        <button @click="increaseCounter">Add 1</button>
    </div>
</template>
<script>
export default {
    components: {},
    data() {
        return {
            count: 1
        }
    },
    created() {},
    mounted() {},
    unmounted() {},
    methods: {
        increaseCounter(){
            this.count++;
        }
    }
}
</script>