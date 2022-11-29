<template>
<div>
    <select name="" id="" @change="changeCity" v-model="selectCity">
        <option value="">==도시 선택==</option>
        <option :value="city.code" :key="city.code" v-for="city in cityList">{{city.title}}</option>
    </select>
    &nbsp;
    <select name="" id="">
        <option value="">==동 선택==</option>
        <option :value="dong.code" :key="dong.code" v-for="dong in selectedDongList">{{dong.title}}</option>
    </select>
</div>
</template>
<script>
export default {
    components: {},
    data() {
        return {
            cityList: [
                {code: '02', title: '서울'},
                {code: '051', title: '부산'},
                {code: '064', title: '제주'},
            ],
            selectCity: '',
            dongList: [
                {code:'02', dongCode:'1', title:'서울1동'},
                {code:'02', dongCode:'2', title:'서울2동'},
                {code:'02', dongCode:'3', title:'서울3동'},
                {code:'02', dongCode:'4', title:'서울4동'},
                {code:'051', dongCode:'1', title:'부산1동'},
                {code:'051', dongCode:'2', title:'부산2동'},
                {code:'051', dongCode:'3', title:'부산3동'},
                {code:'051', dongCode:'4', title:'부산4동'},
                {code:'064', dongCode:'1', title:'제주1동'},
                {code:'064', dongCode:'2', title:'제주2동'},
                {code:'064', dongCode:'3', title:'제주3동'},
                {code:'064', dongCode:'4', title:'제주4동'},
            ],
            selectedDongList: []
        }
    },
    created() {},
    mounted() {},
    unmounted() {},
    methods: {
        changeCity(){
            this.selectedDongList = this.dongList.filter(dong=>dong.code === this.selectCity)
        }
    }
}
</script>