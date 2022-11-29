<template>
    <div>
        <div>
            <input type="radio" name="" id="html" value="HTML" v-model="favoriteLang">
            <label for="html">HTML</label>
        </div>
        <div>
            <input type="radio" name="" id="css" value="css" v-model="favoriteLang">
            <label for="css">css</label>
        </div>
        <div>
            <input type="radio" name="" id="js" value="js" v-model="favoriteLang">
            <label for="js">js</label>
        </div>
        <div>
            selected : {{favoriteLang}}
        </div>
    </div>
</template>
<script>
export default {
    components: {},
    data() {
        return {
            favoriteLang: ''
        }
    },
    created() {},
    mounted() {},
    unmounted() {},
    methods: {}
}
</script>