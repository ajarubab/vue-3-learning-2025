<template>
    <h1>Gender</h1>
    <label for="male">Male</label>
    <input type="radio" id="male" value="Male" name="myGender" v-model="gender"> <br><br>
    <label for="female">Female</label>
    <input type="radio" id="female" value="Female" name="myGender" v-model="gender"> <br><br>
    <h2>I am a {{ gender }}.</h2>    
</template>
<script>
    export default {
        name : 'MyHome',
        data(){
            return{
                gender : ""
            }
        }
    }
</script>