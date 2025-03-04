<template>
    <h1>My Home Component</h1>
    <button v-on:click="Click()">Click me</button>
    <br>
    <br>
    <button v-on:click="ClickMe('Click me Again Function Called')">Click me Again</button>
    <br>
    <br>
    <button v-on:dblclick="DblClickMe('Button double clicked')">Double Click me Again</button>
    <br>
    <br>
    <h1 v-on:mouseover="mouseMove()">Count : {{ count }}</h1>
    <br>
    <button v-on:click="incrCount()">Increase count</button>
    <br>
    <br>
    <button v-on:click="decrCount()">Decrease count</button>
</template>
<script>
export default {
    name: 'MyHome',
    data() {
        return {
            count: 0
        }
    },
    methods: {
        Click() {
            alert(" Click me Button Clicked");
        },
        ClickMe(data) { alert(data); },
        DblClickMe(data) { alert(data); },
        incrCount() { return this.count = this.count + 1; },
        decrCount() { return this.count = this.count - 1; },
        mouseMove() { console.log("Mouse moved over count number") },
    }
}
</script>
