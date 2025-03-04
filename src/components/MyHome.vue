<template>
    <h1>My Home Component</h1>
    <button v-on:click="Click()">Click me</button>
</template>
<script>
export default{
    name : 'MyHome',
    methods :{
        Click(){
            alert ("Button Clicked");
        }
    }
}
</script>