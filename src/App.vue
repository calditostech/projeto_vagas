<template>
    <div>
      <h1>Componenente App</h1>
      <button @click="desmontarComponente()">Desmontar o componente conteudo</button>
      <TopoPadrao @nomeDoEventoQueSeraCapturadoNoComponentePai="acao()"/>
      <Conteudo v-if="visibilidade"></conteudo>
    </div>
</template>

<script>
import Conteudo from '@/components/layouts/Conteudo.vue';
import TopoPadrao from '@/components/layouts/TopoPadrao.vue';

export default {
  name: 'App',
  data: () => ({
    visibilidade: true
  }),
  components: {
    Conteudo,
    TopoPadrao
  },
  methods: {
    desmontarComponente() {
      this.visibilidade = false
    },
    acao() {
      console.log('Chegamos até o componente PAI')
    }
  }
}
</script>

<style>
h1 {
  color: red;
}
</style>
