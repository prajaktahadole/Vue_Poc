<template>
     <hr>
    <h1>Counter</h1>
    <h2> {{count}}</h2>
    <button  v-on:click="handleCount()"> Counter</button>
</template>

<script >
    export default {
      name : 'Counter',

      data(){
        return {
             count : 0,
            }
      },
      methods : {

        handleCount(){
            this.count = this.count +1
        }
      }
    }
</script>

<style scoped>
    h1{
      color: green;
    }
</style>
