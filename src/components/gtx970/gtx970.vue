<template>
  <div class="root">
    <div class="main-card" @click="show970Modal = true">
      <img class="card-image970" src="./970.png" />

      <h1 class="card-header">GTX 970</h1>

      <p class="card-text">
        The GeForce GTX 970 was a high-end graphics card by NVIDIA, launched on
        September 18th, 2014.
      </p>
    </div>

      <Teleport to="body">
        <Modal 
          :show="show970Modal"
          @close="show970Modal = false"
        />
    </Teleport>
  </div>
</template>

<script>
import Modal from './modal970.vue'

export default {
  components: {
    Modal
  },

  data: () => ({
    show970Modal: false,
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
.card-image970 {
  transform: rotate(30deg);
  height: 160px;
  width: 160px;
}
</style>