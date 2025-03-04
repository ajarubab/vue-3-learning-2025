<template>
    <h1>My Home Component</h1>
    <h1>{{ Name }}</h1>
    <h1>{{ getName() }}</h1>
    <h1>{{ getCountry("India") }}</h1>
    <h2>Other Data : {{ getData() }}</h2>
    <h2>Other Data State: {{ getData().State }}</h2>
    <h2>State: {{ getState() }}</h2>
    <h2>Age: {{ getAge() }}</h2>
</template>
<script>
export default{
    name : 'MyHome',
    data(){
        return{
            Name : 'Rajat Kumar',
            Age : 28,
        }
    },
    methods : {
        getName(){
            return "Radhe Radhe";
        },
        getCountry(c){
            return c;
        },
        getData(){
            return{
                State : "Delhi",
                Email : "Raja@kumar.in"
            }
        },
        getState(){
            return this.getData().Email;
        },
        getAge(){
            return this.Age;
        }
    }
}
</script>