<template>
  <div class="root">
      <div class="main-card">
        <img class="card-image" src="../img/1050.png">

        <h1 class="card-header">GTX 1050</h1>

        <p class="card-text">
       The GeForce GTX 1050 was a high-end graphics card by NVIDIA, launched on October 25th, 2016. 

        </p>
      </div>
  </div>
</template>

<script>
export default {

}   
</script>

<style>
.main-card {
    display: flex;
    flex-direction: column;
    justify-content: space-around;
    align-items: center;

    font-family: 'Geforce';
    color: #00FF29;
    
    background-color: black;
    box-shadow: 10px 10px 10px rgba(24, 24, 24, 0.379);

    margin-top: 30px;
    margin-right: 62px;

    padding: 10px;
    
    width: 220px;
    height: 350px;
}

.card-text {
    color: #FFF;
    font-weight: bold;
    font-size: 18px;
}
.card-image {
    height: 160px;
}
</style>