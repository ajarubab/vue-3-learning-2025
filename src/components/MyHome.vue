<template>
    <h1> My Home</h1>
    <ol>
        <li v-for="x in user" :key="x.name">
            Name : {{ x.name }}, Age : {{ x.age }}
        </li>
    </ol>
</template>
<script>
    export default {
        name : 'MyHome',
        data(){
            return{
                user : [
                    {name: 'raja', age : 23},
                    {name: 'raju', age : 21},
                    {name: 'rajan', age : 28},
                    {name: 'rajat', age : 22},
                    {name: 'rajesh', age : 52},
                ],
            }
        }
    }
</script>