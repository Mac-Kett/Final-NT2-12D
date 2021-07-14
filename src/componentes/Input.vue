<template>
  <section class="src-componentes-entrada">
    <div class="jumbotron">
    <h1>Macarena Agustina Quiroz</h1>
    <h2>Comision: 21D</h2>
    <h2>Docente: Daniel Sanchez</h2>
    <br>
      <h3>Escriba aqui...</h3>
      <input type="text" v-model="valor" /> <br />
      <br />
      {{ valor | codificado }} codificado
      <br />
      {{ valor | pasarAmayuscula }} | mayuscula
      <br />
      {{ valor | pasarAminuscula }} | minuscula
      <br />
      {{ valor | intercalaDesdeMayuscula }} | intercalado iniciado por mayuscula
      <br />
      {{ valor | intercalaDesdeMinuscula }} | intercalado iniciado por minuscula
      <br />
      {{ cantidadCaracteres }} | cantidad de caracteres ingresados
    </div>
   


    <p>respuestas: 1:b 2:b 3:c 4:b 5:b</p>
  </section>
</template>

<script lang="js">
  
  export default  {
    name: 'src-componentes-entrada',
    props: [],
    mounted () {

    },
    mixins: [],
    data () {
      return {
        valor: '',

      }
    },
    methods: {
       
    },
    computed: {
        cantidadCaracteres(){
        return this.valor.length
      }
    }
}


</script>

<style scoped lang="css">
.src-componentes-estructura {
}

.jumbotron {
  background-color: white;
}

hr {
  background-color: #444;
}
</style>
