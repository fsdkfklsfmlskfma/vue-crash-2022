<template>
  <div id="root">
    <div class="first-row">
      <gtx1080 />
      <gtx1070ti />
      <rtx2080 />
      <gtx1060 />
      <gtx1050 />
    </div>

    <div class="second-row">
      <gtx770 />
      <gtx750  />
      <rtx3090 />
      <rtx3060 />
      <gtx970 />
      
    </div>
  </div>
</template>

<script>
  import gtx1080 from './components/gtx1080/gtx1080.vue'
  import gtx1070ti from './components/gtx1070ti/gtx1070ti.vue'
  import rtx2080 from './components/rtx2080/rtx2080.vue'
  import gtx1060 from './components/gtx1060/gtx1060.vue'
  import gtx1050 from './components/gtx1050/gtx1050.vue'
  import gtx770 from './components/gtx770/gtx770.vue'
  import gtx750 from './components/gtx750/gtx750.vue'
  import rtx3090 from './components/rtx3090/rtx3090.vue'
  import rtx3060 from './components/rtx3060/rtx3060.vue'
  import gtx970 from './components/gtx970/gtx970.vue'


  export default {
    name: 'App',
    components: {
      gtx1080,
      gtx1070ti,
      rtx2080,
      gtx1060,
      gtx1050,
      gtx770,
      gtx750,
      rtx3090,
      rtx3060,
      gtx970,

    },
  }
</script>

<style>
* {
  margin: 0;
  padding: 0;
}

body {
  background: linear-gradient(180deg, #5AE077 0%, rgba(18, 19, 19, 0.58) 89.06%);
  background-repeat: no-repeat;
  /* padding: 5rem; */
  background-attachment: fixed;
}


.first-row, .second-row {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;
}

.second-row {
  margin-top: 3rem;
}





</style>
