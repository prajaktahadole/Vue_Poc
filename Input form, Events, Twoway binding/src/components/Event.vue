<template>
    <h1>Click Event</h1>
    <button v-on:click="test()">Click Me</button>
    <button v-on:click="getData('Button 1 Clicked')">button 1</button>
    <button v-on:click="getData('Button 2 Clicked')">button 2</button>
    <button v-on:dblclick="getData('Button double clicked')"> double click</button>
    <h2> {{count}}</h2>
    <button  v-on:click="handleCount()"> Counter</button>
</template>

<script >
    export default{
        name : "Event",
        
        data(){
            return {
                count : 0,
            }
        },

        methods: {
            test(){
                alert("Button clicked")
            },

            getData(text){
                alert(text);
            },

            handleCount(){
                this.count = this.count + 1;
            }
        }
    }
</script>

<style scoped>

    h1{
      color: red;
    }

</style>
