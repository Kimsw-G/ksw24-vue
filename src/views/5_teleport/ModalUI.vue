<template>
<div>
    <div class="black-bg" v-if="(isModal==true)">
        <div class="withe-bg">
            <h4>상세페이지</h4>
            <p>상세페이지 내용</p>
        </div>
    </div>

    <button @click="openModal">Modal ON</button>
</div>
</template>
<script>
// UI 상태를 데이터로 저장
// 데이터를 통해 모달창 상태 작성
//
export default {
    components: {},
    data() {
        return {
            isModal : false, // 모달창의 상태 state

        }
    },
    created() {},
    mounted() {},
    unmounted() {},
    methods: {
        openModal(){
            this.isModal = true
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
    width: 70%; height: 70%;
    background-color: rgba(0,0,0,0.5);
    position: fixed; padding: 20px;
}
.withe-bg{
    width: 90%; height: 90%;
    background: rgba(255, 255, 255, 1);
    border-radius: 8px;
    
}
</style>