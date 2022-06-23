<template>
  <div>
    <!-- <button
      class="btn btn-success"
      @click=" $emit( 'changeTitle', 'Vue CLI è molto bello' ) "
    > -->
    <button
      class="btn btn-success"
      @click="ChangeTitol"
    >
      {{ testoBottone }}
    </button>
  </div>
</template>

<script>
export default{
  name: 'BtnCambiaTitolo',
  props: [ 'testoBottone' ],
  data(){

  },
  methods: {
    ChangeTitol(){
      this.$emit( 'changeTitle', 'Vue CLI è molto bello' )
    }
  }
}

</script>
