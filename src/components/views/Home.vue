<template>
    <div class=" container py-4">
        <div class="row">
            <div class="col">
              <pesquisar-vaga></pesquisar-vaga>
            </div>
        </div>

        <div class="row mt-5">
            <div class="col-4">
              <indicador titulo="Vagas Abertas" indicador="100" bg="bg-dark" color="text-white"></indicador>
            </div>

            <div class="col-4">
              <indicador titulo="Profissionais cadastrados" indicador="150" bg="bg-dark" color="text-white"></indicador>
            </div>

            <div class="col-4">
              <indicador titulo="Visitantes Online" indicador="200" bg="bg-light" color="text-dark"></indicador>
            </div>
        </div>
    </div>
</template>

<script>
import PesquisarVaga from '@/components/comuns/PesquisarVaga.vue'
import Indicador from '../comuns/Indicador.vue';

export default {
    name: 'Home',
    components: {
        PesquisarVaga,
        Indicador
    },
}
</script>

<style>

</style>