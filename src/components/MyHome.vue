<template>
    <h1>Color</h1>
    <label for="black">Black</label>
    <input type="checkbox" id="black" value="Black" v-model="color"> <br><br>
    <label for="red">Red</label>
    <input type="checkbox" id="red" value="Red" v-model="color"> <br><br>
    <label for="green">Green</label>
    <input type="checkbox" id="green" value="Green" v-model="color"><br><br>
    <label for="blue">Blue</label>
    <input type="checkbox" id="blue" value="Blue" v-model="color"><br><br>
    <h2>Opted Color are : {{ color }}</h2>    
</template>
<script>
    export default {
        name : 'MyHome',
        data(){
            return{
                color : []
            }
        }
    }
</script>