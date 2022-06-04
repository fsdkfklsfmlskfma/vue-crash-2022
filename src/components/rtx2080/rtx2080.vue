<template>
  <div class="root">
    <div class="main-card" @click="show2080Modal = true">
      <img class="card-image2080" src="./2080.png" />
      <h1 class="card-header">RTX 2080</h1>

      <p class="card-text">
        The GeForce GTX 750 was a high-end graphics card by NVIDIA, launched on
        February 18th, 2014.
      </p>
    </div>

    <Teleport to="body">
      <Modal 
        :show="show2080Modal"
        @close="show2080Modal = false"
      />
    </Teleport>
  </div>
</template>

<script>
import Modal from './modal2080.vue'

  export default {
    components: {
      Modal,
    },

    data: () => ({
      show2080Modal: false,
    })
  };

</script>

<style>
.main-card {
  display: flex;
  flex-direction: column;
  justify-content: space-around;
  align-items: center;

  font-family: "Geforce";
  color: #00ff29;

  background-color: black;
  box-shadow: 10px 10px 10px rgba(24, 24, 24, 0.379);

  margin-top: 30px;
  margin-right: 62px;

  padding: 10px;

  width: 220px;
  height: 350px;
}

.card-text {
  color: #fff;
  font-weight: bold;
  font-size: 18px;
}
.card-image2080 {
  transform: rotate(50deg);
  height: 160px;
  width: 160px;
}
</style>