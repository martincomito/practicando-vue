
<template>
  <div>
    <!-- Por cada elemento en la prop botones va a renderizar (mostrar) un botón con su título y mensaje cuando se haga click -->
    <button 
      class="separado"
      v-for="elemento in botones"
      :key="elemento.key"
      @click="mostrarMensaje(elemento.mensaje)"
    >
      {{ elemento.titulo }}
    </button>
  </div>
</template>

<script>
export default {
  name: "Inicio",
  // ! Prop es todo lo que me llega desde afuera cuando usan este componente en otro lado. En este caso sabemos que es un array que se llama botones, si mando otra cosa que no sea un array me va a decir que el tipo de prop es incorrecto.
  props: {
    botones: Array
  },
  // ! Methods = Funciones
  // ! Esta función recibe un mensaje y lo muestra en el alert, cuando hacemos click porque está más arriba con el @click.
  methods: {
    mostrarMensaje (unMensaje) {
      alert(unMensaje)
    }
  }
};
</script>

<style scoped>
 .separado {
   margin-top: 4rem;
   margin-right: 2rem;
 }
</style>
