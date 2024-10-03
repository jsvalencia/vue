<template>
    <h1>Hola Mundo</h1>
    <h3>Contador: {{ contador }}</h3>
    <h3>Cuadrado: {{ contador*contador }}</h3>

    <div>
        <button @click="contador++">+1</button>
        <button @click="contador--">-1</button>
    </div>
</template>

<script lang="ts" setup>
import { ref } from 'vue';// Se importa al declarar la variavle reactiva


/*const props = defineProps({
    //value: Number
    value: {type:Number, required:true}
})*/

const props = defineProps<{
    value:number;
}>();

const contador =ref(props.value);// es automanticamente retornado y se puede usar 

</script>

