<template>
    <hr>
    <h1> Get Input Feild Value</h1>

    <input type="email"   v-model="email" placeholder="enter email">
    <br>
    <br>
    <input type="password" v-model="pass"  placeholder="enter paasword">

    <br>
    <br>

    <button type="button" v-on:click="getData()">Submit</button>
   
</template>

<script >

    export default {
        name : 'GetInput',
        data(){
            return {
                email : null,
                pass  : null
            }
        },

        methods : {
            getData(){
                console.warn( this.email, this.pass)

                alert("data submitted")
        }

    }
}
</script>

<style scoped>
 h1{
      color: orange;
    }
</style>
