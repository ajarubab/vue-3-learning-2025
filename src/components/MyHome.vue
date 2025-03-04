<template>
    <h1 v-if="Show">It's Day Now</h1>
    <h1 v-else>It's Night time</h1>
    <button v-on:click="Show=!Show">Change Time</button>
    
</template>
<script>
    export default {
        name : 'MyHome',
        data(){
            return{
                Show : true,
            }
        }
    }
</script>