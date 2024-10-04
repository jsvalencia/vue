<template>
    <h1 className="text-3xl font-bold underline">
      Hello world!
    </h1>
    <hr/>
    <MyCounter :value="25"/>
    <CounterCopy :value="3"/>
    <CounterCopy3 :value="2"/>
</template>
<script lang="ts" setup>
import MyCounter from './components/Counter.vue'
import CounterCopy from './components/CountercCopy.vue'
import CounterCopy3 from './components/MyCounter3.vue'
</script>

