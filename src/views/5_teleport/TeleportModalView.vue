<template>
<div>
    <div id="modal"></div>
    <h1>⭐TELEPORT Modal!</h1>
    <button @click="openModal">open Modal</button>
    <div id="modal"></div>
    <teleport to="#modal">
        <div class="black-bg" v-if="(isModal==true)">
            <div class="withe-bg">
                <button @click="closeModal">❌</button>
                hello teleport modal!<br/>
                Click Outside
            </div>
        </div>
    </teleport>
</div>
</template>
<script>
export default {
    components: {},
    data() {
        return {
            isModal:false
        }
    },
    created() {},
    mounted() {},
    unmounted() {},
    methods: {
        openModal(){
            this.isModal = true
            console.log('hi');
        }
    }
}
</script>
<style>
body{
    margin: 0;
}
div{
    box-sizing: border-box;
}
.black-bg{
    width: 100vw; height: 100vh;
    background-color: rgba(0,0,0,0.5);
    padding: 20px;
}
.withe-bg{
    width: 90%; height: 90%;
    background: white;
    border-radius: 8px;
    padding: 20px;
}
</style>