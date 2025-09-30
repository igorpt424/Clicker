
<template>
  <div class="wpapper">
    <div class="container">
      <img src="../assets/apple.png" class="apple">
      <p class="count">{{ count }}</p>
      <router-link to="/menu" class="link">-></router-link>
    </div>
    
    <button @click.prevent="increment()"><img src="../assets/hedgehog.png" class="hedgehog"></button>
  </div>
</template>

<style scoped>
/*.wpapper{
  column-gap: 20px;
  position: fixed;
  left: 50%;
  top: 50%;
  transform: translate(-50%, -50%);
}
.container{
  gap: 10px;
  align-items: center;
  display: flex;
}
.count{
  background-color: red;
  padding: 10px 50px;
  font-size: 25px;
  border-radius: 15px;
  border: 7px solid brown;
}

.apple{
  max-width: 50px;
  max-height: 50px;
}

.hedgehog{
  max-width: 500px;
}
.link{
  padding: 10px;
  background: yellow;
  text-decoration: none;
  color: black;
  border-radius: 50%;
}*/
.wpapper {
  column-gap: 20px;
  position: fixed;
  left: 50%;
  top: 50%;
  transform: translate(-50%, -50%);
  .container {
  gap: 10px;
  align-items: center;
  display: flex;
    .apple {
      max-width: 50px;
      max-height: 50px;
    }
    .count {
      background-color: red;
      padding: 10px 50px;
      font-size: 25px;
      border-radius: 15px;
      border: 7px solid brown;
          }
    .link {
      padding: 10px;
      background: yellow;
      text-decoration: none;
      color: black;
      border-radius: 50%;
      }
    }
    button {
      .hedgehog {
        max-width: 500px;
      }
    }
  }
</style>

<script setup>
import { ref } from 'vue';

const count = ref(0)
function increment(){
  count.value++
}
</script>