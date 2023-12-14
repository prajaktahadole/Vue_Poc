<script >
import Event from './components/Event.vue';
import Counter from './components/Counter.vue';
import TwoWayBinding from './components/TwoWayBinding.vue';
import GetInput from './components/GetInput.vue';
import CheckBoxx from './components/CheckBoxx.vue'

    export default {
      name : 'App',
      components : {
          Event,
          Counter,
          TwoWayBinding,
          GetInput,
          CheckBoxx
      }
    }
</script>

<template>
    <h1>welcome to poc2</h1>
    <Event></Event>
    <Counter></Counter>
    <TwoWayBinding></TwoWayBinding>
    <GetInput></GetInput>
    <CheckBoxx></CheckBoxx>
</template>

<style scoped>

</style>
