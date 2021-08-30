<template>
    <div>
        <h1>Olá Vue!</h1>
        <Reutilizacao />
        <Reutilizacao />
        <Reutilizacao />
        <Reutilizacao />
        <p>Meu nome é {{ nome }} e trabalho como {{ profissao }}</p>
        <MultiplosEventos />
    </div>
</template>

<script>
    import MultiplosEventos from './MultiplosEventos.vue'
    import Reutilizacao from './Reutilizacao.vue'
    export default {
        name: 'PrimeiroCompomente',
        components: {
            MultiplosEventos,
            Reutilizacao
        },
        data() {
            return {
                nome: 'Henington',
                profissao: 'Desenvolvedor'
            }
        },
    }
</script>

<style>

</style>