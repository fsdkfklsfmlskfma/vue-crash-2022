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
          The GeForce GTX 1080 was a high-end graphics card by NVIDIA, launched
          on May 27th, 2016.
          <br />
          <br />
          Built on the 16 nm process, and based on the GP104 graphics processor,
          in its GP104-400-A1 variant, the card supports DirectX 12. This
          ensures that all modern games will run on GeForce GTX 1080. The GP104
          graphics processor is a large chip with a die area of 314 mm² and
          7,200 million transistors.
          <br />
          <br />
          It features 2560 shading units, 160 texture mapping units, and 64
          ROPs. NVIDIA has paired 8 GB GDDR5X memory with the GeForce GTX 1080,
          which are connected using a 256-bit memory interface.
          <br />
          <br />
          The GPU is operating at a frequency of 1607 MHz, which can be boosted
          up to 1733 MHz, memory is running at 1251 MHz (10 Gbps effective).
          <br />
          <br />
          Being a dual-slot card, the NVIDIA GeForce GTX 1080 draws power from
          1x 8-pin power connector, with power draw rated at 180 W maximum.
          <br />
          <br />
          Display outputs include: 1x DVI, 1x HDMI 2.0, 3x DisplayPort 1.4a.
          GeForce GTX 1080 is connected to the rest of the system using a
          PCI-Express 3.0 x16 interface. The card's dimensions are 267 mm x 112
          mm x 40 mm, and it features a dual-slot cooling solution.
          <br />
          <br />
          Its price at launch was 599 US Dollars.
        </p>
      </div>

      <div class="card-image1060gtx">
        <img src="./1060.png" alt="" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    show: Boolean,
  },
};
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
  .card-image1060gtx {
       transform: rotate(20deg);
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