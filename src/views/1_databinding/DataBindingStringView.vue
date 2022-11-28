<template>
<div>
    <h1>HI {{userName}}</h1>
    <p>{{message}}</p>
</div>
</template>

<script>
export default{
    data(){
        return{
            userName : "Kim SeongWuk",
            message : 'Hello World!!',
            arr : [],
            obj : {}
        }
    }
}
</script>

<style scoped> 

</style>