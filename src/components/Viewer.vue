<template>
  <div id="viewer"></div>
</template>

<script>
import ViewerJS from './classes/viewer.js'
export default {
  name: 'Viewer',
  componentes: {
    ViewerJS
  },
  data() {
    return {
      width: 100,
      height: 100,
      viewer: null
    }
  },
  mounted() {
    this.initViewer();
    this.addViewer();
  },
  methods: {
    initViewer() {
      this.viewer = new ViewerJS(window.innerWidth-30, window.innerHeight);
    },
    addViewer() {
      document.getElementById("viewer").appendChild(this.viewer.renderer.domElement);
    }
  },  
}
</script>

<style scoped>
  #viewer {
    float: left;
  }
</style>