<template>
  <div>
    <Header />
    <Hero />
    <Colecciones />
    <ListaProductos />
    <Footer />
  </div>
</template>

<script>

import Colecciones from './src/components/colecciones.vue';
import Header from './src/components/header.vue'
import Hero from './src/components/hero.vue'
import 'flowbite/dist/flowbite.css';
import ListaProductos from './src/components/listaProductos.vue';
import Footer from './src/components/footer.vue';

export default {
  name: 'Onapolo',
  components: {
    Header,
    Hero,
    Colecciones,
    ListaProductos,
    Footer,
    setup() {
    onMounted(() => {
      // Aquí puedes inicializar cualquier codigo
      initFlowbite();
      if (typeof document !== 'undefined') {
        // Código que interactúa con el DOM
        console.log('El componente se ha montado en el cliente.');
      }
    });
  },
  }
}
</script>
