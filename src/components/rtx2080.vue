<template>
  <div class="root">
      <div class="main-card">
        <img class="card-image" src="../img/2080.png">

        <h1 class="card-header">RTX 2080</h1>

        <p class="card-text">
          The NVIDIA GeForce RTX 2080 Ti is the fastest consumer desktop graphics card in 2018.
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