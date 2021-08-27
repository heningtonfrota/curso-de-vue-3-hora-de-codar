<template>
    <div>
        <PrimeiroCompomente />
        <LifeCycle />
        <Pessoa />
    </div>
</template>

<script>
    import PrimeiroCompomente from './components/PrimeiroComponente.vue'
    import LifeCycle from './components/LifeCycle.vue'
    import Pessoa from './components/Pessoa.vue'
    export default {
        name: 'App',
        components: {
            PrimeiroCompomente,
            LifeCycle,
            Pessoa
        }
    }
</script>

<style>

</style>