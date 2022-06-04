<template>
  <div 
    id="modal-container"
    v-if="show"
  >
    <div class="controls">
      <button 
        class="modal-close"
        @click="$emit('close')"
      >
        <img src="../back.svg"/>
      </button>
      <img src="../nvidia.png" class="nvidia" />
    </div>

    <div id="modal-mask">
      <div class="card-description">
        <p>
          The GeForce GTX 770 was a high-end graphics card by NVIDIA, launched
          on May 30th, 2013.
          <br />
          <br />
          Built on the 28 nm process, and based on the GK104 graphics processor, in its GK104-425-A2 variant, the card supports DirectX 12. Even though it supports DirectX 12, the feature level is only 11_0, which can be problematic with newer DirectX 12 titles. The GK104 graphics processor is an average sized chip with a die area of 294 mm² and 3,540 million transistors.
          <br />
          <br />
          It features 1536 shading units, 128 texture mapping units, and 32 ROPs. NVIDIA has paired 2,048 MB GDDR5 memory with the GeForce GTX 770, which are connected using a 256-bit memory interface. 
          <br />
          <br />
          The GPU is operating at a frequency of 1046 MHz, which can be boosted up to 1085 MHz, memory is running at 1753 MHz (7 Gbps effective). 
          <br />
          <br />
          Being a dual-slot card, the NVIDIA GeForce GTX 770 draws power from 1x 6-pin + 1x 8-pin power connector, with power draw rated at 230 W maximum. 
          <br />
          <br />
          Display outputs include: 2x DVI, 1x HDMI 1.4a, 1x DisplayPort 1.2. GeForce GTX 770 is connected to the rest of the system using a PCI-Express 3.0 x16 interface. The card's dimensions are 267 mm x 111 mm x 38 mm, and it features a dual-slot cooling solution.
          <br />
          <br />
          Its price at launch was 399 US Dollars.
        </p>
      </div>

      <div class="card-image770gtx">
        <img src="./770.png" alt="" />
      </div>
    </div>
  </div>
</template>

<script setup>

</script>

<style>
#modal-container {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
  
    z-index: 9998;
  
    background: linear-gradient(180deg, #000000 42.19%, rgb(13, 117, 11) 100%);
    
  }
  .card-description {
    color: #fff;
    text-align: left;
    width: 700px;
    font-size: 20px;
  
    margin-left: 3rem;
  }
  .card-image770gtx {
    margin-right: 20rem;
    margin-bottom: 20rem;
  }
  #modal-mask {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  .modal-close {
    background: none;
    border: none;
  }
  .controls {
      display: flex;
      flex-direction: row;
      justify-content: space-between;
      align-items: center;
      padding: 1rem;
  }
  .nvidia {
      height: 80px;
  }
</style>