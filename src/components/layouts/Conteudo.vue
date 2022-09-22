<template>
    <div>
        <h1>{{titulo}}</h1>
        <button @click="atualizarComponente()">Atualizar</button>
        <button @click="conteudo = 'home'">Home</button>
        <button @click="conteudo = 'publicar-vaga'">Publicar Vaga</button>
        <!-- renderizar de modo dinamico os componentes home e publicar vaga-->
        <!--<home></home>-->
        <!--<publicar-vaga></publicar-vaga>-->
        <component :is="conteudo" />
    </div>
</template>

<script>
import Home from '@/components/views/Home.vue'
import PublicarVaga from '@/components/views/PublicarVaga.vue' 
export default {
    name : 'Conteudo',
    components: {
        Home,
        PublicarVaga
    },
    data: () => ({
        teste: 'O componente foi criado',
        titulo: 'O titulo esta criado',
        conteudo: 'home'
    }),
    methods: {
        atualizarComponente() {
            this.titulo += '*';
        }
    }
}
</script>

<style scoped>
    h1 {
    color: blue;
    }
</style>