<template>
    <h1> My Home Component</h1>
    <input type="text"  placeholder="Enter username" v-model="username"><br><br>
    <input type="password" placeholder="Enter Password" v-model="password"><br><br>
    <button v-on:click="userDetails()">Submit</button>
    
</template>
<script>
    export default {
        name : 'MyHome',
        data(){
            return{
                username : null,
                password : null,
            }
        },
        methods:{
            userDetails(){
                console.log("Username : ",this.username,"\nPassword : ",this.password);
            }
        },
    }
</script>