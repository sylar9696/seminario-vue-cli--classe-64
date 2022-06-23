<template>
  <div id="app" class="text-center p-5">

    <div>
      <h2>{{ TitoloPagina }}</h2>
      <!-- COmponente figlio -->
      <BtnCambiaTitolo
        testoBottone="Cliccami per cambiare titolo"
        @changeTitle="funzioneCambiaTitolo"
      />
      <!-- <BtnCambiaTitolo testoBottone="nuovo titolo bottone"/> -->
    </div>

    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import BtnCambiaTitolo from './components/BtnCambiaTitolo.vue'

export default {
  name: 'App',
  data(){
    return{
      TitoloPagina: 'Vue Cli Emit'
    }
  },
  components: {
    // HelloWorld
    BtnCambiaTitolo
  },
  methods: {
    funzioneCambiaTitolo( valoreEmit ){
      this.TitoloPagina = valoreEmit;
    }
  }
}
</script>

<style lang="scss">

</style>
