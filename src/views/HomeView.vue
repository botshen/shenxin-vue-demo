<script setup lang="ts">
import { onMounted } from 'vue';
import axios from 'axios';



const handleTestClick = async () => {
  console.log('test');
  axios.post('/api/xxxx', {
    firstName: 'Fred',
    lastName: 'Flintstone'
  })
  .then(function (response) {
    
  })
  .catch(function (error) {
    console.log(error);
  });

};

</script>

<template>
  <main>
    沈鑫
    <button @click="handleTestClick">test</button>
  </main>
</template>
