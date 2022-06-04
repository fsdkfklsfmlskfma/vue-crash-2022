<template>
  <div class="root">
    <div class="main-card" @click="show3090Modal = true">
      <img class="card-image3090" src="./3090.png" />
      <h1 class="card-header">RTX 3090</h1>

      <p class="card-text">
        The GeForce GTX 750 was a high-end graphics card by NVIDIA, launched on
        February 18th, 2014.
      </p>
    </div>

    <Teleport to="body">
      <Modal 
        :show="show3090Modal"
        @close="show3090Modal = false"
      />
    </Teleport>
  </div>
</template>

<script>
import Modal from './modal3090.vue'

  export default {
    components: {
      Modal,
    },

    data: () => ({
      show3090Modal: false,
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
.card-image3090 {
  transform: rotate(222deg);
  height: 160px;
  width: 160px;
}
</style>