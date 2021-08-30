<template>
    <div>
        <Header :esta_logado="true"/>
        <PrimeiroCompomente />
        <p class="paragrafo-pai">O dado de app é: {{ testando }}</p>
        <LifeCycle />
        <Pessoa />
    </div>
</template>

<script>
    import Header from './components/Header.vue'
    import PrimeiroCompomente from './components/PrimeiroComponente.vue'
    import LifeCycle from './components/LifeCycle.vue'
    import Pessoa from './components/Pessoa.vue'
    export default {
        name: 'App',
        components: {
            Header,
            PrimeiroCompomente,
            LifeCycle,
            Pessoa
        },
        data() {
            return {
                
            }
        },
    }
</script>

<style>
    body {
        background-color: #333;
        color: #FFF;
    }

    a {
        color: red;
    }

    .teste {
        background-color: black;
    }
</style>