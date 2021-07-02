<template>
  <div id="app">
    <!-- <ListaDeBotones :botones="botones" /> -->
    <ContenidoExplicito :edad="10"/>
  </div>
</template>

<script>
/* eslint-disable */
import ListaDeBotones from '@/components/ListaDeBotones.vue'
import ContenidoExplicito from '@/components/ContenidoExplicito.vue'

export default {
  components: {
    ListaDeBotones,
    ContenidoExplicito
  },
  data () {
    return {
      // botones: [
      //   { titulo: "Culo", key: 1, mensaje: 'que piola' },
      //   { titulo: "Culo2", key: 2, mensaje: 're cheto' },
      //   { titulo: "Culoasdas", key: 3, mensaje: 'aaaaasa'}
      // ]
    }
  }
}
</script>
