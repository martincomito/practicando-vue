<template>
  <div>
    <!-- v-if sirve para evaluar cualquier expresión o variable que queramos, y con eso mostramos o no cierta info, en este caso con la prop edad que viene desde el lugar donde se llama el componente vamos a saber si soy mayor o menor -->
    <p v-if="edad >= 18">Sos mayor de edad</p>
    <p v-if="edad < 18">Sos menor, rajá de acá</p>
  </div>
</template>

<script>
export default {
  props: {
    edad: Number
  },
  data () {
    return {

    }
  }
}
</script>

<style>

</style>