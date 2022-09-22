<template>
      <div class="h-100 p-5 bg-light border rounded-3">
        <h2>Pesquisar Vagas</h2>
        <div class="row">
            <div class="col">
                <div class="form-group">
                    <label>Título da Vaga</label>
                    <input type="text" class="form-control" placeholder="Pesquise por palavras chaves, por exemplo 'PHP', Analista">
                    <small class="form-text text-muted">Informe palavras que estejam relacionadas com titulo da vaga que voce procura</small>
                </div>
            </div>
        </div>
        <div class="row">
            <div class="col">
                <button class="btn btn-outline-dark mt-2" type="button">Buscar</button>
            </div>
        </div>
    </div>
</template>

<script>
export default {
   name: 'PesquisaVaga'
}
</script>

<style>

</style>