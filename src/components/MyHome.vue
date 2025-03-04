<template>
    <h1> My Home</h1>
    <Child msg="Hello my Child" :userDetails="user" :funCall="callFunction"/>
</template>
<script>
import Child from './Child.vue';

export default {
    name: 'MyHome',
    components: {
        Child,
    },
    data() {
        return{
            user : {
                naam : 'Raja',
                Age : 28
            }
        }
    },
    methods:{
        callFunction(){
            console.log("parent function called");
            alert("Parent function called");
        }
    }
}

</script>