<template>
    <h1>Child components</h1>
    <h2>Message from Home : {{ msg }}</h2>
    <h2>Name of user from Home : {{ userDetails.naam }}</h2>
    <h2>Age of user from Home : {{ userDetails.Age }}</h2>
    <button v-on:click="funCall()">Click me</button>
</template>
<script>
    export default{
        name : "MyChild",
        props:{
            msg : String,
            userDetails : Object,
            funCall : Function,
        }
    }
</script>