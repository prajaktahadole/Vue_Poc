<template>
    <hr>
    <h1>Two Way Binding</h1>

    <input type="text" v-model="writtentext">

    <h2>{{ writtentext }}</h2>
   
</template>

<script >

    export default {
        name : 'TwoWayBinding',
        data(){
            return{
                writtentext : "lets learn two way  binding"
            }
        }
    }
  
</script>

<style scoped>
 h1{
      color: blue;
    }
</style>
