<template>
  <div class="root">
    <!-- @click="show1050Modal" -->
    <div class="main-card" @click="show1050Modal = true">
      <img class="card-image1050" src="./1050.png" />
      <h1 class="card-header">GTX 1050</h1>

      <p class="card-text">
        The GeForce GTX 1050 was a high-end graphics card by NVIDIA, launched on
        October 25th, 2016.
      </p>
    </div>

     <Teleport to="body">
      <Modal 
        :show="show1050Modal"
        @close="show1050Modal = false"
      />
    </Teleport>
  </div>
</template>

<script>
// ИМПОРТИРОВАТЬ МОДАЛКУ
import Modal from './modal1050.vue'

export default {
  components: {
    Modal
  },

  data: () => ({
    show1050Modal: false
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
.card-image1050 {
  transform: rotate(35deg);
  height: 160px;
  width: 140px;
}
</style>