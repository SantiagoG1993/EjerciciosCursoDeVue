<template>
  <NavBar/>
<!-- <PrimerComponente/>
<SegundoComponente/> -->
</template>

<script>

/* import PrimerComponente from './components/PrimerComponente.vue'
import SegundoComponente from './components/SegundoComponente.vue' */
import NavBar from './components/header/NavBar.vue'
export default {
  name: 'App',
  components: {
/*     PrimerComponente, */
/*     SegundoComponente, */
    NavBar
  }
}
</script>

<style >
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
</style>
