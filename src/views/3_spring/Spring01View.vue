<template>
    <div>
        <h1>{{value}}</h1>
        <button @click="posting()">
            제출
        </button>
    </div>
</template>
<script>
export default {
    components: {},
    data() {
        return {
            value: 'banana'
        }
    },
    created() {},
    mounted() {},
    unmounted() {},
    methods: {
        posting(){
            this.axios.get('/v1/test')
            .then((result)=>{
                console.log(result);
            })
        }
    }
}
</script>