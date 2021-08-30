<template>
    <div>
        <h1>Olá Vue!</h1>
        <p>Meu nome é {{ nome }} e trabalho como {{ profissao }}</p>
        <MultiplosEventos />
    </div>
</template>

<script>
    import MultiplosEventos from './MultiplosEventos.vue'
    export default {
        name: 'PrimeiroCompomente',
        components: {
            MultiplosEventos
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