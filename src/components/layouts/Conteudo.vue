<template>
    <div>
        <h1>Conteúdo</h1>
        <home></home>
        <publicar-vaga></publicar-vaga>
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
    }
}
</script>

<style scoped>
    h1 {
    color: blue;
    }
</style>