<template>
    <h1> USE OF FOR LOOP AND WHILE LOOP</h1>
    <ul>
        <li v-for="x in color" :key="x">
            {{ x }}
        </li>
        <br>
        <li v-for="y in firstTable" :key="y">
            {{ y }}
        </li>
        <br>
        <li v-for="z in secondTable" :key="z">
            {{ z }}
        </li>
    </ul>
    
</template>
<script>
    export default {
        name : 'MyHome',
        data(){
            return{
                color : ['Red','Black','Blue','Green'],
                firstTable : this.getTableOf(5),
                secondTable : this.getAnotherTable(12),
            }
        },
        methods:{
            getTableOf(n){
                let res = [];
                for(let m = 1; m<= 10; m++){
                    res.push(n*m);
                }
                return res;
                
            },
            getAnotherTable(n){
                let res = [];
                let m = 1;
                while(m<11){
                    res.push(n*m);
                    m++;
                }
                return res;
            }
        }
    }
</script>