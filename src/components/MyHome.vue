<template>
    <h1> My Home Component</h1>
    <h2>The Count is  {{ count }}</h2>
    <input type="text" v-model="count">
</template>
<script>
    export default {
        name : 'MyHome',
        data(){
            return{
                count : 10276,
            }
        }
    }
</script>