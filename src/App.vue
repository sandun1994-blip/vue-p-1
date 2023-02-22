<template>
  <div>
the current count :{{  count}}
  </div>
  <button @click="handleClick">+</button>
  <button @click="count--">-</button>
</template>


<script setup>
import { ref } from 'vue';


let count =ref(0)
console.log(count);
const handleClick =()=>{
 count.value++
}

</script>