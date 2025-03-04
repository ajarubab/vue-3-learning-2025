<template>
    <h1>MyHome Component</h1>
    <h1>20 + 15 = {{ 20+15 }}</h1>
    <h1>The word "asfjhaskhgbalejgklgh" has {{ "asfjhaskhgbalejgklgh".length }} Characters.</h1>
    <h1>{{ naam }} is of {{ Age }} years old and lives in {{ getCountry() }}</h1>
    <h1>{{ naam1 = "Ramu" }} is of {{ Age1 = 34 }} years old and lives in {{ getState("Nepal") }}</h1>
</template>
<script>
export default {
    name: 'MyHome',
    data(){
        return{
            naam : "Raja kumar",
            naam1 : "",
            Age : 28,
            Age1 : 28,
            getCountry : function(){
                return "India";
            },
            getState : function(a){
            return a;
            },
        }
    }
}
</script>
<style scoped>
h1{
    color:blue;
}
</style>